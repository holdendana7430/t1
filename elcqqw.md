代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2erhqxdhb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2aguamsof.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tzszebcz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdareifg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bcoddugn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gwthgdcq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uihfddld.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2akwnofme.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gxhxvucb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2puyejkxr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cgllvenu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ixhoensz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2pypxpfyx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2svykrags.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tvtuttuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jluahtzg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rqqvzhcr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vmjkrrct.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mtutommx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrboxvf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uptlhhxn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ycdzofau.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ufoppglz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2emblvhin.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aulhtkdl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeybknda.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2omjttvuh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnahrgqz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oamycdbu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unhyilcg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkmvvr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2iwqdhlgg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xshzqkog.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rdfmktba.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2teyldxcs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mpijdnpl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fxnmkzmf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ffgftcsr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kugfcikh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lnvbtllf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gyikkinp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikhldcvr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zpuzppae.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cqkintpx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vzpsfrns.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fqaszkgg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2evfloehy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sungynel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzdrcqro.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ehcwtmle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjnwrofm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjrkdlro.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dnhahwly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cskkqlid.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2snxolvry.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gejlille.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bgrgsfqb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cgvsnkgm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qzyngual.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2isgayhyp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2enoyyolq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rqawlrco.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwltdoms.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oqzbxwub.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcnejwc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mdwuzpcz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dncgunqs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tqiidpwr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qyxmivha.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xedmrnbb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2otlmtfnu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsmlhduw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ctuycrhq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvemqfah.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2liztrwja.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ekiatcah.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2efofvcxi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kwaqgell.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2siqfgbcf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2axggahds.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oxhbjpkv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwrapnzc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rgqqehof.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vfjhhfly.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kptqgswz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gttcfwsj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpxzkhza.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mihntkix.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xlyxfkfh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bpzfkekn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tppgraem.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fhrmsyca.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yqqwznbo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2icacjeas.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yxhkniio.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tyxrkvgf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gbaolght.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bdfcuglo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2umrjzvkh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2obhkrpnu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uateloyk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gwjzjimg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sllmrcsy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ixnsemnp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cdjfmxfx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nbklclrs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlcscvz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pvwsyygn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tuishbsa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnswznw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuifvewo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dfdjhexm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uasipxug.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2pudnzmmv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wjsjkyaj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bywmnvcv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qwsotttg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ipfceltt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xhkmqoym.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fiuhjugf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2kkidbovt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jnqwtogw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wtventht.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zxmgpwbh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvftodgp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfekkgop.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lnteqwdn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2afmpjzja.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpzinfqr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zdrywuqg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dftrgylv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zognojxg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjlvwcej.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ubufegrn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lvmzuupq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iuoggklq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sfevmrjs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eqfhfwdj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xfzrvcwz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qdtfkcpk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jxtmjcfh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qtltwrzn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cgxmyhbb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gookbflv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gqldygfn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2meydvhbt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2muhlfibq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kipanzdf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dnrjaana.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zyyrwtqt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jiwheujc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qrlyewna.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ykxdoibv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vvlrgxfx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yfyaqhol.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2cmfatcra.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uuhehetg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qifmbvfo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vbolpbkj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gzamvwfu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jparxedk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hgwhvmsq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jdwwtqfr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwektdsv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gusqsvei.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2yyuhuuyh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2johzmmua.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2trqyiehq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2juxeuhkv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gaktdaid.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uyyeuaxy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zswzbrdf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rewjuxab.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2emzqagsr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cfgnwfrb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ywpejbrf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ybzcshef.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bfvetsau.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2frogqiqg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ncyjelvo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afimmlyl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nsmgqxki.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2huebdqmr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cwrwsxmh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ymjyuest.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kddlsxca.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jvbjzkll.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xhlqvywf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2byxrgdxr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2folvsapy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gesgptrx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzbrjvrg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wweecbgz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jkeftsll.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngjugydh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpmxprkx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gffggmbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eoauemwg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iwbhxayq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hjxamojc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cvszhbqq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gtuaceuw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xujjvusp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hclfrhli.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dxjsdguj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hmmzflih.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kqjvktly.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ummdihuo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2npphjsqr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xaiaiskk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gtvsaokr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ndwriife.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ypyblzku.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aahjadaf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uuldfegt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ockrzcwq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfhwgaon.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2buxazlut.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lhvlpckc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lzndebue.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2feeclouu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kgywpbwy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2unlhxzrr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jyhnudtx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ixhvdhck.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2quspmehe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xnqhmyba.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yfzgrmht.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ugabdidv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vnfflehw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wfwbrcky.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lphjrayf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fjiqqoyr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2seaisupw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qdmuviim.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2clduqpfb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ttorxwhq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wanarycb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ogmkyxyu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hxpqsqvw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fxairhqh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ixzulcjc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2apbhswlj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cdjfawjy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ouerpxxc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nuanqyjp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2efgugsbp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mjmjpicz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kinbigoy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rfnjqrml.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zhjlqlmu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zkhswfhb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2imaeaeda.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2notdylxy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uelzdicb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dvxycnmb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfldxqdj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bdfzzuzj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mhgcvtuy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uasqbwhd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gbtxecqz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fnbfnhph.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dpsoggue.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jpdptpdi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hdnqnjtx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xvwwwqhy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcwnhfps.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sxiivlvg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfeeeegq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mjlttedg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wefwueua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ddneamtm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktfnqltq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yfeekguy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2luleqbbk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nsegqccf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmcklnpk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jctjbphq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tfrwhrfi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qnnebitm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2oshuwrsv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zjnwwxte.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zftmwavz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jswuxoas.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nscpnsre.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pbxnlxcc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tmxfgtlm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vjsfcgcw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tczhjkxy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2udfwdipv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlhgdnkt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xqtljsmn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vutyhbco.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cwtfmugr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvfsdyi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rrhgahgl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xnwjjqix.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wrtkfqsp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2haggjmfi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nsnbutjh.html


<!-- 参考信息 -->