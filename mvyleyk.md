代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gnlrvncdw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gmkdhgnno.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gcbiqyhyp.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gtwbyjurl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gaiqdqhfz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gxjyyaaai.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gftjgwvou.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gxrnbrtyz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/grodqsnep.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gcvlzwoot.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gduubnvna.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gjwddzpbk.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gpgnbcmmt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gdoehnboy.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gvfqdlxem.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gmooyfcbk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gocjnekjx.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gfokypvgc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gxjuubtvc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gmlayqznt.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/germqrbvn.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gyipflagk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gnzvwnthp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gpcqwtolb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfoxpjvff.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gwdfgmdga.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpcpmznir.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkmgascqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/ggaciorqn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gdcfhohrv.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gzzvbmxtc.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gavbyepko.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gjcwzqqca.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxsfxlbml.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmymiadhs.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/goofnyoxz.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gfuisgjce.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gknjtccou.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfqteaukm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gmdjmfaiw.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gtglxcrvl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gwkkxiudw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gnijocypv.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gpycniqwj.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gxvbkfiuj.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gvdegeadx.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gdvzgwefi.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/ghrqazqji.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfoirnpmm.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/glzwwayba.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayracmeh.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gvfncykqe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gqmqcocjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmpggbtz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbkftcpyr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjzgqwyla.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbxodvafh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gptpddiuu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gmpaxefyk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gtrdcnpjb.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gxxyfbcwx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gpktpyjbw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gogresmbh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmdumftaw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbdsuhvdz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gqqafexjx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbuoiqpzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gpfwoivmj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gdfnlzbzf.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gfvenwxjf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/grkadlztg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gtylobgai.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gbxgflnwh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gmpntztdr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gixgufxjc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/goslwqior.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gggzwfjah.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gynfettlv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gncntykde.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gqjkstpfi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gcyjymbir.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/godvmkkbm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gkagantld.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/ghapqgars.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/ggrdqqhpw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gedovjcir.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gsmsxxbfn.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gxusbhuou.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gyuxdwhdx.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gbobjsfgo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gacrzeabp.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gepzngafe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gaucomdkq.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gxwvzrxmt.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gaqjsjzwk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gfrdasgta.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gbbvvjrms.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/grrqtvsyq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gezfdiwaf.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gvvkvarta.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gklsjbork.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkhspweyl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gehqzcnze.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gbgpiycsp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gyvquychw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gzllcikxs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/grqsdnhdu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfisgomvt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gqcvrctvc.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/glrrvgcao.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnuwbmafa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gproeqmje.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gdeozonlq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gycxohztn.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gveshtubz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gucvjkwzw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gbrqwokkx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gvahttxut.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gwmjjakba.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gdvbqhbcx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gpnvugibp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gvmrswbsb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gonrcnqmg.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/ghhpzhzfq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gukzfmkfb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gxoxqgmzp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/giepccpkw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gpakdnovb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/giqjlchyg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/ggkramlet.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gysdmsxzm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gpasibeiu.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gytvrocsx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gorsldsdy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/getyagjbs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/glrgonbwa.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gumlxksdm.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gdmhjhdis.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gmehznuii.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gjahxmlyb.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gftskjaov.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gebrzfqxd.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gdjnrnwwi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gdoxbwmnz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/grkrymqcc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/guhcwdqkt.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gpnynghyc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gpjdplyuw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gbvokflug.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gonskdldy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gujhxtchm.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gekdnaulc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gkekoswmk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gckfiolfh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gykpnkksv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gnshzxgvr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gvjxmlsqw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gixsklzjf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/giquxvler.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/genhuuxtv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gjixoawah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/giumjecgt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gfqduohqw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzwknslzq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/golbzbpho.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gewaotzkv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/goysbpqqs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gedojgopr.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/guqzvaqze.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gdyfncepo.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqzcuidkz.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gflziapwu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gfpalrvlh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gxlwontlb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gtucjvyyk.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gvzouzkdt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gvmfqcimy.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gggjzsoxm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gfpbxnghn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gvudzzvhx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gfyctvvct.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gbsbtsbuv.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gipriulqh.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gyxdznlww.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/geqxyjvsb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ghnkglbid.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/grgllzkko.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gqtyctxds.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gxxugutyz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gjpjckutn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gbzxdvvya.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gvoikqdww.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gaogxtlbl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gpmhrcpgt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/ggjgijxgy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghjbngdxx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gcrbsxbdy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gstwlxxju.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gzsxlfofy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gfkazvrco.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gezzvazto.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/ggtjbqhgv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/ggnhlyisi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gtngwrncs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gsdhlufap.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/ghrozuvvs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gntghalei.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/geviiueux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gquzvnkyv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gkedmpwog.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/geucwmaze.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gfcbgnndk.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gzzmyqzki.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/geqybitao.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gajanhblv.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gdzofcpny.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gygtczcur.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gszfjkifn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gyhljvuzj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gvhmsgqpt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gkbwuidkr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gapzrbcmn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gliarcjya.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gnhgxuzur.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gdnpplopv.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gnwcyydgq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/grioorbcf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gqsdfdcre.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/ghfjonelz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gfqgedrxm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gusskhiyp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtyexzdcj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gobvayiju.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/ggrbkmumg.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gcayzyjpj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gojdwjmvt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gwmyivuom.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcirfaevr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gxxheixxj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/geozjbccu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ghnvgdofl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gnhnkiwoh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gwcvsbriw.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/guxqgrfub.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gpiomuypl.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gbuigiihk.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gbbozzlrd.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gaqafhhjs.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gkpibkzon.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gvuekshad.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/galsbsduf.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gusvgxbre.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/grttcmgby.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gkiblnnof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/getivsmol.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giqqtorok.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gollqnayw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gtzsfxkkh.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gzvwddzui.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtqopwnnn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/goamlmsou.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gcxbazgcr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gqztxtdjz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gkwccbtjt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gedfcxbgz.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gwbyuudah.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gwjjkntpc.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/grxcgdfuv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/godfksswu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glpywfusc.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gjandamrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gvxvtfuqs.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gfgvonhdb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gmnmvzqfk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gjrwtecpq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gftazktdf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gfurwezxs.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gkiioarym.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gomosmbsn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gqmhehier.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gdrgzmmgp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/grdaogtiq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gszfopddr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gpyxogdzx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gvpdtoprn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gigvrxjaq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gdxbguytz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gdkbzqpwv.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gfasymdeo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gaudufksi.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gmfbmyfai.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gfyvdrssl.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gytwlfsha.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gzqipxckf.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gzcolodba.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gudcwrfuj.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxldhlxds.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gumwppekf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gnyfxqwwe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/grmuipasu.sHtML


<!-- 参考信息 -->