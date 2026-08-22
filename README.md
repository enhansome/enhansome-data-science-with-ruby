<img src="header.png" align="center">

\[[RubyNLP](https://github.com/arbox/nlp-with-ruby) ⭐ 1,076 | 🐛 7 | 🌐 Ruby | 📅 2023-06-27 |
[RubyML](https://github.com/arbox/machine-learning-with-ruby) ⭐ 2,221 | 🐛 6 | 🌐 Ruby | 📅 2024-12-26 |
[RubyInterop](https://github.com/arbox/ruby-interoperability) ⭐ 41 | 🐛 1 | 🌐 Ruby | 📅 2020-11-16]

# Awesome Data Science with Ruby with stars

> Links and Resources for Data Processing and Analysis in Ruby

[Data Science](https://en.wikipedia.org/wiki/Data_science) is a new
"sexy" buzzword without specific meaning but often used to substitute
Statistics, Scientific Computing, Text and Data Mining and
Visualization, Machine Learning, Data Processing and Warehousing as
well as Retrieval Algorithms of any kind.

This curated list comprises [*awesome*][awesome] tutorials, libraries,
information sources about various Data Science applications using
the [Ruby programming language][ruby].

A lot of useful resources on this list come from the development by
[The Ruby Science Foundation][sciruby], our [contributors][contributors] and
our own day to day work on various data intensive applications.
Read [why](#wait-but-why) this list is awesome.

:sparkles: Every [contribution](contributing.md) is welcome!
Add links through pull requests or create an issue to start a discussion.

Follow us on [Twitter](https://twitter.com/NonWebRuby)
and please spread the word using the `#RubyDataScience` hash tag!

<!-- nodoc -->

## Contents

<!-- toc -->

* [Ruby vs. Python vs. Julia vs. R](#ruby-vs-python-vs-julia-vs-r)
* [Standing on the shoulders of giants](#standing-on-the-shoulders-of-giants)
* [Data Manipulation](#data-manipulation)
* [Distributed Computing](#distributed-computing)
* [Data Structures](#data-structures)
* [Data sets](#data-sets)
* [Statistics](#statistics)
* [Numeric and Symbolic Computation](#numeric-and-symbolic-computation)
* [Visualization](#visualization)
* [Interactive Computing](#interactive-computing)
* [Input and Output](#input-and-output)
  * [General formats](#general-formats)
  * [Database Adapters](#database-adapters)
  * [Domain specific formats](#domain-specific-formats)
* [Provisioning Infrastructure](#provisioning-infrastructure)
* [Machine Learning](#machine-learning)
* [Articles, Posts, Talks, and Presentations](#articles-posts-talks-and-presentations)
* [Related resources](#related-resources)
* [Wait but why?](#wait-but-why)
* [License](#license)

<!-- tocstop -->

<!-- doc -->

## Ruby vs. Python vs. Julia vs. R

| Ruby         | Python | Julia | R |
| ------------ | ------ | ----- | - |
| Daru / Rover | Pandas |       |   |
| NArray       | NumPy  |       |   |

## Standing on the shoulders of giants

Ruby is (for now) not a Data Science centric language with a very large established library.
Leveraging libraries from R, Python, and Julia helps Ruby to solve your tasks!

<!--- TODO: Add the talk by @mrkn --->

* [pycall](https://github.com/mrkn/pycall.rb) ⭐ 1,116 | 🐛 52 | 🌐 C | 📅 2026-08-21 — Bridge into the Python world.
* [rserve-client](https://github.com/clbustos/Rserve-Ruby-client) ⭐ 130 | 🐛 13 | 🌐 Ruby | 📅 2024-05-03 —
  Ruby connector for [Rserve](http://www.rforge.net/Rserve/), R's binary server.

## Data Manipulation

* [kiba](https://github.com/thbar/kiba/) ⭐ 1,775 | 🐛 0 | 🌐 Ruby | 📅 2026-01-10 —
  lightweight Ruby ETL (Extract-Transform-Load) framework.
* [jongleur](https://gitlab.com/RedFred7/Jongleur) —
  Workflow manager using DAG definitions to execute ETL tasks.

## Distributed Computing

* [ruby-spark](https://github.com/ondra-m/ruby-spark) ⭐ 226 | 🐛 23 | 🌐 Ruby | 📅 2017-08-31 —
  Ruby Interface to [Apache Spark](https://spark.apache.org/) 1.x.x.
* [jruby-spark](https://github.com/chyh1990/jruby-spark) ⭐ 7 | 🐛 2 | 🌐 Java | 📅 2016-04-27 —
  JRuby based bindings for [Apache Spark](https://spark.apache.org/).

## Data Structures

* [spreadsheet](https://github.com/zdavatz/spreadsheet) ⭐ 1,150 | 🐛 13 | 🌐 Ruby | 📅 2026-04-21 —
  manipulation library for MS Excel spreadsheets.
* [daru](https://github.com/SciRuby/daru) ⭐ 1,061 | 🐛 92 | 🌐 Ruby | 📅 2023-08-15 —
  Data Frame and Vector structures with comprehensive manipulating and visualization methods.
* [nmatrix](https://github.com/sciruby/nmatrix) ⭐ 478 | 🐛 76 | 🌐 C++ | 📅 2024-04-24 —
  dense and sparse linear algebra library for Ruby via [SciRuby](http://sciruby.com/).
* [numo-narray](https://github.com/ruby-numo/numo-narray) ⭐ 469 | 🐛 63 | 🌐 C | 📅 2025-06-06 —
  n-dimensional Numerical Array for Ruby.
* [Rover](https://github.com/ankane/rover) ⭐ 387 | 🐛 2 | 🌐 Ruby | 📅 2026-08-15 —
  Data Frame and Vector structures with comprehensive manipulating and visualization methods.
* [kdtree](https://github.com/gurgeous/kdtree) ⭐ 126 | 🐛 0 | 🌐 C | 📅 2025-05-01 —
  blazingly fast native 2d k-d tree.
* [cumo](https://github.com/sonots/cumo) ⭐ 99 | 🐛 5 | 🌐 C | 📅 2026-08-22 —
  CUDA-aware numerical Array library with [NArray](https://github.com/ruby-numo/numo-narray) ⭐ 469 | 🐛 63 | 🌐 C | 📅 2025-06-06 similar interface.
* [mdarray](https://github.com/rbotafogo/mdarray) ⭐ 36 | 🐛 3 | 🌐 Ruby | 📅 2017-03-31 —
  Array structure for `JRuby`.
* [networkx](https://github.com/SciRuby/networkx.rb) ⭐ 32 | 🐛 2 | 🌐 Ruby | 📅 2023-02-23 —
  Ruby based [NetworkX](https://networkx.github.io/) clone that handles various
  usecases of the Graph Data Structure.

## Data sets

* [red-datasets](https://github.com/red-data-tools/red-datasets) ⭐ 33 | 🐛 75 | 🌐 Ruby | 📅 2026-07-08 —
  Growing collection of publicly available data sets such as CIFAR-10, Iris, MNIST etc.
* [rdatasets](https://github.com/kojix2/rdatasets) ⚠️ Archived —
  Data sets available in R via [Rdatasets](https://github.com/vincentarelbundock/Rdatasets) ⭐ 414 | 🐛 0 | 🌐 HTML | 📅 2026-06-15.

## Statistics

* [enumerable-statistics](https://github.com/mrkn/enumerable-statistics) ⭐ 130 | 🐛 8 | 🌐 Ruby | 📅 2026-06-22 —
  fast implementation of descriptive statistics for the `Enumerable` module.
* [descriptive-statistics](https://github.com/jtescher/descriptive-statistics) ⚠️ Archived —
  descriptive extensions for the `Enumerable` module or standalone usage.
* [statsample](https://github.com/sciruby/statsample) ⭐ 100 | 🐛 21 | 🌐 Ruby | 📅 2017-11-21 —
  basic and advanced statistics for Ruby. <sup>\[[dep: GLS](#gls)]</sup>
* [statistics2](https://github.com/abscondment/statistics2) ⭐ 62 | 🐛 5 | 🌐 Ruby | 📅 2024-04-03 —
  Normal, Chi-square, t- and F- probability distributions for Ruby.
* [fast\_statistics](https://github.com/Martin-Nyaga/fast_statistics) ⭐ 59 | 🐛 3 | 🌐 Ruby | 📅 2023-10-20 —
  fast computation of descriptive statistics (min, max, mean, median, 1st and 3rd quartiles, population standard deviation) for a multivariate dataset.
* [distribution](https://github.com/sciruby/distribution) ⭐ 51 | 🐛 19 | 🌐 Ruby | 📅 2020-07-05 —
  probabilistic distributions and descriptive measures for them.
* [rb-gsl](https://github.com/blackwinter/rb-gsl) ⚠️ Archived —
  Ruby interface to the GNU Scientific Library. <sup>\[[dep: GLS](#gls)]</sup>
* [pca](https://github.com/gbuesing/pca) ⭐ 27 | 🐛 1 | 🌐 Ruby | 📅 2017-01-05 —
  Principal Component Analysis (PCA) in Ruby.
* [simple\_stats](https://github.com/brianhempel/simple_stats) ⭐ 25 | 🐛 1 | 🌐 Ruby | 📅 2013-12-16 —
  `Enumerable` patches for descriptive statistics.
* [statsample-glm](https://github.com/sciruby/statsample-glm) ⭐ 24 | 🐛 13 | 🌐 Ruby | 📅 2019-01-24 —
  extension of `statsample` by Generalized Linear Models.
* [statsample-timeseries](https://github.com/sciruby/statsample-timeseries) ⭐ 14 | 🐛 3 | 🌐 Ruby | 📅 2017-08-06 —
  extension of `statsample` by Time Series estimators.
* [statsample-bivariate-extension](https://github.com/sciruby/statsample-bivariate-extension) ⭐ 2 | 🐛 2 | 🌐 Ruby | 📅 2017-08-22 —
  extension of `statsample` by Bivariate Correlations.

## Numeric and Symbolic Computation

* [numo-linalg](https://github.com/ruby-numo/numo-linalg) ⭐ 44 | 🐛 11 | 🌐 Ruby | 📅 2025-08-25 —
  linear algebraic operations for NArray.
* [symengine](https://github.com/symengine/symengine.rb) ⭐ 29 | 🐛 19 | 🌐 C | 📅 2019-03-14 —
  Symbolic Computation with [SymEngine](https://github.com/symengine/symengine) ⭐ 1,401 | 🐛 258 | 🌐 C++ | 📅 2026-08-20.
* [numo-gsl](https://github.com/ruby-numo/numo-gsl) ⭐ 23 | 🐛 4 | 🌐 Ruby | 📅 2024-06-07 —
  Math and Statistics for NArray using GSL.<sup>\[[dep: GSL](#gsl)]</sup>
* [numo-ffte](https://github.com/ruby-numo/numo-ffte) ⭐ 5 | 🐛 0 | 🌐 C | 📅 2018-01-18 —
  Fast Fourier Transformation for NArray using the FFTE package.<sup>\[[FFTE](#ffte)]</sup>

## Visualization

Comprehensive tools for Data Visualization.

* [chartkick](https://github.com/ankane/chartkick) ⭐ 6,528 | 🐛 7 | 🌐 Ruby | 📅 2026-08-15 —
  Create beautiful JavaScript charts with one line of Ruby.
* [Gruff](https://github.com/topfunky/gruff) ⭐ 1,398 | 🐛 14 | 🌐 Ruby | 📅 2026-07-28 —
  graphing library built on top of [rmagick](https://github.com/rmagick/rmagick) ⭐ 731 | 🐛 4 | 🌐 C++ | 📅 2026-08-19.
* [ruby-graphviz](https://github.com/glejeune/Ruby-Graphviz) ⭐ 615 | 🐛 40 | 🌐 Ruby | 📅 2025-03-16 <sup>\[[dep: Graphviz](#graphviz)]</sup>
* [Vega](https://github.com/ankane/vega) ⭐ 302 | 🐛 0 | 🌐 Ruby | 📅 2026-05-11 —
  [Vega](https://vega.github.io/vega/) and [Vega-lite](https://vega.github.io/vega-lite/)
  based visualization for Rover.
* <https://github.com/zverok/worldize> ⭐ 262 | 🐛 1 | 🌐 Ruby | 📅 2018-08-20
* [nyaplot](https://github.com/domitry/nyaplot) ⭐ 222 | 🐛 38 | 🌐 Ruby | 📅 2016-06-24
* [gnuplot](https://github.com/rdp/ruby_gnuplot/tree/master) ⭐ 219 | 🐛 17 | 🌐 Ruby | 📅 2019-12-20 <sup>\[[dep: gnuplot](#gnuplot)]</sup>
* [mathematical](https://github.com/gjtorikian/mathematical) ⭐ 170 | 🐛 7 | 🌐 Ruby | 📅 2026-06-19 —
  PNG and MathML renderings for your equations.
* [daru-view](https://github.com/sciruby/daru-view) ⭐ 98 | 🐛 48 | 🌐 Jupyter Notebook | 📅 2022-08-28 —
  daru-view is interactive plotting gem for web application
  (any Ruby web application framework like Rails/Sinatra/Nanoc/Hanami) & IRuby notebook.
  It is a plugin gem for daru.
* [matplotlib](https://github.com/mrkn/matplotlib.rb) ⭐ 97 | 🐛 8 | 🌐 Ruby | 📅 2023-03-16 —
  Ruby based wrapper around [matplotlib](https://matplotlib.org/). <sup>\[[dep: matplotlib](#matplotlib)]</sup>
* [ruby-gr](https://github.com/red-data-tools/GR.rb) ⭐ 97 | 🐛 9 | 🌐 Ruby | 📅 2026-06-23 —
  Ruby interface to [GR](https://gr-framework.org/), a framework for visualisation applications. <sup>\[[dep: GR](#gr)]</sup>
* [Rubyplot](https://github.com/SciRuby/rubyplot) ⭐ 64 | 🐛 24 | 🌐 Jupyter Notebook | 📅 2022-06-18 —
  graphing library built on top of [GR](https://gr-framework.org).
* [numo-gnuplot](https://github.com/ruby-numo/numo-gnuplot) ⭐ 54 | 🐛 5 | 🌐 Ruby | 📅 2022-10-08 —
  gnuplot interface for the Numo package.
* <https://github.com/zuhao/plotrb> ⚠️ Archived
* [gnuplotrb](https://github.com/SciRuby/gnuplotrb) ⭐ 29 | 🐛 8 | 🌐 Jupyter Notebook | 📅 2020-04-06
* [Nyaplotjs](https://github.com/domitry/Nyaplotjs) ⭐ 21 | 🐛 3 | 🌐 JavaScript | 📅 2015-12-29
* [iruby-chartkick](https://github.com/Absolventa/iruby-chartkick) ⭐ 18 | 🐛 2 | 🌐 Ruby | 📅 2026-06-13 —
  Use [chartkick](https://github.com/ankane/chartkick) ⭐ 6,528 | 🐛 7 | 🌐 Ruby | 📅 2026-08-15 within IRuby-backed jupyter notebooks
* <https://github.com/brasten/scruffy> ⭐ 15 | 🐛 3 | 🌐 Ruby | 📅 2011-01-01
* [benchmark-plot](https://github.com/v0dro/benchmark-plot) ⭐ 7 | 🐛 0 | 🌐 Ruby | 📅 2016-07-10
* [daru-plotly](https://github.com/genya0407/daru-plotly) ⭐ 3 | 🐛 2 | 🌐 Ruby | 📅 2017-05-22 —
  [Plotly](https://plot.ly/) based visualization for Daru.
* <https://github.com/masa16/ruby-mathgl> ⭐ 3 | 🐛 0 | 🌐 C++ | 📅 2016-03-20

## Interactive Computing

* [iruby](https://github.com/sciruby/iruby) ⭐ 923 | 🐛 49 | 🌐 Ruby | 📅 2026-06-30 —
  Ruby kernel for [Jupyter](https://jupyter.org/).
* [jupyter\_on\_rails](https://github.com/Yuki-Inoue/jupyter_on_rails/) ⭐ 88 | 🐛 11 | 🌐 Ruby | 📅 2024-03-19 —
  Another integration library for IRuby and Rails.
* [iruby-rails](https://github.com/mrkn/iruby-rails) ⭐ 22 | 🐛 1 | 🌐 Ruby | 📅 2019-02-17 —
  Integration library for IRuby and Rails.

## Input and Output

### General formats

* [oj](https://github.com/ohler55/oj) ⭐ 3,225 | 🐛 14 | 🌐 C | 📅 2026-08-13 —
  High-speed JSON parser.
* [ox](https://github.com/ohler55/ox) ⭐ 913 | 🐛 3 | 🌐 C | 📅 2026-08-08 —
  Optimized for speed XML parser and object marshaller.
* <https://github.com/fiksu/rcsv>
* Markdown
* Nokogiri
* CSV

### Database Adapters

* pg
* Mongo
* MySQL

### Domain specific formats

* [bolognese](https://github.com/datacite/bolognese) ⭐ 52 | 🐛 24 | 🌐 Ruby | 📅 2026-07-23 —
  conversion tool for citation formats like BibTeX, RIS, or Crossref XML.
* [inih](https://github.com/woodruffw/ruby-inih) ⭐ 7 | 🐛 0 | 🌐 C | 📅 2021-04-29 — fast C based INI parser for Ruby.
* BibTeX

## Provisioning Infrastructure

* <https://github.com/k1LoW/awspec> ⭐ 1,177 | 🐛 40 | 🌐 Ruby | 📅 2026-08-16
* <https://github.com/mrkn/gpu-instance> ⭐ 0 | 🐛 0 | 🌐 Ruby | 📅 2016-05-15
* <https://github.com/mrkn/computing_node> ⭐ 0 | 🐛 5 | 🌐 Ruby | 📅 2015-02-17

## Machine Learning

Please look at our extensive [Awesome ML with Ruby][ml-with-ruby] list.

## Articles, Posts, Talks, and Presentations

* 2019
  * *Parallelising ETL workflows with the Jongleur gem* by [Fred Heath](https://github.com/RedFred7) <sup>\[[post](http://bootstrap.me.uk/gems/2019/01/06/jongleur-etl.html)]</sup>
* 2018
* 2017
  * *Progress of Ruby-Numo: Numerical Computing for Ruby* by [Masahiro Tanaka](https://github.com/masa16) <sup>\[[slides](https://speakerdeck.com/masa16tanaka/progress-of-ruby-numo-numerical-computing-for-ruby)]</sup>
  * *Chartkick: data visualization made easy with Ruby* by [Govind Unnikrishnan](https://twitter.com/govind_k_u) <sup>\[[post](https://blog.redpanthers.co/chartkick-data-visualization-easy-ruby/)]</sup>
  * *Development of Data Science Ecosystem for Ruby* by [Kenta Murata](https://twitter.com/mrkn) <sup>\[[slides](https://speakerdeck.com/mrkn/development-of-data-science-ecosystem-for-ruby) |
    [video](https://www.youtube.com/watch?v=U9GdgZowmGY) |
    [page](https://rubykaigi.org/2017/presentations/mrkn.html)]</sup>
* 2016
  * *Scientific Computation and Data Visualization with Ruby* by [Sameer Deshmukh](https://twitter.com/v0dro) <sup>\[[slides](https://www.slideshare.net/SrijanOne/webinar-scientific-computation-and-data-visualization-with-ruby) |
    [video](https://www.youtube.com/watch?v=5970kC6MfBE)]</sup>
* 2015
* 2014
* 2013
  * *Seeing the Big Picture: Quick and Dirty Data Visualization with Ruby* by [Aja Hammerly](https://twitter.com/the_thagomizer) <sup>\[[video](https://www.youtube.com/watch?v=dWPRLCU39AU) |
    [slides](http://www.thagomizer.com/files/dataviz_windy_city_13.pdf) |
    [code](https://github.com/thagomizer/data_visualization_talk) ⭐ 3 | 🐛 0 | 🌐 Ruby | 📅 2013-09-20]</sup>
* 2012
* 2011
* 2010
  * *NArray and scientific computing with Ruby* by [Masahiro Tanaka](https://twitter.com/masa16tanaka) <sup>\[[video](https://vimeo.com/14823720) |
    [slides](https://www.slideshare.net/masa16tanaka/narray-and-scientific-computing-with-ruby)]</sup>

## Community

* <https://gitter.im/red-data-tools/en>
* <https://gitter.im/red-data-tools/ja>
* <http://ruby-data.org/>
* <https://twitter.com/RubyData>
* <https://discourse.ruby-data.org/>

## Related resources

* [Awesome Big Data](https://github.com/onurakpolat/awesome-bigdata#data-visualization) ⭐ 14,538 | 🐛 3 | 📅 2026-07-31 -
  awesome curated list on all around Big Data.
* [Awesome Data Science with Python](https://github.com/r0f1/datascience) ⭐ 4,654 | 🐛 0 | 📅 2026-08-11
* [Awesome Spark](https://github.com/awesome-spark/awesome-spark) ⭐ 1,890 | 🐛 24 | 🌐 Shell | 📅 2026-02-27 —
  awesome list on Apache Spark goodies.
* <a name="symengine"></a>
  [SymEngine](https://github.com/symengine/symengine) ⭐ 1,401 | 🐛 258 | 🌐 C++ | 📅 2026-08-20
* <a name="imagemagic"></a>
  [ImageMagick](https://imagemagick.org/index.php)
* <a name="gsl"></a>
  [GSL](https://www.gnu.org/software/gsl/)
* <a name="ffte"></a>
  [FFTE](http://www.ffte.jp/)

## Wait but why?

There are a lot of software lists with tools related to the Data Science.
There are a couple of lists with Ruby related projects. There are no lists of
only working and tested software with documented scope. We'll try to make one!

What is awesome? Awesome are documented, maintained and focused tools.

Can something turn not awesome at a point? Yes! Abandoned projects with broken
dependencies aren't awesome any more! They leave this list.

## License

[![Creative Commons Zero 1.0](http://mirrors.creativecommons.org/presskit/buttons/80x15/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/) `Awesome Data Science with Ruby` by [Andrei Beliankou](https://github.com/arbox) and
[Contributors][contributors].

To the extent possible under law, the person who associated CC0 with
`Awesome Data Science with Ruby` has waived all copyright and related or neighboring rights
to `Awesome Data Science with Ruby`.

You should have received a copy of the CC0 legalcode along with this
work. If not, see <https://creativecommons.org/publicdomain/zero/1.0/>.

<!--- Links --->

[ruby]: https://www.ruby-lang.org/en/

[ml-with-ruby]: https://github.com/arbox/machine-learning-with-ruby

[awesome]: https://github.com/sindresorhus/awesome/blob/master/awesome.md

[change-pr]: https://github.com/RichardLitt/knowledge/blob/master/github/amending-a-commit-guide.md

[sciruby]: https://github.com/sciruby

[contributors]: https://github.com/arbox/data-science-with-ruby/graphs/contributors

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-22._
