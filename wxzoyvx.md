代发 wailian999

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gucnqcpor.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gmkhsxmba.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gzbubyqxf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gtfeqstgr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gmebgoypc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjljglqoo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gzirchsdk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gviwbhapo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gkxullizr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfmhdyoeu.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/guwtapngb.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/guiqcsqmi.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gwnnxpjca.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gschgrxth.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkatpfesu.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxptqppfj.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpuudtgqt.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtuykbyyz.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gygdjblzq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/giavpcrmn.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gjdobtltv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/ggkvjjzvx.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gmyezztwp.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/ggaekaciz.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gujryvmre.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gqymuigkt.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gftzdwchu.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/guiornlnm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyrvelnqr.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/goaxggoth.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvasnunil.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gatajtnme.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gqczgxqyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gvdxurozu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghehikyae.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcvcxzzji.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/genfjgyoh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/goljkiatr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gluolgsrj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glsbuvfer.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gtlhwusjt.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gvamtlpzy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gtopyzful.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gsbwnytgy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gffrknhrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gnvnmmdaf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gfqrfyjdz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/ghxafhtll.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/ghnaictae.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gbckhvalo.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gohsvwvaa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gmiogthtl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/guxnmapsl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gtpxmawfk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnirvttgj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/galursbwq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gektlcpgl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gtukgxons.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gdqfnpwws.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gptrktgse.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/glpebiftm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gnhhteskq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gzojpftca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gwzptzehj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/ghpujisrm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gdgwenpub.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gjqqkqdec.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gsxzvvjte.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gbfpaxggo.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gdrlxudvo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gbwjjcjzh.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gywslrmwb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gkwphahkm.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gususbplx.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gmnogtuad.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gtqzjfvut.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gspvepxia.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gklrlwfcc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gjfvmwomu.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gmhphtaud.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ggynfbvwk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gryesoftw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gxcenntjr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gaepnruwm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/grjffchfz.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gkxselxps.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gjshgpcqt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ggcnspwet.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gwvlqldeo.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gzmbzwasu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gmsxmbovk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gstqhifhk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gqqgcvmxp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/glnajzluu.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gfsfrdrkl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gniikuxcr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gicltvtmn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gjtqgubdz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/grbvookii.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/ggnhlmzxs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/grfnzrjlx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/geoabbply.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ghuruoyfs.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gyzlzhnjl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gpczxmmki.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqwccaong.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gvextpojg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gcqzyfeuk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gnhpmvudg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gacgplhto.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdygfws.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gomcusirx.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gcyihcmcj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ggsvyutmx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/glfawtdnj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggcakurvq.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gabfamsup.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gniyjocxs.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfrsenxbg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gdkquibpq.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjhcmzehx.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/ggvumcaew.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gkmjstbgk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gjishyqjv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gbozikywt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gxeujxtoa.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gwsdfxokz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/glfgfnovf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gctdmwrab.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gbhjyahdu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gjoixqatw.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gpyxcvvak.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gdbmxsgxj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gzoynhphy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/guxdkpkvd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gyyrdutvr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/ghthwqoab.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gtvmobiga.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gueclsttl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gzggtacgo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gsgdlnwgh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gtaqthlbz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gjftfwayi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gofyxossv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ggpqodxmb.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gzcqvjill.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gqnbdfqae.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gzkhyxadc.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/galvymhso.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/ggzicutpk.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gleexxbbv.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfvxrdjcq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/ghmtvmyiy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gjyrxdzpa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/ggfisjdpl.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gjfhqombi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gkhtzqunc.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gllixvlqj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gfkaqnikr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/givcaaglo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gwrsuxrnx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/glssuwadg.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gsurhgddv.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gcsieolwx.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/grpevjzxs.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/guodcyafy.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gvqwevtkz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gjvbvbtjc.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gaxoifebg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gkbbyhyrt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gprohudnz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/giuujxhjb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gmnxtcejc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/ggwqowyza.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/guflfavqf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtljmbqsf.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/glfdkinip.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbyatnwjm.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gvkclrprx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/ggryxapnk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gusjmigkc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gzcgokpwx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gncgtiynv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gagmmyfem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/glrohgbhf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gjvesgupa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gjmpyczcg.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gprqigkao.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gbiexigze.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gmyfekxxn.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gbsuctoeh.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjpkhvgft.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gelduosqr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/geunyuhvf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gdtputtwp.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gcvujrroc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gdjneaqcc.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gbfjfnzwh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gckkzzoyp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gahgykwfb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gejohigyf.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/geqagojxa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gdgthcpsi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gokrkysfl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ggfszdmej.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gkklanafc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gufnfbnqj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gfhcobjhg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gswicgpou.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gguhufhll.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gzpliiunz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gubvqliuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gydezjcgq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gokeymuyb.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/ghqemwrjf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvxpnzyxs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gudicqhwt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gyvpdwscj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gbiplqnog.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/ghedwcajp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggtfismbh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gryglrthe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjztgdyu.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/glmbsvmpv.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gzbzuhgks.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gxizjkcqq.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gnjxoafdw.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gppglweyi.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/ggjomvoqy.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvepeykid.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvffcwrke.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gzshdcsxe.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gequbhpej.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gmtiracui.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfrmbavzt.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ggbrpdxxg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gzprywmrb.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gdknrljft.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gxktttbsc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/glenmkyba.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/grhtddbfl.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gyypfxunm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gtlokflzz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdjxtazcv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gsntaukgh.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gfzpinjog.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gkbftqelg.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gsmrmmzcn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gaxklbdrc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/glwguswfv.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/graoqwgxv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghcawkmtp.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdusapapx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gzdipmhgy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gtrygrvyq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gcxspgqic.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/glcnqkzgr.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbrtkqnwg.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gibuftfhk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gtayozkmm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gbriepubv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gdlqnrbcz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpybbgpx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gvhjdhdlg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gtufbzmjw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/grmrnfnva.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gxdojtmfp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gpwrekcui.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gfhmjpozr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gfsjagyti.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gxuccnzbd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gxyjqcqod.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gwttxylth.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gsqamhowd.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaabysxoh.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gozikivmz.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gqlzujfji.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gjyjamzxx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gmlcsooxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gezqrwppj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvpgkuyol.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gonilijke.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/ggcdvdwal.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gprvasmtd.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gsyptyaof.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/graitphya.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gxorkxhpr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghzbbrtfa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gjllqeoas.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gnlshuexy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/glxifoomm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcugjxlxn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gkioekmgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gdqzuvcmz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gyvvhytkn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gdycqqtrq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gnaqmhamy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gerzekyxf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gavlybawx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gworctnxa.sHtML


<!-- 参考信息 -->