kreb-scout
==========

kreb-scout is a library of math problems which are written as feivel templates and intended for use in latex documents to be processed with ximera.

Here's the idea:
1) ximera takes a latex file and presents it interactively on the web.
2) feivel takes a template and turns it into a latex file.
3) kreb-scout is a library of pre-written templates.

Writing a problem template for kreb-scout can be a little complicated. But eventually with a large and easy-to-use library we can simply import even complicated problems.


Problems which need solving
---------------------------
* Discoverability: As the library grows, just knowing what exists is hard. Need a (preferably automated) way to organize/search. Tags?
* Documentation: Feivel templates are naturally literate due to semantics of import. Make the library its own documentation. Key features: hyperlinking between sections, show all parameters with meaning, description of problem, examples. HTML with embedded latex seems a natural choice. (pandoc?)

Idea: can both of these problems be solved by making kreb-scout a literate hakyll site?


Theory of problem templates
---------------------------
A good source of problem templates is concrete problems: take a specific math problem and try to generalize it.

This is not as simple as taking an existing problem and randomly changing the numbers. To give a simple example, suppose we'd like to have our students factor a polynomial. Depending on the coefficients, this can test many different skills. Consider things like $x^2 + 2x + 1$, $x^2 + 3x + 1$, and $x^2-1$.

Instead, to generalize a problem to a template it is helpful to start with the answer and work "backwards". Ask: what skills does this problem actually require? What skills do I want to test? What is it about the structure of this problem that make it test the skills that it does? I have found that in college algebra, at least, answering these questions requires some number theory. (That's why feivel has to know some arithmetic.)
