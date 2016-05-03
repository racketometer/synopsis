# ONK Report

## Graphics
To add an illustration or image use

```
\graphic{width}{path}{caption}{label}
```

`width` is relative to page width

`path` is relative to `graphics/` folder

## Source code

There are three definfed languages in the `LstListingsLanguages.tex` file.

Here is an example of Java code. Remember to prefix labels for source code with `lst:`.

```
\lstsetjava
\begin{lstlisting}[caption=Showing Java, label=lst:awesomeCode]
class HelloWorldApp {
    public static void main(String[] args) {
        System.out.println("Hello World!"); // Display the string.
        for (int i = 0; i < 100; ++i) {
            System.out.println(i);
        }
    }
}
\end{lstlisting}
```

## Citations
Add references to `Literature.bib`.
When adding or using new references, run one BibTex and two Quick Builds to display the data.

### Web pages

```
Something about ASP.NET \citep{aspnetmvcWeb}.
```


```
@misc{aspnetmvcWeb,
	author = {Microsoft},
	title = {{ASP.NET MVC}},
	url = {http://www.asp.net/mvc},
	year = {2014},
	note = {Accessed 24.05.2015},
}
```

### Books
```
As Johnson explains in Design Patterns \citep[p. 185-193]{gof}...
```

```
@book{gof,
    author = {Gamma, E. and Helm, R. and and Johnson, R. and Vlissides, J.},
    title = {Design Patterns},
    publisher = {Addison Wesley},
    year = {2005}
}
```
