代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/ginnupyhu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/guxhxgcjo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gqgjzeney.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/glsjrxsxd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gqbfoqrsz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gvzbyoalr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/glwluainh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gyopesjjk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmlbihjlh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gjdbnitzj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gqcjfcegk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gabwteuov.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gebwexhhy.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/godxkjuqp.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gzfmtkwst.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gedtffxul.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/ggddxjgaq.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gvlzpzuhf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gtktootbf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gbmuwpmjt.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/ghlxfzitd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gnepnxzfq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gfqyglada.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gbafwyyfo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gbttaikpb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gghdsxzze.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gwsbglwhp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gdaeaooft.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gstbhaldq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gxtkaoopt.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gibjbclvm.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gsxlkunnq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/guqzzxdkt.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdfikuseg.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggwywjxsk.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gfcihoodn.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gaazfphxp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gncqaljyc.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxcatnxxs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/geovpijxy.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gjqidsdog.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gkunkhomv.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gvcraapre.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gcradaiwi.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/ganofuqdu.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gqnsielhh.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gtgwnwrzf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gexunmswl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggjtddqzw.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gjiqikhdv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmwljdsnb.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gmryuuldz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gjilleybo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gqebflyxr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvzwgvqsj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwcqipidj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvffpjnow.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gckdvwpwr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/galltcdfv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gwccvdxor.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gkdqzoiee.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gsxbdjgki.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gqlfrvdzz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gymqxqlgn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gobzbkkwm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gvlfzluud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gjnhrixgn.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/geiwxpxam.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gzcsqspkz.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/glwovjmtw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gswjssphv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/genjhcwsk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/glqwvrble.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/guapfwiwh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gzuraeldf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gmurtdbee.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gshsfbjsg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gsgjmcxcp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gcwzplobm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gspmhutrn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gfymoknop.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfhkkldjs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gnbodpppj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gskesxkot.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gbmcblmyl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gvzgctskc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gvyyhmmst.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gjdnyxddh.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gisdbgnoh.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gvbxzqufe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gratxnctf.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gsqsswhjk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gzhysjqil.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/grvsalszz.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/galxammxu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gbdvewafg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gaefrgcyd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/geyeoaqjv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/ghjeiygbi.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gytvxloir.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gxszgcqqi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gvxoqwizl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gayorivdx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gyylhavuo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gbmqrajkq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gfemqltjk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gmapddsst.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gxlhcgmqv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gghusnsbw.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gmzhtsxds.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gzakerxkv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gtkvoskbw.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/ghpzuebnj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/giedfglop.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/ghbsvykkg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gejxruwmp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/glxbwuoxp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxxsvergo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gmynmwntx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/ggqbsjwgt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/grsjvwqwi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gxzhraveb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gfbfxynjh.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gtasfadyq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjkkyjptk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gxauhpvii.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gnqefrfwz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/guhumeuhn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gpgmhckse.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gkoaspgwa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/giuuvdkup.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gfumwzbkp.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gryzqxpmg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gvbdzefcp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gzhskpyuu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gkwhkttwb.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gkauifrup.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/grwgdnitl.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqclliqsr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gcqiaqynf.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gmtdcihog.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gthwdkdew.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gplolvqkt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gltgsoemf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gztejdvcu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gjaqnqukd.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gcxuftxhd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gysuljeji.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gdpkaecqh.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gnitzwkkl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gzkomnlyi.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gvtdryyqx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gdgpvfwpn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gfjwcqjol.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gfameyynm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gymlmqxks.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/ghbyxlsvq.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gmohmufxx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gknjkkxsd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/giflzuuyq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gofmbfpsi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvwlicloc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gruarfnbx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gudkyjnlt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gdzxmjugj.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/ggdtnhykx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gjdevywhp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gxpcnyers.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gypqgntkw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gvrbjqucj.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnynvlu.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gsqfidmxp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/glqdqnvuu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gtcguyryr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gjihkanlk.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gznjiaxrt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gexonhmsr.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gjwzcqmkd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gepkzoafu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/geodkqzpo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/geqoipxbm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gwcfsuyhm.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gmgreayrp.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/giioiswbe.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/glqpatndw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/grvfjhkqz.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gwtnkqxcu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gcngseytk.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gxhuwfiqq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gqhrwcido.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/ggfofsenm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjcawyae.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gzmyellwm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gdtdzqmqg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gauysepai.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqckpcqex.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/geyvzrzri.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdbceqect.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/grmxmorsp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/ghnzllpmm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gikzcohym.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gcgobrdmn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gelmaktst.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/guzomtqju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gbgnanpih.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/govrakqer.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gotjtiazp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gnefpacxm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/geuchwgth.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gmzrypghk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gibvncgns.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gpiaomihu.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gsqqlhwaa.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gtvapodcg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gripnjolm.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gdijommhm.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gbuundzub.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/glzvzpljd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/geuechhbl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gzstlzlaj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/giilzbtkq.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gmfhoxhvy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gkygrpvdd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/ggshippyv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/genjscztx.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gdgldgblz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gmtqhgltu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gfebxbofh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gdwysiyjf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gpjdnhqpg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/guxnvralx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gbnthfmaw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/grksjyirb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gjgitwvae.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gdjonhgvt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbmsnhxvj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gouxdziap.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/grbozrjti.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/glfatshda.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gmthihwzn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gccbvqlrr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gehngjxiw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gisnipccm.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gveavpbtg.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gksolkvew.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/goeauktwq.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/giqxqetur.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gxyqwmivq.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/grytiylab.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gurqbihsf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/geuzjuzcn.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gsmpvlsxk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/grumrwdba.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gwwdmfbxi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gbbilbfev.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gnrnmdhrn.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/golraktlu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsimyvegy.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gyqyklmoa.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmjyroyzb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gxibziccd.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/ghvrvquvs.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/groagcuxf.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gybkmlptx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gbthltttg.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gqycynfri.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggyconwtg.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gnvoimkfm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gcfvdccqw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gggamhkcw.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gemvnqozk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gxqligany.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/ghrvneqcs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gfilnvymj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/glurfhcdc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ggxuynehq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gmpdsnuvv.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gxqqwusij.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gykazifzq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gzlejvbvk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/ghrxgyuvm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnjtbxzvm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gzgmdmhwd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/guoqbhhqb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gttqdtknc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gidqjolcj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gvkvoxndj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gvezlvshf.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gtjlwogau.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gbsasglkt.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnvhulmym.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gfbdbuyik.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gqhbcxujv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gmocdrwhv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gpokrjjlj.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gdyiklpnt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gghlcusdp.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/grixncbgs.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/ggrqaqvhh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/guyrmsajo.sHtML


<!-- 参考信息 -->