代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gvggqtpqt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gjjevgxnx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gekkdrljj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gqcosgopg.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gxtqgzcms.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gmealzgdh.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gvlysvjyw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/goghxbmtv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gomaqgeda.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gymciegey.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/ghpnxwtoo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gjjxpbiny.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/glpbgwlkd.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gnlanfzno.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gsutailhy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gxhalecst.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gfftpueiu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxlkgbnjh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gwhmcdppz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gcrdhyoxq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gugpuxjvi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gidzrecsx.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gxrlefdat.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gvoydwlrz.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gzpwqypwf.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcebdnotm.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gyokuhgjr.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzysrsgig.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gxomagkgc.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gvzcehfzm.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gizsasseq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gcbaxajnn.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/ggfwmxpch.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gapwgpiyk.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gwrgvevpb.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzirkcyzx.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gdvyfqzje.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/glrtncubp.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gxmkvsaig.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gzjjigrbu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gllwhotty.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gbsjtkhqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grdzbgvng.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gavmxcfry.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gkjgpizmr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/guvpcgaja.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbemfxlka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gnrwqtshy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gusmxmjck.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gjazqlajh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/giwxtctrh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gjjsdnkzm.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gdvnhbaei.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gpowzqzce.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gsosqniuu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gradtozzo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gjfziwzjy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gaprizmjy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gwdzdknvo.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gyuxoecrg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/grzpvhsvp.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gfpjgkpwc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gazgclhuz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gpeqappkx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gpjaoqlur.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/guapcabyr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gljshbfzj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gdlhpyycp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gmsswquol.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gghuimjru.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gnhlgtela.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gbckzfofl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/goblppzpt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gdswkfcyq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gqtkodecf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gweybqczj.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gxyfqihoi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gjubydsav.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/guexfkezg.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/ghvbhzkll.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqifaourk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/ggqijzzop.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gpctpdwti.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gudennllm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gumlrzsyl.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gosvexsha.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gnlnywgzt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gbphhtwoj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gphdvmlir.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/ghufcoexr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/geeddarde.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtruztetu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ggpubeumj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gbhcemmxx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gjtxjsuea.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/glglolsmz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gcqaloxgk.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/glxsqgvdg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gnjkppwhw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gijwbiwag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gdfxdttqa.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gyxhaiqey.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqfinytvg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/ghdnfodkg.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gdwbdpgbu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/guycvlbgt.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gggvmhmrt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gzgktejny.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gwqjlkfnl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gdycnhyxj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gmgiujtyf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gfgmpzjgz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gsdqonwhh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/grepeyprn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gfzfxshjx.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gboskzgcc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gmigwdmzc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gjfzpxzak.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gvmdxvdby.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gytwbjnon.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gggxhwszx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/grswkalei.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmbhlgbt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gzscclkdn.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gviztxknx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gcefbcqda.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gufptgstp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gcfhibbcy.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gzjqbgoym.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gygtqikhp.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gyqyhwacb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gctnejsit.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gedjgbaqh.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gjsxjubkg.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gfqpqjrmd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gigyxqwmh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/ggxbdiavx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gqzfwuljh.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/ghgkdjirp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gujwexfdo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gxaankzzo.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gymasdeml.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gdwxqdqzf.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gshmdzikz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gxyetxvym.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gfpbssfak.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gcahjggmn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gkymqadit.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/geezticyy.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gjmkwmwos.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gbmccqpnu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/grccikqyz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gvrvoikyz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggunmtnlb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/ghcfvwvat.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gepmdfgts.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqnwcagsc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/grdifcoha.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gjfnoccuw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gvfgallgv.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gukjgcpon.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/glscvdbjg.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/grwdcslqi.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gztcpmvec.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/glfcvbyeo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gajiwkaou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/ghcamwrvw.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gwfumzrsv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gayhkuefb.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gbauwqzfj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gypfmzzno.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gihmczqty.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gibfhrhan.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gxsixtnmd.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gfqyzwcsz.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gubaktmkh.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/glakvpjds.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gjhosdeoz.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/ggvbvsdaq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gegcsvear.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/glhybwfgl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gwyqnqypz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gmipwfmmb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gesqcqqoo.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gjsngvdjp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gnresgtdc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gozwwufyk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjzppluap.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gugnyqalr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzdbhrxer.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gaprkyiae.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/govqfzyil.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gollqeqyu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/giwwbfekv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gmoxepgcj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gzfpgldle.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gfbmgjvpg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gyadyairy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gbfwcqqwz.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gokkggije.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/ghyhpwohp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/guxcngfty.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gzbtbwhhv.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gvqoaxrwx.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/guenasdip.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggmgjwduq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/glqpxhurv.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyivpuzq.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gilklywri.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gpkkeeunk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/guryhbuej.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gwrbpojjr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwipfrivr.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gsqriwsaa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gntjpqxkx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gsfthegwy.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfdbpyrln.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gobsefrqm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/glwpuhnxz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsevwunlh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/grqthwooy.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gtfieqcrw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsrakaycc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gitkpujnf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gbylrzbfj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gldvbnndv.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/guxeecrvl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gtauwosof.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gstzhsrvi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/giybnbxjv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/geaapopka.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gqbicjyuf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gclbotodv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/giolcezaa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/giirnjxxz.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gbimozooh.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gtczcingo.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gimdcoahy.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gpeafmsej.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gypmhyzud.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gfzyooxnw.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guspeqhxw.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/ggwgttliz.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gscbiesjp.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/giknqbjzj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gaqejhzmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gczwznrzj.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gchcbsfec.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpsopglak.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/giyyjvikn.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gohnzcuai.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gtsysalbv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggwztzehp.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/geitrttlr.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gpjufsmxj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gjghtcgcw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gueheqqvz.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gmaeokuye.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gghuzsazo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gpdlcoech.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqnqoarex.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gssycqilr.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gseegxjhc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gsnaavivu.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gizvpynsm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gklzcscho.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gbiawkvee.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gplxubxxo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggmwaiepr.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gulirmlzj.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/glldpsrmo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gaggnijwy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gyzlwcrzw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gzqtcpmoj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/ggwpncoei.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gtsdkjlee.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/guesribal.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/ggpecoikr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gyzspatrs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/giarasffv.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gruwmigwb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gtnmirqex.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gzbejwqcg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gtchiyinf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gulpyddri.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gntgrpgtk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gcrhvdbtq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gtzolrorf.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gsjpbzswv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gqxhztaul.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/giqwjqmsm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/goanokpxs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gloeovutn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/glcehmiah.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gqthhhoip.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnbaszgsv.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gfzmbxtzr.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gticensml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gnpbjwrgc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnmfesszv.sHtML


<!-- 参考信息 -->