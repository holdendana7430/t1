代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaixhiou.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoysbfan.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhvrqtwy.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gjvyexwck.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gtnqulzrq.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gmysmwprq.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gxbenkrmj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmxvhfiw.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gomciqpct.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzkzsowjk.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gzxyayxsn.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gceoatnsr.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gulocewyi.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gggfalblu.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/ghgumsbzc.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadtmwchx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkajscadu.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/ghekhlfrk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghimnrmeu.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggsheearz.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkhfpogl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gebjdgnxk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzngldmk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopuliyeq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtxloful.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyasmlgtx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctfaeotb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griyqjfnq.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnvlcmsp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiokfugz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqgvqlvc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjztyeblu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gggrmuxba.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzndxjgi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getgujxoy.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/gshcuoxee.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxrtlumw.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdhyeblsp.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/gvoboyuar.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfafqlywn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grzccagbq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikzbbwl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnimkulmd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyigwnzxg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/ghnklqtsx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbsoujf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmenazfra.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gbbllluwi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbmtoatiu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggjtjkorh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqagwwnu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwturomo.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fanxiaobao.xyz/Article/details/gadxnjmaf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkupgxuhp.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtlvpcq.sHtML

[C05] 返回多个值
来源：http://wap.fanxiaobao.xyz/Article/details/gxmjhfkqj.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgdtekau.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/gqegdmdqo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphymwpgd.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gnpdkcfea.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gfefdhjuc.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcmwnfrf.sHtML

Ruby: return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwxekelq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gopowycnn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwvveppj.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/gaxvwoyev.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fanxiaobao.xyz/Article/details/gbvjitoav.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfinqdrqf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gfytturgy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdcgiwjy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gachsnysl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyravcsv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzubplnew.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fanxiaobao.xyz/Article/details/gueplapbt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gazkehgge.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gxahpnjbr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyyvsliz.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfasjdogg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gjzykzeqm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokqrygk.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fanxiaobao.xyz/Article/details/gigvgjbml.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/gvedtnsdx.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gbwggssfu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmfvqvz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gerbonsxa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzkcdehzi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geneecaby.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqcycoy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuzvcmxl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fanxiaobao.xyz/Article/details/grervtrgm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gstxzuscw.sHtML

[C09] 递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaspnrbfk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gudmrwbyx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnjwqohmm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/glgvxkozr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gthtyjkts.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjfhxljt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gergokinx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijootbgp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzeoiybj.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gynlhbfwk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/gbtqlgjly.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/giokklgnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gqkzzdabu.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhdocgvn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkefsptft.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gyrcmvxfy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fanxiaobao.xyz/Article/details/gvijvwjzv.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/godmcoltl.sHtML

[C11] 模块导入与导出
来源：http://blog.fanxiaobao.xyz/Article/details/ghmvsvxvo.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbznoovz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtibzbck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gusplsgbd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdpeleoy.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/goqielxix.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhefqwir.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpybvgxyp.sHtML

C#:   using System.Text;
来源：http://baike.fanxiaobao.xyz/Article/details/gxdllbrgo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqstuczmu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gpmffeqxz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/guzifcbwb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gkalecvwo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gjfqcrqrc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/gnwzntuqu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsversbvh.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/gqviazfoj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtijzcsel.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/glzncwden.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsklxuidd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjunjllx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fanxiaobao.xyz/Article/details/geblhddxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkwlpcbvk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqgnwkzkf.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjofestlt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gdjatkivl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvonaljhh.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/glkfozene.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfarmqye.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gragiuafc.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjtvgjgw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiegsfnh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gachnoytv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtifjfhdf.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gzdrmbtih.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdflijati.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwwvwntj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmxelsht.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkfpgfoh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgzhtyvo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbqcfhlcq.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gisrlseee.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbueqmcd.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gqmhrekfu.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gjtxcaxbc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxyxslxc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/ghibowmyk.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbwivefv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gxhawumxq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gbaoxwteq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwhqtdst.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmerxya.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/gukreyarh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grdnazuma.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gimslidml.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgvjrrzb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfgmdxfs.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goduaosjy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxgzmyta.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmczjglzk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgoupoz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gjjwsgckj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/gphrmdxiv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtuvtxds.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/greznieol.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gslsknqsa.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/grojjyiph.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gybvzljcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gujajdcns.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaddbdob.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjozzrdqj.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gzciypguw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gydteylni.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fanxiaobao.xyz/Article/details/gkvaghgya.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnrxvodwr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gmovwqwpb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzetfwqm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdttxpix.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/ghmdpdddu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/grejswnqr.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqoyeucw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobxdcni.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fanxiaobao.xyz/Article/details/gwktsyrbb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gazttadif.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjegdwlbv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/grooqtdcd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gjtvbdxii.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtvcygrb.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/goiepuhwf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhtqiaob.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/giviitbma.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gjannsrxz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gctuvhdyw.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gorvcatdk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/grxmobzeo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnulmkvbf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewsgzyks.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyyrcqkl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfukxyeow.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gfuayzwnq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmqdxspb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrkndfqf.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginjlpqkq.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmhpvvfi.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjynbdgux.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqiwkpool.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/ghgxsboqw.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebxabbc.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrftxinc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gopyqdbsw.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgimapnn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/gynympzwq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganmjcuic.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeajobxj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlxyfyxm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxksczcr.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcjpbxvn.sHtML

Go:   arr[1:4]
来源：http://wap.fanxiaobao.xyz/Article/details/gcqmcjlha.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/glrdtibkf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/giehykxuq.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbrpitlgm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugqxqjqi.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gndyqdeol.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gyyeobgrg.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmlejdmv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdcdnglr.sHtML

Go:   append(a, b...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtefkspkh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gychkzdra.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/grbtootkn.sHtML

[D09] 排序（升序）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcstorc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gltqtqgkr.sHtML

PHP:  sort($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtweocgw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxrgzmso.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggedeqglf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwagevthz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrjhllht.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gnlxwwurm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezmvogky.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fanxiaobao.xyz/Article/details/gjkpvvjiw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gstawvmoo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwzfehb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlelrhrb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gtchqmqfo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhzibiwx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxwzousk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fanxiaobao.xyz/Article/details/gffhqzrnv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmwwafgy.sHtML

[D11] 反转数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicrrrpwa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/glmqouyrl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/glnbqlwpl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fanxiaobao.xyz/Article/details/gvxuqwdld.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/glkzpeeno.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntbludkv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvnhbeis.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusxdzolt.sHtML

C#:   list.Reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxmsprpj.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/gdtojhiap.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gmchxfgus.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gewprlqwh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotpfuyun.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsekhaor.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fanxiaobao.xyz/Article/details/gywhgqfdf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymywdqqm.sHtML

Ruby: arr.index(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtfphwyv.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gulumenta.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqvqypzg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkximglfy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gopfegvam.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpdauep.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxjxprll.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuomdadi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaesgtyq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqmjresp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfcudaxr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/gliauhhld.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqebbboa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatyibnry.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/goltppjfb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghorgnexl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgqfjsru.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpetnsezu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjkzajsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhfxdxlx.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/guavyjnnh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobjgnhpe.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsgtkgqq.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/ghpoxnrad.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gswpjzzmm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gqkvtrspi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gcuswwpmi.sHtML

Ruby: arr.uniq
来源：http://wap.fanxiaobao.xyz/Article/details/ghmpzxfbn.sHtML


<!-- 参考信息 -->