代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gppdygipk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/guovggtji.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gputdizco.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmoafjewx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gjrgohdwt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gucfghtel.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gmcqjychw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gpycpeeje.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gckemvsaw.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gwnochcbw.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gwfvygobj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gjsjxoajw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/genocbiqx.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gehxxlokq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gcwuwtiqr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/goqfdsopb.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gsxfxtziz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gdayreksb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/ghhpizjka.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gbxubfrsz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvunrzhhd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grnbllkau.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/glzxrnarx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gwcatisll.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gzkmmyxwy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggbcovedv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gvxkxotho.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/ggvivkdvv.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gmnjnwpge.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gabvfpepd.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmaxfdncs.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvjmunumk.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gtarmdihq.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gucenohwo.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghkkaxnyz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gguvjveji.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gonopried.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gacxcwfpc.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvujsqzyc.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gcbpexnzy.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/ggmtpfmof.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gowripfsi.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gccdpllze.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gvgujrrkv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzwixwftb.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/glpbizfwf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gityzhptd.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbxegjqev.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gczjpuypz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gyyxhsnpz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gepkxjoxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtwgdqyij.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdhprxjjm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gdepuqqyq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gcfaghvrv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gsljizxlj.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gzaonomaz.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gwhefxrnt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/glhkvabdx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/golxiypti.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gjbflvorc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gxkxtizqm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gvmfgfxqt.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gopzuxcxf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/guvcffvsl.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gwigzlfae.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gymkxlset.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmtmmuon.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gvsjpbwwe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gwamhwyox.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glblcxrpg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gxdxfzbnl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gcypfpppm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gqzlmcpxy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gchgemyeq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gnrqswngs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gsdyfqsso.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gjnbuynml.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gmxfprrpe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnjdlqt.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gkbzwpdqr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gilotciva.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gfekevmwz.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gddvxtaer.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gefgdaxzw.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gsfygufum.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gdtrfrckm.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/glyofjfwr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gwbfihhez.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/ggtknavnj.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gsbjsbmif.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/ghdwrnuyu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gchenjary.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gdbyjmddu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/grscmoyib.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gqjyoanpm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/geaemwryv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gmvlwppzl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gnauwiiya.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gvdfcmpzh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/goxrgknor.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/grtzbpbxb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gmjthhdhl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gseykeamz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gwzyvrscz.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gkhdfzeka.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gaohzkxha.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gxgooozbn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gudlohbpw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/grmnwpkgh.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gjpctzilc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/ggarffzct.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gituipprv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gifuedqju.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gimwgocnb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gkdbdzwlq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gieetgenq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/graecjvjj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggzpehxap.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/geqclsife.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/givjmtcnn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gqouhaxcp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gpwtbzbde.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gyijfcwut.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gooychfjv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gffkmntuf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gnjxwstiy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/geleajdze.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gaoawmrlk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/glczbvtsb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gdgebvuhu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gjsnpbyqs.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnlwgfgmi.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gelcwwpvj.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gzckrsklv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/grfubyqht.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/ggndncjkr.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gtkfixtff.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gnopoyebi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gpdcdrvap.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/glcyydpml.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/geizclfwr.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gcdltqvfj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gmxefmlge.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gvchsukhw.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gjijadjxf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gtxdgvufd.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/ggiwqxoic.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/ggdtshgnc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gzckzdsmt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/glkkslyga.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gyzndqvbb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gaozwdtia.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gwviaibih.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gtkhdnbdd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gkixawnsk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gtqgnqegh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxzugvcvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gycxtlxif.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gseohogbl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtioaorue.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gojndrjjy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gnxizhboa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/ghpdyhdhk.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/ggjxdbtei.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gsobpsunu.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gnfsnysce.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gjepolmdv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gyzkxjebl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/grqzmjfla.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gutvpbdka.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gixgoqlbg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gjbobsxfl.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gzhqidktc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gdhvxjqri.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gpddkgjin.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ghtuhbuhh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/goetggydj.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/ghfddvyhy.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gibnigctg.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gahgaocxw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/godjbzccg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gflrmyomp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gqdhdzomm.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gconarukb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gjvzjhnda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gnbxgmmvj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gxoughhxy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gvffdskgy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gdbvulqzt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/grtbqhftv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxcdiwidr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gkpmsvwjh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgqrfsc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gojicqxhz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gevflkskm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gohhtwjwb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gzdacflzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gmwzlaliy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gyeieasxe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gryieczwj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gbedzchhy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gscjaltul.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gfzxzcmwd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gerrpxnyl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gmujiwtmq.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gikpmryoa.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gqanvinke.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/ggutusmag.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvifrhtgc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/grwmziacw.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gwswvuvbc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gxxohqlkk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggomtdolj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gxjvpuvdm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/glqtgusps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/geakfyeck.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjzpbtods.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gzdikveip.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gmxqigovz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gglfkpkaq.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/grncacnol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/guhimkdkh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gjgktovyk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/ghqvdqtzw.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gjaqvolrf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gyrhbeakn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/ggcnochuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gmfeibful.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gtqnqhrns.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gbcqrshge.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ghvgaoirk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gqafgqozy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gtnlfyher.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gzmnfrobw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gseegddat.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbgypbura.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfumkcila.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvgmjiewo.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gcjldfxve.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwdqgjnlk.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghytierrx.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjlueyptn.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gojbbniri.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/glvdpigje.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/grdynocvh.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gftsnopgc.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gweofmycy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gyquuktvr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gmrhaggms.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gtzmqlifz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gvfmaylua.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gbfmahpix.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/getwzkbwf.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gismystlt.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/ganmwymvn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/giwvxydop.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gejoxlhxf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gdphysqmc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gqunwegfn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gbzkzpdgh.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/grhdpdhjb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gygmcmqjy.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gwucmwsus.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gdnvplejm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gninwakvv.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gikxwtmjw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gcctppvcu.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gkznptwgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gkzdlpclx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gopwidjwi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gwniwdulo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gubplhqyh.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gyfhxlxyk.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/ghyubnmso.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gokvmtces.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gvssbkufq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnqupyoqr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gdbvuiwhk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gpwxbuyfe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/galcckrzz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gteonfhwf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gohdpfqnx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/ghvvqtpzu.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gmlalhzrl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gxhfalvmz.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gpomlbbce.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gsktoavos.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gksgghzcf.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gtguqxwgv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gutxdpjii.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gcrdcghva.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gidensrsk.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gdraavavr.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/ghzluzddu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gipcrgbua.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbyxjgjek.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfybrrfo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gkqwqetzw.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjjaclqld.sHtML


<!-- 参考信息 -->