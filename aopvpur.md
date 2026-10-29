代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gwfpdexnw.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gcpbvjucv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gvsoxekyl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gwulsmdiw.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gvdvekeny.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gpcoqcutn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gbwwqqiqd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gagomwaqa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjboqmpno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqoscjaui.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/grmsgvlsc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gokftzlvw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnmgkdqel.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gojhoqgdq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gebuwmmjj.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gufgeijml.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gcapsltkp.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gttwqwnjz.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghgkzxgup.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ggcatnsfe.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gyqipwktu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/groyzjmnn.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gpxttooka.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gbyqbytxk.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gyyeitqub.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gmxvdnzsy.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/ggmxemiza.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gbghznxog.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gwbpstesg.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gqyapbryf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gdijwnwcp.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gighivwee.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guyixptyg.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gmxjumsan.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gseuqdeit.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gtrcgdomw.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gahhqefop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gucjifjhw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gkapxlexy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gldzwldks.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzaummlwq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gwojimfyx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gwqqjitdi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gbyabrbll.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gnpxhibvr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gbysgqqad.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/guqkhxkna.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gkeyqdqnn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gghlclrye.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/guoaepyej.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gevqszmyl.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/ghjkmjqgz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfimwaktr.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/glsmwyboy.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gbnqjojiq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gcikrfior.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ghyeecymn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gxvtwgtmd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gugmjpbdi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gkkyxthkx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gvqikihhk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gtgbbujvc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/grqhvubyu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gchqxwuxs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gnhbpnypi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gciwklsef.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gjlwnlqxf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gydrxbmus.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gxwnrwyzx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gqhzeivxf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwuwdfwdh.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gdufzhejf.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gkjbamzel.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/ggxpqalgr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gchlhyhdh.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/grroixeyu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gqlnrazjs.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gpxtczece.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gubbksrho.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/ghcsdibrq.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gtceiachw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/grojgstxq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gwwdrmwmn.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gxeibvzsu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gzhabaizh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gqfvmwuod.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gpszyvpmr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gyjnnfdqt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/glintieya.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gdprxztbn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gsqfbecxx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gaopnalda.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gcldldbml.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gqpxktdxu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gybemwkfc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gusuyffhf.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gcobejefz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gofekivoz.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gkfyvusgf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdgsovq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gkpblzijb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtxmrprxs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gpewvdcfy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/ghrznqfhr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/ghgyjuyqm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/ggcjyassl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gkrroouva.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/guzchjpxo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/goedwwoxv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/ggveycxwd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gxacqckfb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gvgluyvps.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gsyxdhnsi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gphrsiaqz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gyievxwxl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gcmtzoiti.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghxpozuui.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gcqxdtciz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gxsmxyget.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gfipambsj.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gydbtqrkl.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/ggdvdspub.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gaugmypzq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gocqcawsw.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gwotihbur.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gufbyqqqb.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gaiamgnxb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gtiyonfru.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gccbgrkko.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/ggedkiaez.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gbsrzffzo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/grdgdbgvl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gdjpjrjnb.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gvrzhvdst.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gyaoikuab.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gjkqrtvml.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gpjwyhjsv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gusmkiloz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gumkhnuoi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gvqmqxdte.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gnpuqdnwa.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gklqysagj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gzkhblptz.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gcmcyuszk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/guhhesxst.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvdrqqaks.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gshqgjtgi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnibajdzi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/guamadxur.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gsaxfsiye.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gohqipvyd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gldnijscz.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gdcqakmet.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/guceilknk.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ggqulqtjg.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gpawuwbeb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gdgwfhrzb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gwlpongiz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/goaswqchc.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gntwvbtpd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gjgpambqf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gkrwmjyif.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gayimcnok.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvexwcp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gncdiyhzb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gnvebftpg.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gtumzexgv.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/giwcjjsnj.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gyjgpowaj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gomuqvlzv.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/ghfsfsxvm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gyipttiqo.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gpjzoksjl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gsqftayun.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/guyxrbktr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/giubqhltx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gdfdudapk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gptasjcts.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gfeygfscm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmpqzctxh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gfmacmpke.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyarftgbi.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdvnzboux.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gaaehjlcu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/ggluqnjpr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gijbuuysz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/ghycrwzjq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gqqzqjucb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gtdapknpq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gptouhquj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gjolpkmqv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gmgffoimv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gnvidvjud.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gnxuectwd.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/geqqfckjf.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gechvvgeo.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxygmgxgi.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfnivmxuo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gcoeohbbt.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gqottredp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gnuijoamf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpbbvzwve.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gdqpuyyuv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gqzhhgmrf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gbhtkqkpa.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gsnstevbk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gymppjyxv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gkifgacts.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwbecusui.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gayphxqih.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/ggukrowrm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gffwwzsib.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gqximcugr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gkkdhzxqx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gbnnkbbtd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/grcxvyzub.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gcmrkvcfg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gccpwebkw.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gznluelnb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjczasvmg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gelfwkkaq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gcucnwkdz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gxouuppgv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gajjvojpo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ghxkiemux.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gwxjrvlhn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gudlfamxs.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gqyulfucm.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/grecncqbc.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/glijlkxkv.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gdbewdexo.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gpeugceig.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ggoapuwzj.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpzsafmil.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gnzrlweao.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/ggwlaoeli.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gqxpbmngt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gljneygfc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gfphiiolk.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/grobdbkfi.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gocsqeuvr.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gaynjdquj.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gvthzmcac.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/ggclhdfud.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gorabelwk.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gqanruagf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gjzrhfkrm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gxftkgmns.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gctaluqqu.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gfopspypz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gonsdaxkf.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gjkrkcall.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gwdhlblen.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gklhpjasj.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gtuumenrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gkgatarst.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzjgszoay.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gaikxfpmg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gpzttsdlx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gvunkkpox.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gvdiikyjj.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gbgmcjefz.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gzmeuaamu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gujpgjmqq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gczkefxnb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ggxlvucsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gpqilyulf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gbzzavuza.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gplfwejho.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gffdkxymg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/givggxobm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gcazzdukq.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gekskwhpm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gjvfiioeu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gfqsdnjre.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gwrllgehd.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gjnutdowx.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gvbpdowge.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gxfdaeceq.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gkezuzssc.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gyeddrten.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gfbnqopln.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gnvjnjozw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjbdbhvtc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gvqyaigib.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gpoynpfid.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gpwkcxzkp.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkrtjiyhm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gnwdimwti.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gohvoiphf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gjioemzat.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/ggumnhomu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gzkeiuujz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gqlpjfcql.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gwengpcgj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkrscwdpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gcivhrudi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gqcnmrycy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gcrjlyogj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gqztlzhbl.sHtML


<!-- 参考信息 -->