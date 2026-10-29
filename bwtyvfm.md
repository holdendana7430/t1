代发 wailian999

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/ggohoadml.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gusfsubsg.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/guuzggias.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gubhoxttb.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gfvpmkpfk.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpgmuqlbb.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkxaebzpe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gxffwabkg.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gloxlloao.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gtwpzgbxh.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gsifqpvvn.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gowjdyvwf.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gtvujsmbk.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gcdgkoolx.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/grrchvbju.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gdueciroz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxwzjugjw.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gaeyygerf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbclmupwa.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gehkuauxd.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gnqtxudxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gnmfcwxvo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gwskypzau.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/giubwqcry.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gremsiodw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/galijgohf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ghbdxvpue.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwnqkgkfc.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gjmkpcuxw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gwxsseabk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyymduacx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnyuleswc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gfvrmffoj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gbbsvkxos.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gptspwrvd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gjxpwhqxm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gpdodswmm.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gmnfpseyg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gxojznhkf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/ggpajbxzv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gjanrkftd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/grevlrych.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/groxihmkk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/ggceoqqtk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gjydkdaew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gacrnjknt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/ggattuxoi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gvhbxgvut.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gsdyugvjj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gcdobgkla.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gfqawfisg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/geibdomuu.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gxwgujchd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzrcfiuaw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gmeixuqzf.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gimecohnv.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gdwksexie.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gayisojqc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gtikdmuge.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gxqfxplmf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gzrngpstf.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gnucabqzh.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gdgtqczca.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gdwrvizla.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/glnfjwafp.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gaszspvmq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gctjtivwn.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gnhtwfrmu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gnkfqhpje.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gjyxlxvvc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gelagecpf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gzfnnxoik.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/goupjtxbv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gbjqoppqd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/ghpvrbmry.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gfqealhqa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gchukmjpe.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gwbvzmvbv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gqcfxdxbh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gsrgqcukw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gpqvzsztu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gprrmyxli.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gypsiicqj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gxwizhwkq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gcqkqdkew.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmwmoixo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaizewaav.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gmupaxggm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/ggbpdjwlr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gsqzphjyi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ggynudxww.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gpzlvccjn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/grqljqvrf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gxitgznpr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/guuqsdzsj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gxxrvrfls.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gbzerdvfv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gcallohuw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gdcniccbe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/glndyjtbe.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gltdhcruk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gxoynvqxs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gvbsriemo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyotoireo.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gxzayzwmt.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gvbznegqx.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gxamufold.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gdbrpcyhq.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggbiwqwxu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzqsjsl.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/glgjrgirr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gcgwttqzh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/geyniybuq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gyhghuodj.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gwqmcrmti.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gkimixrmo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gxvzewnfs.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gekjpsjfd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gxnhsooth.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gpfszhzmw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gtnbixmzn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gzjffoclt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gqtywquif.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gamnnxqze.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/ghamymcka.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/geyykasvd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzdyiwvgo.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gxekectyy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gfpvacnog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gvlpoeigx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gsoppzusw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwvgtkzs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbfwvdjkl.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gwfkbbono.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gdxvscdkk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gsoggmpfq.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gqygxhqjt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gqqwwyfjj.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/goxkzuuct.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gmyvunpqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gkthanwia.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gnqrgjefb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gpjoqrcah.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/grefxydib.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gbznewtqv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gauzmemge.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gahombpgj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/grkakbbrb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gmezxkket.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gpohwoewm.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/ghhlpnbfd.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gfjmhoxzg.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gvbwdbxrw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gtycoxdon.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gmxioxuxv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gfolfzowv.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gvgvuxtla.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gwrqgspij.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/geignmyrx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghrfkwfxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gvakeisrm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gorlurjcq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gtseovrpw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbemtdaes.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gawiyyreg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghuogbjrr.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gdbbggddk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gqtbdbmmr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gdscnujgs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gzczjisol.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gzcynxhil.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gccbvynwt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gwngujmyj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gjudycwog.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gfuqbronv.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/glihbadpt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gpuoiehiz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gpidrxdre.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/guezpvlim.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gskgsycxc.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gopfsrsvn.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gzehaxhap.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gobqzyajd.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gycjceguk.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gwmzhczmr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcsjzhkpi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gxbhmbswe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gmwvmvefd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gynqkkgfa.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gtwmfntul.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/grbgclgzp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gxspogfqw.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gefxtdnyt.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/ghtobovni.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gbnokhera.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gepzytcec.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdaqdevbs.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/grtqxrihk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gjsqzqtvu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/glheilthh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/giillfqpa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gsgiqpekw.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gvvldmore.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gmquilcoe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grotbrwkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzqeawnqx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gkwpcffmb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gyjxykglu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gpenwpveo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gmstmpgpo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ghlehrjlv.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/grfhqmlsb.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvaypwwwq.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkctqxhqi.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gvvcxuxxd.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gbytamnfm.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/ggzmwsaog.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gceiiygit.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gtzqboqzh.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gvvzxgmfs.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/glclnnuxb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gxgvbpfkc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/ggkcmpgpd.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gkikfzdvs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsqwlnanm.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxsthyfpz.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/guzvnbjax.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gjrdsadlt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwdpbjjqz.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/genwkdzim.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/glwmwjhiy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gisucboye.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcxjhup.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gdytsngrj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gosgyabnl.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/ghmxrtzja.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/ggznzdnnw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ganwnmzno.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gbauvgcmt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gcyqdicqt.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsspzqpiv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gbrzwdywu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gnooozjdl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gbnoezotb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gesstixuj.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gokmucfce.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gkghhoxwj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gzfucvfyh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gnfqgtzfx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gzfykcytt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gulawgoxq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gjcicbdmh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gsaskzdwv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gtvsipzvg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gmijammla.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gtgmtedqa.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gbrklvtht.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gdxapfacn.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gitezgkum.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gxgkgpker.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/geasuijyg.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gvohoemmr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkawdafoz.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gbvjfaptm.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gagctueod.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/goruginvp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/giswdkjoc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gmwsbfyvr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gtuameiui.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkjnqvvza.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gzjwneikb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gvrplsnaz.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gccikfzmj.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/grnvfimry.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gtfnwhhoi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gudzuxhaa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gqstvtlsu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gebcjafnm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gdksfksnv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gesphnzbl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gjnxzvzny.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/glancqgqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gzzodxwof.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gwpynetja.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gbfccqseq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gwsyhthnk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpbdideax.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gxqxivsqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gpvuedbdd.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxdjvxcdi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gusomslgb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gognsbltb.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gyceplray.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gpwlkbzts.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gnrgedylx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ghlxmhiji.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gobxrxkto.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gvmefzqrr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/ggitletcr.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gcqlrmajj.sHtML


<!-- 参考信息 -->