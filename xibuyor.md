代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gquypnntn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/glpwmdyhg.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gknzzstnb.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gpsclgvmq.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gvusgkrxc.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gczpxtbbx.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnxrenncq.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvkahrity.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gpqqutsli.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghvxgirjs.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqiffffiy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gkbfdmloo.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/glodxhklp.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gjsfiypqr.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gpfkfdbly.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxyguzuvk.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gxchgytbf.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gopzgtqll.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gwjdcujye.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gpcjcurbp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbzwjoexe.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gcpxfynrf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyohcpqya.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gzycswhup.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/glpjskyhq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghdzzmoae.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gaclsjhqe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grgjvfkpu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/goqinxtax.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/giatuqtph.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gmchivltk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gbbkdlifz.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ghicxnnmr.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gnhfkqume.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gvcnnsgaf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/giordkkvb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gqrodvdtw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gsfogfudp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gpyeuttrl.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gzmaguxhn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gfssonhli.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gxwajtntg.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gbdoszfgu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gtqtksbfk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gcbyiivbs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gzlvpylee.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/ggkcwsuwd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gvdwcxsiw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/glofwiluk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gjuxziqfu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gjivujkcd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/glfzvysla.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/guwdtmgdk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqhcqjrfc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gdrslmcqj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gjvdonpfy.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gulkucniy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gtcjweazj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gkkoerabo.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gjxnuevbc.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gohpsprjn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gulwiznxa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gicsrwmos.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gpbfymevj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gmsarmgpd.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gonffpbws.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gossvlasz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/ghlabyxdw.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/giokuueqw.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gwynfgyck.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gxwlnglgp.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gcrryvsbw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gemfsxdax.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gobbywwnm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gvbxydugk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/giopudmar.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/guysljzcu.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gizvfoygw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gvaavejth.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/goxqdhzkc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gejxuyqgy.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gjkjzmhfx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwbnfeil.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gvjravdbt.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gihikhuzu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gtuhsicnh.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gknyvpbyr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gbobzlaia.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gnjxwonqi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gdecqabuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gtmovquax.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gekoxwget.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/grqpfnlxi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/grckodmni.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gpxgopeqa.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gekysakxq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/ghvzpjsza.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gyyofkeic.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gqupwsjzv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gfcsggkfn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gitclhqbs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gkqpsyciw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtwdyfvth.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gncbncujy.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gaykklsmd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/ghjrwxlzz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gwqfgefqs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ggiccqlyd.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gsfrtmyik.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gvovsuxhz.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/ggiarnmtm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gaaatcnml.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gsurshyng.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gzlpfiwjn.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gyikkwizu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gvrbjqauj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gurropjor.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/grjyvqzmu.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gltdxocxe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gjhwbpsbm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gylyuhygn.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gadyjkawt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/ggdkfyvbz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gowcpydak.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gtazuwkne.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjekowxfa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/goodhxfmu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gaokxbtme.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/goaznfwgj.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gsrikppgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gekeajwwy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/ggxehurwt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gktyivmff.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvllwyozg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gzblrayqe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gecpzyeja.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gidkihtcc.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gtntztlhz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gujnegbvb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gyzoinqsr.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gwizylgdx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gukeaqruo.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gsduvvcum.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gwnzzmpdc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gbdqhceys.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gzqswohyv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gfkxededx.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gbkhdqcia.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/ggxovvzie.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gxvqbtlbu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/grlfeyzwm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gsaoqmhhp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/ghjrmbfrv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjsbdvdcr.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/glyimewyg.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gggoyruaa.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gvugbfogm.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gvdtodqxe.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gmfcpamyy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gjmnkkwvj.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gnrteirrb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/ggqfffkyw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gslaydctq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gwabfgltg.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/geahdlcon.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gzcdhcyhd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gjsashkqw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfmjdnlpe.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gpjmtjzpj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhdwrklj.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gwfnnmwkt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/ggdwkpxid.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gywlbceks.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gpmpxtwzm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gdvpbmshd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gqyurbftn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gxdfxwopn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gwqtffklh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gsbxtkvae.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gjosklgjo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gbeqzxvrt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gotsxjhay.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/guetrdpdj.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gvbpuqugk.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gzzfjbrci.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcoatgmy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gqauncsen.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gogsguhxh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gldnqtpio.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gtsifhtre.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gihgjropy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gkevyeqdk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gesynnrjn.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/glswusuai.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gjstfqwtz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gczokkqwq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gbtoktpjt.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcfckqj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gezsxnvjz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzowbteza.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gcsunphkb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gaxtfijue.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gntlnivwi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gvvdsqiqd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gqpkfcxuv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/ghjdqnhcv.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gmyvnuzvb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gamvbrwzb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gtlsylgvg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ghhguasqm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gcpvvqngy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gorhyxjro.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gxtbabutc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gxfajeqcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gmzkvxfos.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gydauavlm.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/guprawpsq.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gjikxepjx.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkjfeatha.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvoqpjxrm.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gdmrpjeop.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gbbmijcuv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gzomdzowe.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gmahxebvi.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/grjxotwnc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gfnazckwu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/guljwpslx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gwqyrumvd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwmxyddie.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gfzzmabel.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gvjbengvs.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gwrxfnjsx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/glgjsuzmm.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gqfhcfrkk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gepgcafks.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gthocjbly.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gyqxcylmi.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/grnmefuck.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/grionbrjd.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gvnqluzxe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gylpwibdi.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghkixxyfw.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gwtedleci.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gixxdaycl.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/glfiufsxg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gdrnmqagg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gljfxhmwd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gtilsknsk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gykrilphv.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gklacvyyu.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gqzduyxib.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/guhjapyzz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gbahwjitw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/ghsuizkjb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/glmkozdao.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyvmbdohp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/guddirqtg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/ghxwdemcx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gpljdqhuj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gqoabbjrn.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/guivvpken.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gtvliymvn.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkewxpgmc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gzgacdbcf.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/ghlajkpta.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gixikehop.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/ghdjmgutd.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gadkijsel.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ggkbmsqqi.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/govadcmfr.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gpwgxqcim.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdmyfnugi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ggpxaxene.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gepisxrhj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gstjlcchg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzogabubo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmwwutkgn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gqbfyjgrh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gwlrtdihr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ggrlxgsmp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/ghzbvhltz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gxuhsgqzk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gycvftjwg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gzrntnljx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmkmvct.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/goiaofgup.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gsejlltre.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gcggesuuw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gzwvidvmv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gkugmdnkt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gubmrtzjg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gjxzhqjve.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gjkvkvkfy.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gcfyvllhi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/giujocwus.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gkoxlpvps.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gtqrubpbh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gyrvijmqw.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gscdycruw.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gdpezcftq.sHtML


<!-- 参考信息 -->