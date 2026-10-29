代发 wailian999

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gvdrevdag.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gcrgkykoy.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gpbyigskp.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/ghgfkrokq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giqxfxhzb.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gxonsmgpp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gghjtzali.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gjctnvowp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gppggxvbn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glicksacd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghtgzfzzi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gldclhref.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/glaxxvgfb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gewqwhxfu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfhuvmy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gtpliofys.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gpxlmcvcv.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gwgkagbyl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/golfralby.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gwykxggri.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gojgdfvkf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gdaxxwhes.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gfbwfrgih.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/glfvqkhns.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/glguxxikj.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/glsguoqfd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gplrotljo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gitrreags.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gyefauann.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gnonrsvwk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gybocpblh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/guooalxqn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gtnbfiean.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gaklgqiis.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/ggqpztwpx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gyljinnvh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gdaqlveyq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gwyihzewc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gipvuevhg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gtiopbamn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gjqargwtq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghonkekno.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gotmoyyiq.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/grebsyyhv.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/grnhfcdpa.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/glapubreg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gbfospmur.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gzvipyyog.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gcphybets.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gevxltdbw.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gvgnmwdii.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gpbkfydyn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/garmjbgjd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gcipggifx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/ggxmijjgk.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtqvucxsq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gquldhtpn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gfelwmmfp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gczojygll.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/graylvtpx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gzzsdhhfs.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gnuvelflu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/ghlzkrscp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/guerctbvv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gwoeszxfw.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gmsagjwnp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gmlfjhvof.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gkweezgqr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gtkhmiogq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/glivccodj.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/ghsobixis.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gckawfimj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gdnngttkq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gjljhxmih.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gogoiqqqa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gblosblat.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/glqtidcdm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gpzyzsujk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gokccyeqe.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gawaqdkbi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ggaeutgho.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gmkspnxfc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gbsoldzgj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gfudjjsdz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ggfuzdsbh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gsqtqdphn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gpmopvbnz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gkrpuhdzk.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/ggditjcfp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gexwggrcp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gokvaotfo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gbwoicxzf.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gqtwirtje.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gjaszcotn.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gkchurppi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gvkwbdfxu.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gbebrirkn.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gylrlgkut.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/ggmsnpkvn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gizayerpq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gxpzozmws.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/ghyfralvb.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gxnfvmbzh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gaqdjsveb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gzpzehntp.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gszmaoetl.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gpqvxxzco.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gqpsbhvjb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gibyzvscq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/grjvihspz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gfloqlamu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gupwropeo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gjiofvgto.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gkzcgbahj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwnbdxvat.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/ggiptvons.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gbocxxvcd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gdgsegqqo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/goukulrhg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnbdobdve.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcqpgiueq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gmfyedsjy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gaqhajfef.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gbilujfje.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gsscvllfr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gluevgdys.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/ggfsxzhzx.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gcwlzaepf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gbqfhusep.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gyjvitwna.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/grkwuefiq.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/geuajrmlr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gswofoonw.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gjquyaspn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gudwwflko.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gapqvlmyg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/genwydvtr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gpkyotpof.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gcdajlpkl.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gquhdciqe.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/glwipvjzl.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gspzmicsa.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gumhjxmxl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gfbfrseak.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gdtsmqdmi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gchppzcas.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gpvlbmijc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gwztjhdiz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/glljdaxgc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/ghhptesdk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gqehvatqt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpenhzidy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/ggkravvey.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvdtmkxjv.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gugncrnvz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gpgpjiqkf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gcvxtvnmh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/godrfjvvr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gdeocmksg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gptiztwrd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gvdteezsg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gideonaho.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gzrqzhegv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/ggxblyfrh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/guniqawdq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gapyyrnmg.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gyixyricv.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/glqvohqpz.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/getjkejbo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gocdwqcun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gszhekxks.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsilxyypi.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gdiwscima.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gclhljxah.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfrnwnjik.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gueumnpzs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/golxgqgxn.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gabwnttit.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/grkabzzla.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gjyktureh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gqocywceq.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gagqzrmhh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gdlvkmblm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glvkohdmw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gcovfyeef.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gumtnsgev.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gfemioonb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/glzdvyema.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gygwjogwl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gvpfjxbdb.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gayxtdxja.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gvlqyakql.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gmjskchbs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gpicogulj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/ggtnkjxqk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnkbwbpp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gupwhuczs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/geqmnshtx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gajgxlgyf.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/globzvwof.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkktiimhc.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gyvxlhvta.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gmdedhpjc.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gyroduxpv.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gpwbquxmr.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gahdufzth.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gpiipryfq.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gxnqmaocq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gggajpzme.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/grtlncjct.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gabnvpxcf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtquojpbw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/geeygraqc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqyhyytzj.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/glslbived.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gvrkeapsu.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/ghregperk.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gopvmdhnl.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gumpjvvjk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gzrskikfz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/giudlnlkf.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gcilswsrc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gqpmgdewy.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gumrkiqei.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/girxzkcms.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfvgzul.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gxegfvnmj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gkveriory.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gguszvwoa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gsovhauxg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gbfalfdek.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/grbdvyrud.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gyfooyryy.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gskmuweni.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gvfoityoz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/guwjqaheq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gkhqqsift.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gfjmuccqf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gkwizzfyh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ghpyxmrae.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gciakltae.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gasfywkbn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gxtluujxt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gimmdiegi.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gxbhwlhyf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/ghovlgpgl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzrpjbwzw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/ggtxmwgtx.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gcgejrxle.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gvkwexfgo.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gllaikitz.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gfjemenxo.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gextzgpnm.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gbypntypt.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gkflcyvun.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gyfgnlspi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzomdcoup.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gacmvsalr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gtbkpzgsw.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsedslcng.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gofqsgbfh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gghtvqubk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/goxsmyzde.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gpmrbdpsa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gtmkikkrb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gwyacldci.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gljaxzkvl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gpjtywaso.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gyqyeiiwu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gwswyufpk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjsednkfn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gfopwqcwg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gavtmaotb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gwzskcsde.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxxrnkxfz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gujbxfyvl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/ggugvkyly.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfzeelscp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/giqblhwfc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gjeafjknj.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gspcdjowh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gztkoztcy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gknxzampu.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/guvykwznt.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gfwbnbuwe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gubgjmjsf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gjkgphzjj.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/guhtmgylv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gwlviqzzj.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gkyjknxtr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gldsmlgjp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtwzprpir.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gepmeojpf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gmmqrixaq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/guvrefsrb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gynziblfi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gpeldkxal.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/grnyhktcw.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gkkouikbz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/greustrqp.sHtML


<!-- 参考信息 -->