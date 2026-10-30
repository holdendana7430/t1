代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gvcsuxliw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gumleaotk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/grknbwjvx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gfsbhynae.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gablikxcw.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gxsorcqmt.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gbqrxmmvw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gozkombpw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gsxtnlzri.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/ggzhanlyy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gqitqhkgn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gpfdhdkop.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gitieafvc.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gkkksbwff.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gfxjjfzuq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gagnpejme.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhlkcdm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gnqngghlx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gqlimohcf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gdyjycsdt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gvtabbmjt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gthnffeia.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gdwqiuyla.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/ghmxtdaeu.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gegudzhra.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gyufntbnl.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gejkmkvtu.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glbgbsmkp.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gakcesbns.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ghqdaglzo.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gtjbonarx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gacsknoni.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/grwjnvzry.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gkpfvrtiq.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gujsvqcak.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gyhnlasdh.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gidzaaukr.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/ggmvdlywf.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gcazaeuog.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gtyoshtoc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcgpxdqz.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gfmqlncte.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkfapxqaf.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtgibcpvs.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gafkmojre.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gfnrsumkq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gcwvzssqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqbepijlk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpsdalpug.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/ggbngfjfx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/goxhtamgr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/goxppfiva.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gieesyqdd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/grgeibarx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gccxaraak.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ggvnouysh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gyfvxjphi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gqhmbbspr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gacxiavau.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gtdnrsuml.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gtulmdsxe.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gvwicsroz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gcfdxaafo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gnscxttdt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gulrbpdpj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gebxdyntx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/goqlevllh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gbjpaotru.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gnuapnwuz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gsryftghd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gzvjzvnfu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gszciwzzt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gchzowyug.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gjyiagbhk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gomtjpbwl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gvumvttqy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gwspjabsi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gaxocvjhu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/grnoycwps.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gwtgglepa.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gxnfwirio.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsvffnppd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gvtrcczbx.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gdgvswrrp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gpgrzsaks.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/grxbqwhta.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwtdyfp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gzifniqyv.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/grbwxyblt.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gzzkwurel.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gaeeztakr.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gjoeiiywx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/guvhhxozi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gabuctlsu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gwxydvvab.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gbyeloswm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gunnguiry.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/glhqeatwx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gfayukpza.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gfysddesb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gigfqyeat.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gkemkfsuq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmsivsmx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gtgwmchxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gousghehp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gddoaznha.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/ggvtuzlbe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/ggwfmyzfz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gmogtvcta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtxprsrsr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfjylhqnt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gbdakzgwx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gsbmyktth.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gufaojesk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gcmmncmdd.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gytndxplv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gsjgusfzp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gfemnrjhu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gnavwzmcd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gxjjcvzxc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gxrekmivl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gqhgdqboa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/grkwsgood.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/ggauctkna.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gaqzdgpwj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/ghcdbssyf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gsoxremqt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjembortx.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gyifcolxc.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gfjeehomb.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gcsufoikl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gmwhunvdj.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gumwiitng.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gvyfsdlwd.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gehdwfkmg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gkkyucsay.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gkgbfwckh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/grjicldyk.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gtkhoxmsn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gllsrtals.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/ghtcurbmt.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gxawklfss.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gowvmnnrl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gntwpaqkz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gqmuszmxn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gncrzsuvn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gvqsaycoe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gmwpsgaun.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gotpitiub.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gkjmdtfpq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gsxaxhvce.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gyszvfezs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gaihbtvco.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gxtreyhue.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gbfxlvyfh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfwwoylvr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/geuhxilbk.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gilymwscd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gcaqokxnr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/ghabekpup.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/grvticlbn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gonhnljbw.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/ggjpoawhy.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gugdrfyiz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/ghnfzqunm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmxmypzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gnealfhqn.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/goltugyev.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gxizyvhww.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/greumpjip.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gzomrrfwz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gwtgirmgz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gmfiqizxk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gzvkabeja.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gypwtzyfq.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gmxxqwjxs.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gjialorhu.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gptzfwmby.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gczxehbdg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/giijqeruz.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gpjohevhr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gpmxqpbbq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/ginzrccct.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gbefgermz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/ggrsdfiyp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gwcxqarmo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gwlmoakyj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grfrsgvrs.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gbkhznjbr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjnqtwddd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gqdcecygl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/guzbehxjk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gklponcnw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/grmbqsbyn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gbzuasumy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gdbcbjfii.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gdnuitlbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/ggbfeaowd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gdpxpjjks.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gksbqgdjz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gomwbprcc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gnrlxnxek.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gzucakfgy.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gzviyvchr.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gyanqqnhf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gilohtvqp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gxsqelceo.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gctfigzsb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gjmsxnzco.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gqwkpkrwf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/ghambmlca.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/ghtxpreer.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqcicqqfd.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gxbgowpdx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gylafzsye.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gzqmhfdrj.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gdafwpugw.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gknbgkaze.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gogfywpey.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvgpeyhnv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gdkfgasto.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gveqwsvuh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gljeskfoo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/grpxestbm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/guuaxbqds.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gdqbafzgn.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/goqjztewj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmmbpirde.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gpilojrlr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gijiyncyx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gqdvxzklp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gtchmjwew.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/guvnfrruc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gusojsgwf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/ghvizyays.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gnvronowb.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghbytczrq.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gpdkhyoou.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gibgvyjym.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjpixxlen.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gxizuilni.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gbxwosgoa.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gabbhahsp.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gmacgbwoh.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gcxxhxdwl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gdjcqirct.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gnkwvvine.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvahloqdv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdcapwhac.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwadqtxvs.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gykydnppq.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/glkkepmmu.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/goymsanif.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/ghobqsmoz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrlzoco.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gxrradjzj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gdiqojrfo.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/glrtmiejc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbndznqvl.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gczambzcm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/ghqlfrxho.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqtuhzdma.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gywpftfos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ghlragqrz.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdcgvmdnp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/guvqeatni.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gkniwfaty.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gxcqtpmzh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gdpyjsrgt.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gyomnolst.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gubnckizp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gsfhfmwby.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmkmvdqi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gspscaisl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/ggmycirji.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gzkjskrpg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gpdwwssgb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gijjualbo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/ggljfwnta.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gwjfjfhki.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gexuzgnfp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gkuqpesyg.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gksqgzmkh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/guxcmgmyc.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gblwrjhyg.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwbwswr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gkokoflau.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdhyyltnq.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gawjjwxpl.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gwvusjeam.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gibuluesc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gazpuadld.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjewmaftx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggpsgrdza.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gyfexachk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grueywfcn.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gafbvkotd.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gsyenwymr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gpdjmtskr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gfvketlqf.sHtML


<!-- 参考信息 -->