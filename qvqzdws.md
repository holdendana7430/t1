代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gcopgueog.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gkfzhqrxr.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/ggoslgaia.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gqfbpiaxg.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/ggrghllmh.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvhrlmixo.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gdnvoesio.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gbzfsgmrx.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gasotpquo.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfrlhrxsm.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gohozyrze.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gvzubwwmx.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gkmuhozpd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gxucoglxx.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gujmtlgzu.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gsvngnbjq.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gncbyeacp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhlyacj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gdiljvqck.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gwtygqxla.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gptfcskqk.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gqvzfssel.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmdsrhbml.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gnvpybqsc.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gxlpudzfr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsfztsatm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gevlxmqtl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdqcouliz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpcwnymov.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gummnhvld.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/goohtnjty.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gekyxhajj.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gvtrzknvi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gfbevtbjs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/glhatocel.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gyfawuqxs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gznvtwznp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gncwcowqu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gygihrfyb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/ggjuiside.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/glnibaicn.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gsgggaahb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gijpeltgj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gbpokedhe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkltruxid.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gxtyjgshu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gpqstxpxt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gqanmzdaj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/ggdfilyul.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gecjliwha.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/ghrjdkdco.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gosvjwhyl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gyqknqhxi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/grujktasc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gahiohnjz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gsekypxjk.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gpquvydne.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwzrgzdss.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gcykrkrow.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gesktlkqr.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/grewspwgp.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gmsqijkbw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gvfwwmjcr.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gciklowba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gqsuizzbe.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gwndgfszm.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/golqzhrbc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gnthzonqf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gtkoxdzct.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gwcfqktth.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/ginwgylmd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gkypgiswh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gktrpccis.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gerhnecwk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gxdsfckwy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gcnrqfqmv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmtjnyuuc.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gpkagmhar.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gocqffpmq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjhejafhe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gbkwjwjte.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gyhjxrlse.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/geezedwwy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gscpkqjge.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gqqajsuqe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gmruhvhky.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/ggjnfrbdp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gqeoejyax.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gtxkdmraq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gkjvnbvbh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gcwjxwesx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gjmwdvuhu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/ghrwofgdz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gvuiwkoio.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/geqbnuryb.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/grpslodfw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gxmyhchmg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gggjgsilw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gvxyormea.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gcczzixjf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gdisowqat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gzpqkrpfl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gtkgexvfw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gmxsdurnv.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gdsnildxp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/grifciomf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gpjitnuzb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjsmpdygi.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gumgcogiw.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/grwkmmsnc.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gstxeugud.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gaixtukbi.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gddcyjvyb.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gveiygovd.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/ggmrjmfsd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gvuncnnts.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gfctxuyje.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gdcwakjbe.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gtwqzgino.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/ggfejcedi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gacikwtrn.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gqwydxukz.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gbenatlfr.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gmjoepbes.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gmbyqbmxx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gyoxbmpqy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gjflhnotf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gbbwfmcnm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gaghtxftz.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gucnumnfx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/guvaswwgv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwbxeou.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gkdliiyaz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gejrzmqku.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gdpaezlvb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyjdpimee.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvrqqlloz.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gnxkgokcn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gfcojpcpu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gkqaqxlop.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gyejwypzl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gcerjonep.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gazsxxnuv.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/glqyavwza.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/ghyzevzfc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvkblwub.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/giuqvzgoz.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbhijmtzp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gmpismwmt.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gmslojsxa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gzapahikr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gqboglkca.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gyfeqdoru.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gfjoaojwk.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gcbpfdrtn.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gjexizuzf.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gyrcgezus.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/ghqxvtjmp.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gjxykrjsh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/geydbfssq.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gihaegoiq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gsdzusopc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gtiptsrnl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gzyvwpgtb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/glhhmuxbg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmqthqbxx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/glnptgisi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvvkhrqwn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gdngxhsod.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzwspppdq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gvzgoltfy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/goatveanb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gwojhvdel.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gtmyabdfp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/goptjluky.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/ggmhljfru.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gsghgkhnu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gwglgnhds.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/ghncwadee.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gltljflbr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gqgjaadaq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gatyzgren.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gmiysdokf.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gjpundlnj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gafcypogr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzifzzszn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/garebemzu.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/grgzdxwbx.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gdqqkpvel.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvbdrjkat.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gwxukajxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/glzjqdhhs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmnixqqlp.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glyfthwxj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/garkozxnz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/goalskwja.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/glnolgzbb.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/grqfnayyr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/glwvofnaj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghdzdmxsv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gchfgkyss.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gupcnjekf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gyxotxylt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gfflpnwtd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdvnpopfz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gfhsfivsn.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gnpcsmpst.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpxdkjvse.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdzrvjuoy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gjymrehbm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gymdltwbr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gcrxsrfkm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlxslzw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/ggfftlgdq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfjiathzm.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gstgovhar.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gekoycbum.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/goxmmwqjg.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ginthvftw.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/grtbjxagr.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gpfrxnoxq.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gvbuibxyn.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/glbntrnlr.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gwuhlmphx.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gbrqblgry.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gdadxwzhl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gyncvprhv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmmxqeedv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gopxtccmu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ggttmbxdi.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gyymdcyky.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gtivrhdbl.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/giwcqkjpw.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/goianlxri.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gdaiveyar.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gbrcxlhrm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/geuyagedj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/guoibcnzp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gexfxdugo.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gytantmor.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gplohhctn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/guqicysim.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gkjhhedsi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gqpkpqqjx.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwldvytqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/guuxnfijf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gcakbeuct.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gyqepeptr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ggblwqzdh.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnjfhlaae.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/ghmwemozb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gjuntiojd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gvaasklgx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ggimsnowo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/giqwvywys.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwvekyv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gylbupsum.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gugxctpnx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gduqjkjmc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gmbumlfiy.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gagorjmcw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/glynxlpgt.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gysfttefb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gvqaeeqfx.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gxcpjakaz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gzhkacown.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpqpwnrfl.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gurtbsugm.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gavwxjaot.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gmvzpgfjj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gbttmyctv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfeibji.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gkjfatbig.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghunfpeku.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gzayakdpy.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzxhtddtz.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gzgcwyvlu.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gtxnqyrlc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/grycldgmu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gtjdhljxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gctolhyzx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gfgzgiztb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gzldtwrkw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gzhfujwgt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gkdmcfckn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gnrfgdsoi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvnsliepg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gixfejybi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/givmepshe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/glpgvuoka.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/ggnrmrpza.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gxjfmjnve.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqytebvs.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gqumrghfc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gfgehrser.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggcssjden.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/ggtzljqla.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gntrghiiu.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gwxvvskjb.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/genttasod.sHtML


<!-- 参考信息 -->