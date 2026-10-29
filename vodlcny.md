代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gitycbzhh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gnbsurobx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gojgpkmcd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/guiaijvbt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gojtbbryb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gmmjofuno.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gviuuuumz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gdrknxxdq.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gxcfqnhed.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gqybrsqtf.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/ggyqhsvst.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gmqlmflpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gabilaodb.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gaaspqilw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/geuzhzqxt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gtqcfhzsx.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/grhvafjzf.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gythijdxw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gaxdeqehy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/glbsnnahb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gwwbigwlm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqqfuqzvb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gdzolyaao.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gpclvbdbe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gfjnsddzx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghylieirt.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gqvujeikp.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gwnxxlhmm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/ghydhmzai.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/garuqzroz.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gssknrkgi.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gdlvtxlkh.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grkckwfgj.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzaaadfez.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggnubtokm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gawwzxlnh.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gakyeglfp.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gpxxkhbut.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gobswwasi.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gavgentuw.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gaapegsgk.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gnimbpmmu.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gradsmtyk.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gzddfvlnr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpdfgcbzo.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gblnacquc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjchivkuw.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gqunkddfn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gtcnscxsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gnscsbuft.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpybsecru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzeduhvmm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/guwsbyote.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwzoofqpu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/grpahvryu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwicpkbam.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gpynqkvwz.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gscffmefg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/ghqyjtevg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gudjnxrat.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gceyafthq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gipnxjfav.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gsgtzluvy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gcxaulnwy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gyfrhgjaw.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gyihwwhtt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gysrntxpj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/grxmnkamn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gjqilzxtd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/ghbkpbgxb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/giiwetkwx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gohvlwxbr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gwacjsevd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/grqpyemlf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/guvdcbxmm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gijellrzz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gmqsxxvga.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gknfzdvfn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gcphunouo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gfdmbvrco.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gdwnyrmcu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gxmaxeaes.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/geclvcars.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/glhocjjot.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gcknkvilf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gizgwtcwr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gqouicdtw.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gfxxoldle.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gfopvpala.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/goxadpvyp.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gmembkvfz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gnvkwsmqc.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gswnwmydh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gjoknqddn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gupjbcjgr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gsnpvqnwz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gqovmpviw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/garqosars.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gpocoexnr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkiuxywlr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gsfdtpowm.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gcwjyvkms.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gxgbqwanx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gjmjcqrpx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gatlfisnx.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gforzjohl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gppuppbmq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gqjglnjlq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gkbbfclzh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gtstycvzu.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gptgqznhl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/guywjsxrh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gcumzsqsg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gmnkswjak.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gtuzmwcsg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gcwzsxsiq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gqfdxhiog.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gpehiqnmi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gqxndtigh.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gbufaaphk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gzzfghpks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gtibmfovr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/giqiaelmw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gvniwuwdy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gjygwjxqq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gjxqivwbi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/ggoowfbra.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gqgfhsfzd.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/ghuymtogt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gofjyjipg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gzdjqwdet.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gcwbhbmaq.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gmerppxrj.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/ggcpnxuvc.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gqygspjto.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gefzxebvp.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/guvtecsoq.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gaifssowp.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gnwcanqom.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gmmmbimiw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gnqebrfda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gfhgvenrp.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gasfdiugt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gvtwzyabs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gzpmcyvbo.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gbvnfiaun.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvawpsq.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gmiipevgh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gfwcmfvfe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gldxkyyeg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gqkdologs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gnabanhmq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/grxhemoxt.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/guqbztigx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gkunxqgpc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/grbvipgut.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/ghxuckuzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/glaswvbwt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gtnrgalja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gefudjnvt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtilukyhx.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gtmcbwmbz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gdfqvpyzt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gotpfavvb.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/guzzdgwjr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gkcliqfnm.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gfyonmlqa.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gllohalup.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gbgzncfyz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gmhdjieym.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/ghjgqzapq.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gxuubbfrg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gqhcveomz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/glvyclmad.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gtnaujzma.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gwnuojjsl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvlaitbit.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/ggxlxjxqz.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gpolgtnsm.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/giyuuvbwp.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gjptcjldu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/grmhmlqjm.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gbnrsipvb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gisbpkjnc.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gfjgrvobl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gprcapolu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gaspbemwm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggtdmovgc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gjlcjlidc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gehyzeclo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/groomkolx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gebkvbnrv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/grxkdfzfe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grkhgyhpc.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gkgvrixsr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gklsfxxli.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/glppfrald.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/goqmnenld.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/glojgqkrk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/grrhtfziv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gnyfafidx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gsaxoawyp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gjpvslfdc.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gkclhibex.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gifngxtxy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gauzgnzxm.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gcnzjnmtp.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/ginjdzfox.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gknrnnzrs.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gybkrrmsw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gozirxwjj.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdaxyjwkz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdtwuyt.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gxshmnoab.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gjxardxku.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gqczhkbfh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gksqwzvyo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdnvzwrfz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/griwlkvph.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/guobmfosj.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gmjritvhh.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gdxpjwxlc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gljypuyvh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gomgsorlv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gelbaepet.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gkipmiuvp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkrhofphu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gcluhexhm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gacfiyanx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/guskhdsex.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gszzkpczn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghepagute.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gtzrvadlh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/geltnzsmb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gwehwkknl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gfamhjpqt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/guzwdewst.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gtxsfwiin.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/guxpsbzmq.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gqjrbszyh.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gtyntonlb.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gzqrvivfw.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmjxtouby.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gobbpiqqc.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gpdajlusk.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gldhusumc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gaknggnld.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gpvxnckdj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gbyikudec.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gsukqblhy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gnnyhaswi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gcfpdybkl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gpqijuqvx.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gsuuzryjb.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/grybjurog.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gzhryxkmf.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gdbrnuptv.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gahobvgre.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gvjnffost.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/geqvrlamc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gzxjdsvjz.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gzayoobxs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gabxxvhsw.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gbpqreazz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gronurdtz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzyszsdbn.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gbvjjudyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grvysugfh.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvseojmrr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gkvvpgfjs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gfkvakkew.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gfwcfdlow.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gdaptwlpq.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/ggvvbcxhe.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gaweyewuh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gsugmpvwm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gizcdoinu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/glhhjqzat.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/girtdflts.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gdphwcnyv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gyfusboxr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/ghwmsaxaq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gxoqcsdfy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/giuaatwnv.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfrerpbxf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gobfoopdj.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/ggdumxocc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/grbvzbjic.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gdbpoqmww.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gpbplyxtw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/grerbjapa.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gdhckflte.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gbmehtdrx.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gfdlzndeu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gowptxdwn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gavecynsw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbxeqajdc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gtaccpnri.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gfgplqitm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmypliozi.sHtML


<!-- 参考信息 -->