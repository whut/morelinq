# Introduction #

Even though Linq operators are implemented as simple extension methods, their execution behavior can be a little unexpected. Most of our operators try to be as lightweight and efficient as possible. Hence we stream their results whenever possible, which allows for better composition, working on infinite sequences and easy parallelization.
This list serves as a description of certain keywords we use to describe an operators behavior, it does not describe a set of categories an operator can be put in. Although some keywords appear to describe opposite behavior, they are sometime used on the same operator to exactly describe the evaluation of its inputs.

### Point of Execution: ###
  * **Deferred execution**  means no elements are fetched from source sequences until the first element is fetched from the result sequence. This applies to basically all LINQ to Objects operators which return a sequence interface. (It doesn't apply to ToArray or ToList of course.)
  * If **Immediate execution**, the first call to the operator will result in the entire source sequence being processed. A temporary copy of the source sequence might also be required.

### Execution Strategy: ###
  * An operation is **streaming** if it only fetches elements from the source sequence as it requires them, and does not store those elements internally unless otherwise specified. Streaming operators support infinite sequences.
  * An operation is **buffering** if it drains the source sequence (i.e. fetches all the elements) when the first element of the result sequence is fetched, and stores the items internally. Buffering operators don't support infinite sequences.