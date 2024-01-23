

<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN"
  "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>1</title>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
  <link rel="stylesheet" type="text/css" href="../../stylesheet.css"/>
<link rel="stylesheet" type="text/css" href="../../page_styles.css"/>
</head>
  <body class="calibre1">
  <h1 class="tochead"><a id="pgfId-998427"></a>1 Developing a pragmatic learning strategy</h1>

  <p class="co-summary-head"><a id="pgfId-1003461"></a>This chapter covers</p>

  <ul class="calibre11">
    <li class="co-summary-bullet"><a class="calibre" id="pgfId-1003493"></a>What being pragmatic means</li>

    <li class="co-summary-bullet"><a class="calibre" id="pgfId-1003494"></a>What Python can do</li>

    <li class="co-summary-bullet"><a class="calibre" id="pgfId-1003495"></a>When you should consider alternative languages</li>

    <li class="co-summary-bullet"><a class="calibre" id="pgfId-1003482"></a>What you can expect to learn from this book</li>
  </ul>

  <p class="body"><a class="calibre" id="pgfId-998495"></a>Python is an amazing programming language. Its open source, general-purpose, platform-independent nature has given it an enormous developer community, along with an incredible ecosystem that includes tens of thousands of freely available libraries for web development, machine learning (ML), data science, and many other domains. I hope that we share this belief: knowing how to code in Python is great, but knowing how to write truly efficient, secure, and maintainable applications gives you a tremendous advantage. This book will help you go from a Python beginner to confident programmer.</p>

  <p class="body"><a class="calibre" id="pgfId-998524"></a>In the Python ecosystem, we use domain-specific Python tools, such as web frameworks and ML libraries, to complete various tasks in our jobs. The effective employment of these tools is nontrivial, as it requires considerable familiarity with essential Python skills, such as processing texts, dealing with structured data, creating control flows, and handling files. Python programmers can write different solutions to address the same tasks. Among these solutions, one is generally better than the others because it may be more concise, more readable, or more efficient, which we collectively term as <i class="fm-italics">Pythonic:</i> an idiomatic coding style that all Python programmers strive to acquire. This book is about how to write Pythonic code to address pro-gramming tasks.</p>

  <p class="body"><a class="calibre" id="pgfId-998541"></a>Python is so well developed and has so many features to learn that it would be impossible or unwise to try to learn everything about it from this book. Instead, I’ll take a pragmatic approach to defining what I’ll teach in this book: the essential skills that you’ll most likely use in your projects. Equally important, I’ll frequently mention how to use these skills with the consideration of readability and maintainability so that you can form good coding habits, which I’ll bet that you and your teammates will greatly appreciate.</p>

  <p class="fm-callout"><a id="pgfId-998593"></a><span class="fm-callout-head">Note</span> You’ll see callouts like this one throughout the book. Many of them are devoted to tips regarding readability and maintainability. Don’t miss them!</p>

  <h2 class="fm-head" id="sigil_toc_id_12"><a id="pgfId-998610"></a>1.1 Aiming at becoming a pragmatic programmer</h2>

  <p class="body"><a class="calibre" id="pgfId-998622"></a>We <a class="calibre" id="marker-999250"></a>code for purposes, such as building websites, training ML models, or analyzing data. Whatever our purposes are, we want to be pragmatic; we write code to solve real problems. Thus, before we learn to code from the beginning or advance our coding skills in the middle of our career, we should be clear about our intentions. But even if you’re unsure of what you desire to achieve with Python at this stage, the good news is that core Python features are universal knowledge. After you grasp the core features, you can apply them to any domain-specific Python tools.</p>

  <p class="body"><a class="calibre" id="pgfId-998650"></a>Aiming to become a pragmatic programmer means that you should focus on the techniques that are most useful. Mastering these skills is just the first milestone in your journey, however; the long-term game in coding is writing readable code that not only works, but also fosters maintainability.</p>

  <h3 class="fm-head1" id="sigil_toc_id_13"><a id="pgfId-998677"></a>1.1.1 Focusing on writing readable Python code</h3>

  <p class="body"><a class="calibre" id="pgfId-998686"></a>As <a class="calibre" id="marker-999258"></a><a class="calibre" id="marker-999262"></a>a developer, I’m obsessed with readability. Writing code is like speaking a real-world language. When we speak a language, don’t we want others to understand us? If your answer is yes, you probably agree with me that we want others to understand our code too. Whether our code’s readers possess the necessary technical expertise to understand our code is out of our control. What we can control is how we write the code—how readable we make it. Consider some simple questions:</p>

  <ul class="calibre11">
    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-998711"></a><i class="fm-italics">Are your variables named properly to indicate what they are?</i> No one can appreciate your code if it’s full of variables named <span class="fm-code-in-text">var0</span>, <span class="fm-code-in-text">temp_var</span>, or <span class="fm-code-in-text">x</span>, for example.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-998738"></a><i class="fm-italics">Do your functions have proper signatures to indicate what they do?</i> People are lost if they see functions named <span class="fm-code-in-text">do_data(data)</span> or <span class="fm-code-in-text">run_step1()</span>.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-998759"></a><i class="fm-italics">Do you organize your code consistently across files?</i> People expect different files of the same type to use similar layouts. Do you place <span class="fm-code-in-text">import</span> statements at the top of your files, for example?</p>
    </li>

    <li class="fm-list-bullet-last">
      <p class="list"><a class="calibre" id="pgfId-998786"></a><i class="fm-italics">Is your project folder structured with specific files stored in the desired folders?</i> When your project’s scope grows, you should create separate folders for related files.</p>
    </li>
  </ul>

  <p class="body"><a class="calibre" id="pgfId-998801"></a>These example questions pertain to readability. We don’t just ask them from time to time; instead, we ask these kinds of readability questions throughout our projects. The reason is simple: <i class="fm-italics">good</i> practice makes perfect. Trained as a neuroscientist, I know exactly how the brain works when it comes to behavioral learning. By practicing readability through these self-checking questions, we’re training our brain’s neural circuits. In the long term, your brain will be trained to know what behaviors constitute good practice in coding, and you’ll write readable and maintainable code without even thinking about <a class="calibre" id="marker-999270"></a><a class="calibre" id="marker-999274"></a>it.</p>

  <h3 class="fm-head1" id="sigil_toc_id_14"><a id="pgfId-998843"></a>1.1.2 Considering maintainability even before you write any code</h3>

  <p class="body"><a class="calibre" id="pgfId-998852"></a>In <a class="calibre" id="marker-999282"></a><a class="calibre" id="marker-999290"></a>rare cases, we write code for one-time use. When we write a script, we almost always succeed in convincing ourselves that we’ll never use the script again; thus, we don’t care about creating good variable names, laying out the code properly, or refactoring functions and data models, not to mention making sure that we leave no comments (or outdated ones). But how many times did it turn out that we had to use the same script the next week or even the following day? This has probably happened to most of us.</p>

  <p class="body"><a class="calibre" id="pgfId-998892"></a>The previous paragraph describes a mini-scale maintainability problem. In this case, it affects only your own productivity in a short span of time. If you work in a team environment, however, problems introduced by individual contributors add up to large-scale maintainability problems. The team members fail to follow the same naming rules for variables, functions, and files. Countless incidents of commented-out code remain. Outdated comments are everywhere.</p>

  <p class="body"><a class="calibre" id="pgfId-998919"></a>To address maintainability problems in a later stage of your own projects, you should build a good mindset when you’re learning to code. Following are some questions that you might consider to help you develop a good “maintainability” mindset for the long run:</p>

  <ul class="calibre11">
    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-998943"></a><i class="fm-italics">Is your code free of outdated comments and commented-out code?</i> If the answer is no, update or delete them! These situations are even worse than those without any comments because they may provide conflicting information.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-998961"></a><i class="fm-italics">Is there considerable duplication in the code?</i> If the answer is yes, refactoring is probably warranted. A rule of thumb in coding is <i class="fm-italics">DRY</i> (Don’t Repeat Yourself<a class="calibre" id="marker-999294"></a>). By removing duplicates, you’ll deal with a single shared portion, which is less prone to bugs than changes in repeated parts.</p>
    </li>

    <li class="fm-list-bullet-last">
      <p class="list"><a class="calibre" id="pgfId-998994"></a><i class="fm-italics">Do you use version-control tools such as Git?</i> If the answer is no, look at the extensions or plugins of your integrated development environment (IDE<a class="calibre" id="marker-999298"></a><a class="calibre" id="marker-999302"></a>). For Python, common IDEs include PyCharm and Visual Studio Code. Many IDEs have integrated version-control tools that make it much easier to manage versions.</p>
    </li>
  </ul>

  <p class="body"><a class="calibre" id="pgfId-999041"></a>Being a pragmatic Python programmer requires this type of maintainability training. After all, almost all Python tools are open source and evolving rapidly. Thus, maintainability should be the cornerstone of any viable project. Throughout the book, where applicable, we’ll touch base on how to implement maintainability practices in our daily Python coding. Please remember that readability is the key to sustained maintainability. When you focus on writing readable code, your codebase’s maintainability <a class="calibre" id="marker-999306"></a><a class="calibre" id="marker-999314"></a>improves <a class="calibre" id="marker-999318"></a>consequentially.</p>

  <h2 class="fm-head" id="sigil_toc_id_15"><a id="pgfId-999068"></a>1.2 What Python can do well or as well as other languages</h2>

  <p class="body"><a class="calibre" id="pgfId-999083"></a>Python owes its growing popularity to the characteristics of the language itself. Although none of these characteristics is unique to Python, when they were organically combined, Python was set to grow into a widely adopted language. The following list summarizes Python’s key characteristics:</p>

  <ul class="calibre11">
    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-999103"></a><i class="fm-italics">Cross-platform</i>—Python runs on common platforms, such as Windows, Linux, and MacOS. Thus, Python code is transferrable. Any code that you write on your own platform can run on other computers without any restrictions imposed by the differences between platforms.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-999123"></a><i class="fm-italics">Expressive and readable</i>—Python’s syntax is simpler than that of many other languages. The expressive, readable coding style is widely adopted by Python programmers. You’ll find that well-written Python code is enjoyable to read, just like well-written prose.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-999147"></a><i class="fm-italics">Fast for prototyping</i>—Given its simple syntax, Python code is generally more concise than code written in other languages. Thus, it requires less work to produce a functional prototype in Python than in other languages.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-999168"></a><i class="fm-italics">Standalone</i>—When you install Python on your computer, it becomes ready to use right after “unboxing.” The basic Python installation package consists of all essential libraries that you need to perform any routine coding work.</p>
    </li>

    <li class="fm-list-bullet-last">
      <p class="list"><a class="calibre" id="pgfId-999187"></a><i class="fm-italics">Open source, free, and extensible</i>—Although Python works standalone, you can write and use your own packages. If others have published any packages you need, you can install them with a one-line command without worrying about license or subscription fees.</p>
    </li>
  </ul>

  <p class="body"><a class="calibre" id="pgfId-999209"></a>These key characteristics have attracted many programmers, forming a tremendous developer community. The open source nature of Python allows interested users to contribute to this language and its ecosystem in general. Table 1.1 summarizes some notable domains and their respective Python tools. This table isn’t an exhaustive list, and you’re encouraged to explore Python tools in the specialty domain of your own interest.</p>

  <p class="fm-table-caption"><a id="pgfId-1003690"></a>Table 1.1 Overview of domain-specific Python tools</p>

  <table border="1" class="contenttable" width="100%">
    <tbody><tr class="calibre12">
      <th class="fm-contenttable1" colspan="1" rowspan="1">
        <p class="fm-table-head"><a id="pgfId-1003696"></a>Domain</p>
      </th>

      <th class="fm-contenttable1" colspan="1" rowspan="1">
        <p class="fm-table-head"><a id="pgfId-1003698"></a>Tool</p>
      </th>

      <th class="fm-contenttable1" colspan="1" rowspan="1">
        <p class="fm-table-head"><a id="pgfId-1003700"></a>Highlights</p>
      </th>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003702"></a><b class="fm-bold">Web development</b></p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003704"></a>Flask</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003706"></a>A micro web framework; good for building lightweight web apps; flexible extensibility for third-party functionalities</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="3">
        <p class="fm-table-body"><a id="pgfId-1003708"></a><b class="fm-bold">Web development</b></p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003710"></a>Django</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003712"></a>A complete web framework; good for building database-driven web apps; highly scalable as an enterprise solution</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003716"></a>FastAPI</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003718"></a>A web framework for building application programming interfaces (APIs); data validation and data conversion; automatic generation of API web interfaces</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003722"></a>Streamlit</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003724"></a>A web framework for easy building of data-related apps; popular among data scientists and ML engineers</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="5">
        <p class="fm-table-body"><a id="pgfId-1003726"></a><b class="fm-bold">Data science</b></p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003728"></a>NumPy</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003730"></a>Specialized for processing large, multidimensional arrays; high computational efficiency; integral to many other libraries</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003734"></a>pandas</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003736"></a>A versatile package for processing spreadsheet-like two-dimensional data; comprehensive data manipulations</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003740"></a>statsmodels</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003742"></a>A popular package for statistics, such as linear regression, correlation, Bayesian modeling, and survival analysis</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003746"></a>Matplotlib</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003748"></a>An object-oriented paradigm for drawing histograms, scatter plots, pie charts, and other common figures with a variety of customizable settings</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003752"></a>Seaborn</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003754"></a>An easy-to-use visualization library for drawing attractive graphics; high-level APIs based on Matplotlib</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="5">
        <p class="fm-table-body"><a id="pgfId-1003756"></a><b class="fm-bold">Machine learning</b></p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003758"></a>Scikit-learn</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003760"></a>A wide range of preprocessing tools for building ML models; implementation of common ML algorithms</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003764"></a>TensorFlow</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003766"></a>A framework with both high- and low-level APIs; Tensor board visualization tool; good for building complex neural networks</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003770"></a>Keras</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003772"></a>High-level APIs for building neural networks; easy to use; good for building low-performance models</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003776"></a>PyTorch</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003778"></a>A framework for building neural networks; more intuitive code styles than TensorFlow; good for building complex neural networks</p>
      </td>
    </tr>

    <tr class="calibre12">
      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003782"></a>FastAI</p>
      </td>

      <td class="fm-contenttable2" colspan="1" rowspan="1">
        <p class="fm-table-body"><a id="pgfId-1003784"></a>High-level APIs for building neural networks on top of PyTorch; easy to use</p>
      </td>
    </tr>
  </tbody>
</table>

  <div class="fm-sidebar-block">
    <p class="fm-sidebar-title"><a class="calibre" id="pgfId-1006216"></a><a id="marker-1004160"></a>Frameworks, libraries, packages, and modules</p>

    <p class="fm-sidebar-text"><a id="pgfId-1006218"></a>When we discuss tools, we use several closely related terms, including <i class="fm-italics">frameworks</i><a id="marker-1006217"></a>, <i class="fm-italics">libraries</i><a id="marker-1006219"></a>, <i class="fm-italics">packages</i><a id="marker-1006220"></a>, and <i class="fm-italics">modules</i>. Different languages may use some of these terms and have slightly different meanings. Here, I discuss the meanings of these terms that most Python programmers accept.</p>

    <p class="fm-sidebar-text"><a id="pgfId-1006222"></a><i class="fm-italics">Frameworks</i><a id="marker-1006221"></a> have the largest scope. Frameworks provide a complete set of functionalities that are designed to perform a dedicated job at a high level, such as web development.</p>

    <p class="fm-sidebar-text"><a id="pgfId-1006251"></a><i class="fm-italics">Libraries</i><a id="marker-1004162"></a><a id="marker-1004225"></a><a id="marker-1006238"></a> are building blocks of frameworks, consisting of packages. Libraries provide functionalities without users having to worry about the underlying packages.</p>

    <p class="fm-sidebar-text"><a id="pgfId-1006241"></a><i class="fm-italics">Packages</i><a id="marker-1004227"></a><a id="marker-1004163"></a><a id="marker-1006240"></a> provide specific functionalities. More specifically, packages bundle modules, and each module consists of a set of closely related data structures and functions in a single file, such as a .py file.</p>
  </div>

  <h2 class="fm-head" id="sigil_toc_id_16"><a id="pgfId-999852"></a>1.3 What Python can’t do or can’t do well</h2>

  <p class="body"><a class="calibre" id="pgfId-999864"></a>Everything has limits, and so does Python. There are many things that Python can’t do, or at least can’t do well compared with alternative tools. Although some people are trying to push Python in such a way that we can use it for other purposes, at this stage, we should know its limits in two important areas:</p>

  <ul class="calibre11">
    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-999899"></a><i class="fm-italics">Mobile applications</i>—In this mobile age, we all have smartphones and use apps in almost every aspect of life, such as banking, online shopping, health, communications, and certainly gaming. Unfortunately, there have been no great Python frameworks for developing smartphone apps despite attempts such as Kivy and BeeWare. If you work in mobile development, you should consider mature alternatives such as Swift for iOS apps and Kotlin for Android apps. As a pragmatic programmer, you choose a language that leads to a product with the best user experience.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-999932"></a><i class="fm-italics">Low-level development</i><a class="calibre" id="marker-1000654"></a>—When it comes to developing software that interacts directly with hardware, Python isn’t the best choice. Due to the interpreted nature of Python, the overall execution speed isn’t fast enough for developing low-level software, such as device drivers, which require instant responsiveness. If you’re interested in developing software at a low level, you should consider alternative languages that are better at interfacing with the hardware. C and C++ are good options for developing device drivers, for example.</p>
    </li>
  </ul>

  <h2 class="fm-head" id="sigil_toc_id_17"><a id="pgfId-999966"></a>1.4 What you’ll learn in this book</h2>

  <p class="body"><a class="calibre" id="pgfId-999980"></a>We’ve talked a little bit about what it means to be a pragmatic programmer. Now let’s talk about how you’re going to get there. As you write programs, you’ll inevitably run into new programming challenges. In this book, we’ve identified the programming techniques you’ll need to take for the tasks you’re most likely to encounter.</p>

  <h3 class="fm-head1" id="sigil_toc_id_18"><a id="pgfId-1000001"></a>1.4.1 Focusing on domain-independent knowledge</h3>

  <p class="body"><a class="calibre" id="pgfId-1000010"></a>All <a class="calibre" id="marker-1000662"></a>things are connected in some way directly or indirectly, and so is Python knowledge. To put this discussion in a context, consider figure 1.1. We can conceptualize Python features and its applications as three related entities.</p>

  <p class="fm-figure"><img alt="CH01_F01_Cui" class="calibre2" src="../Images/CH01_F01_Cui.png"/><br class="calibre3"/></p>

  <p class="fm-figure-caption"><a id="pgfId-1006255"></a>Figure 1.1 The relationship between domain-independent and domain-specific Python knowledge. Domain-independent knowledge includes basic and advanced Python features, which are closely related. Together, they form the basis for domain-specific knowledge in distinct content domains.</p>

  <p class="body"><a class="calibre" id="pgfId-1000027"></a>The goal of learning Python for most of us is to apply Python to address problems in the domain where we work, which requires <i class="fm-italics">domain-specific Python knowledge,</i> such as web development and data science. As a prerequisite for fulfilling your job, your knowledge base should encompass essential Python features—more specifically, <i class="fm-italics">domain-independent Python knowledge.</i> Even when your job role switches or evolves, you can apply the essential Python knowledge to your new position.</p>

  <p class="body"><a class="calibre" id="pgfId-1000073"></a>In this book, you’ll focus on gaining domain-independent Python knowledge. To facilitate the learning process, we can operationally define domain-independent Python knowledge as two building components: the basic and the advanced.</p>

  <p class="body"><a class="calibre" id="pgfId-1000090"></a>For the basics, we should know common data structures and their manipulations. We also need to know how to evaluate conditions to construct the <span class="fm-code-in-text">if...else...</span> statement<a class="calibre" id="marker-1000666"></a>. When we perform repeated work, we can take advantage of <span class="fm-code-in-text">for</span><a class="calibre" id="marker-1000670"></a> and <span class="fm-code-in-text">while</span> loops<a class="calibre" id="marker-1000674"></a>. To reuse blocks of code, we can refactor them into functions and classes. Mastering these basics is sufficient for writing useful Python code to perform your job tasks. If you know most of the basics, you’re ready to learn the advanced skills.</p>

  <p class="body"><a class="calibre" id="pgfId-1005070"></a>The advanced skills enable you to write better code that’s more efficient and that takes advantage of versatile Python features. Let’s see a simple example to feel the versatility of Python. When we use a <span class="fm-code-in-text">for</span> loop to iterate a <span class="fm-code-in-text">list</span> object, we often need to show the position of each item beside the item itself, such as</p>
  <pre class="programlisting">prime_numbers = [2, 3, 5]
 
# desired output:
Prime Number #1: 2
Prime Number #2: 3
Prime Number #3: 5</pre>

  <p class="body"><a class="calibre" id="pgfId-1005077"></a>If we use only the basic features, we may come up with the following solution. In the solution, we create a <span class="fm-code-in-text">range</span> object that allows retrieval of the 0-based index to produce the position information. For the output, we use string concatenation:</p>
  <pre class="programlisting">for num_i in range(len(prime_numbers)):
    num_pos = num_i + 1
    num = prime_numbers[num_i]
    print("Prime Number #" + str(num_pos) + ": " + str(num))</pre>

  <p class="body"><a class="calibre" id="pgfId-1005082"></a>However, after you read this book, you’ll become a more experienced Python user and should be able to produce the following solution that is cleaner and more Pythonic:</p>
  <pre class="programlisting">for num_pos, num in enumerate(prime_numbers, start=1):
    print(f"Prime Number #{num_pos}: {num}")</pre>

  <p class="body"><a class="calibre" id="pgfId-1005085"></a>The above solution involves three techniques: tuple unpacking to obtain <span class="fm-code-in-text">num_pos</span> and <span class="fm-code-in-text">num</span> (section 4.4), creating the <span class="fm-code-in-text">enumerate</span> object (section 5.3), and formatting the output using f-strings (section 2.1). I’m not going to expand the discussion of these techniques here since they’ll be covered in their respective sections. Nevertheless, this example is simply showing you what this book is all about—<i class="fm-italics">how to use a variety of techniques to produce Pythonic solutions</i>.</p>

  <p class="body"><a class="calibre" id="pgfId-1005086"></a>Besides these techniques, you’ll learn and apply advanced function concepts, such as decorators and closures, for example. When you define classes, you’ll know how to make them work together to minimize the code and reduce the potential for bugs. When your program is done, you’ll know how to log and test your code to make it production-ready.</p>

  <p class="body"><a class="calibre" id="pgfId-1000148"></a>This book is all about synthesizing domain-independent Python knowledge. You’ll not only learn pragmatic advanced features, but also basic Python features and fundamental computer programming concepts where applicable. The key term here is <i class="fm-italics">synthesizing,</i> as discussed in <a class="calibre" id="marker-1000686"></a>section 1.4.2.</p>

  <h3 class="fm-head1" id="sigil_toc_id_19"><a id="pgfId-1000174"></a>1.4.2 Solving problems through synthesis</h3>

  <p class="body"><a class="calibre" id="pgfId-1000183"></a>A common dilemma that beginners run into is that they seem to know a variety of techniques, but don’t know how and when to use them to solve problems. For each technique we discuss in this book, we’ll show you how it works independently, and we’ll also show you how it fits with other techniques. We hope that you’ll start to see how all the different pieces can be composed into an infinite number of new programs.</p>

  <p class="body"><a class="calibre" id="pgfId-1000221"></a>As a fundamental note on learning and synthesizing various techniques, you should expect that learning to code isn’t a linear path. After all, Python’s technical features are closely interrelated. Although you’ll focus on learning intermediate and advanced Python techniques, they can’t be isolated completely from basic topics. Instead, you’ll notice that I’ll frequently make remarks on basic techniques or intentionally reiterate techniques that I’ve already covered.</p>

  <h3 class="fm-head1" id="sigil_toc_id_20"><a id="pgfId-1000355"></a>1.4.3 Learning skills in context</h3>

  <p class="body"><a class="calibre" id="pgfId-1000364"></a>As we mentioned earlier, this book focuses on learning skills that are built on domain-independent Python knowledge. Being domain-independent means that you can apply the skills covered in this book to any domain where you’d like to use Python. It’s almost impossible to learn anything without an example, however. We’ll show most techniques in this book by using an ongoing project to provide a consistent context within which to discuss specific skills. If you’re familiar with a particular skill, you can skip to the section’s Discussion part, in which I’ll discuss some key aspects of the covered skills.</p>

  <p class="body"><a class="calibre" id="pgfId-1000404"></a>As a heads-up, the generic project is a task-management web app. In the application, you can manage tasks, including adding, editing, and removing tasks—everything that will be implemented with pure Python, such as data models, functions, classes, and anything else you can think of that an application may have. Moving forward, the important thing to note is that the goal is not to get a perfect, shiny application from this book. Instead, you want to learn all the essential Python techniques in the process of creating this web app so you can apply your domain-independent knowledge to projects in your own jobs.</p>

  <h2 class="fm-head" id="sigil_toc_id_21"><a id="pgfId-1000441"></a>Summary</h2>

  <ul class="calibre11">
    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000450"></a>It’s critical for you to build a pragmatic learning strategy. By focusing on learning the domain-independent features of Python, you’ll get yourself ready for any Python-related job role.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000462"></a>Python is a general-purpose, open source programming language that fosters a tremendous community of developers who make and share Python packages.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000481"></a>Python is competitive in many domains, including web development, data science, and ML. Each domain has specific Python frameworks and packages that you can use.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000495"></a>Python has its limitations. If you consider developing mobile apps or low-level device drivers, you should use Swift, Kotlin, Java, C, C++, Rust, or any other applicable language.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000511"></a>I make a distinction between <i class="fm-italics">domain-independent</i> Python knowledge and <i class="fm-italics">domain-dependent</i> Python knowledge. This book focuses on teaching domain-independent Python knowledge.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000531"></a>Learning to code is not a linear path. Although you’ll learn advanced features in this book, I’ll frequently mention basic ones. Also, you’ll encounter some difficult topics, which will create an upward spiral learning path.</p>
    </li>

    <li class="fm-list-bullet">
      <p class="list"><a class="calibre" id="pgfId-1000559"></a>The essential recipe for learning Python or any programming language is synthesizing individual technical skills to form a comprehensive skill set. Through the synthesis process, you’ll learn the language in a pragmatic way, knowing what works for the problem that you’re addressing.</p>
    </li>
  </ul>
</body>
</html>
