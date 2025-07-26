WEEK 8 Reflection

This week deepened our dive into hash tables, and while I came away with a working version, comparing it to the instructor’s implementation really brought some of my blind spots into focus. There were a few key areas where my code worked, but lacked some of the structure, safety, or abstraction that make for truly clean and maintainable design.

One thing I missed was consistently using helper methods to encapsulate repeated logic. For example, the instructor used a hashposition() method to compute array indices, whereas I duplicated that same logic inline multiple times. It wasn’t wrong, but it wasn’t clean—and I can see how that kind of redundancy makes code harder to maintain or refactor later.

I also didn’t handle null safety in my contains() method, which means it could throw an error if someone tries to check for a `null` value. That’s a small detail, but one that points to a larger takeaway: robust code isn’t just about making it *work*—it’s about anticipating edge cases and protecting against them.

Another subtle but important difference was type safety. I used some raw types in my toString() method and array declarations, while the instructor properly used generics with casting. My version technically compiles, but it introduces unnecessary warnings and undermines Java’s strong typing system.

Where I did feel more confident was in the rehashing logic. I opted to re-link nodes directly instead of re-inserting them through add(). It’s more efficient, and I’m glad I saw that opportunity—but I also realize it makes the code more complex, and more prone to subtle bugs if not handled carefully. So even in areas where I thought I was “improving” the design, there’s a tradeoff to understand.

Looking at the instructor’s code helped me appreciate how abstraction, consistency, and clarity can elevate even a basic data structure implementation. It’s not just about passing the test cases; it’s about writing code that other people (or my future self) can trust, extend, and understand.

Overall, this week was a useful checkpoint. I’m starting to see the difference between functional and *good* design, and I know where I need to sharpen my instincts. I’m hoping that with more practice—and more careful observation of the example code—I can get better at anticipating these patterns and avoiding the small missteps before they pile up.

