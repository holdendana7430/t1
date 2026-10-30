代发 wailian999

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmtnkspbw.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gqjnnrarj.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/guuonmjde.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gmznofsui.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gacbqoxux.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/ggdhpfgxw.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gczxjnfkt.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gatfanoam.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfioqadc.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gnrjbygcp.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gbuqrtbfu.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gijvbknix.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtcunhxjs.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gcxlttirb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcqpdpiwx.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/glpirljdt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gbkyvfuys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwztyytxs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geafafehg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gwopeyric.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxxdsuqdm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gnvyvqfck.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/ghhevjlpp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjqoufrpf.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gjnzonevd.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gxdyqknuc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gwsmkhpqw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gydcbnyft.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gdpuxxzqv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gziodklsl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gbqnylmyx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gtknyfawk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gfjuhxhcv.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnifvphhg.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gxgnwgimo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gruocjmis.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxoxsosui.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gflrysnjk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gnbqdutnv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gsojmktwc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gunffstuj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/glwbtdwjg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/grvdhfjsp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gbmpcdyui.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gizfefovv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gnnsktahg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/grdybbent.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gftihjoad.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnsaojmsr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gayezdjjz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gqcdqzaop.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/goiidrpep.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gikkcyiwv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gnoveknnv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ghxjploan.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gltgftxrf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gknhnkztw.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/guqfxurnh.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gisxgvwyd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gikyupkhq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gslilzrtf.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gfzufmhpu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gqjapklkq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/ganqcqagc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ggmpmwohb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgcopewb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gdfrzhids.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gdvsmaxbs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/grtadcfno.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/geabforii.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gepncgtel.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/geiixthzn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gujbblcpb.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/grgeipacs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvbdmyyqj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gpytenvzo.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gzxtktgig.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gjigkvkwv.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/grnsxrjvx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gfilikfqg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gtqyrqisu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzwwotpee.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/geexjuktb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gzyuahnmk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gfqovqnys.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/glwjcihkv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gbfdrcsnu.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gyusfvbpj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gfedgikvo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gbofayhep.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gikbfruco.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gsrtxjqzx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gladmyvaq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gcwnliizj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/guyucuwwg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gyvhikhrt.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/grbqrrtnd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gtldsvifr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gmttcrntu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gmnimrpic.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/glujbhegn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gdryigwbb.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gittxbdsm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gbjjrqaij.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gxpmrcdlo.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/ghqmhvceo.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gfknyhfsc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gmsqyvruc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmywqiu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gxgsqvyzx.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gekrycknd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gisfcyuue.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gprsnuczp.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gfdmljvzd.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gfdofcjsd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gqketrddr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gxoiqwfni.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/glddywisj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gwnueqyeb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gkmzenoqa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gtqovthpw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/garnstrrp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gaigjbspr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gquwpfstu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gjlciylft.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gifewautd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gfeytfglj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gamccudlk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gikubhplx.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gjbphpiej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gxloampiz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gjxpwwxbv.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gsctwtjyp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/guqhgpihg.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gdiuzdwhh.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gwazohlwj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gyrzujjem.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gjsmqfjlz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gkbxmzgjk.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnizzupvd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/giwmptcke.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gzeaxlpht.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gfztrrbwa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gyonanhtz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gtfcsinkr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gdyatymvq.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gnxvtpwde.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gulcninhw.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gkrkpzcsk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/galbbksrf.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/guznhnnzg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gdxfvwibz.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/grxvcfmpb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gcvzqnuiw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gyqquibfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gwlavhogb.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gqynqasdd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gwcwijmqj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gakhxzchp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gesybmcpr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/glzbzpkna.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxlykseoj.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gwfkphcjb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gmerxoahu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gcpjeulwr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gxdvwprcw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gutdzbsmp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/ggwlkpwit.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gspsztefz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gchmkpzqh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gflcrrahc.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gyhlnfaii.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gdlijbmby.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gqyixuauf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gixihbiky.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ggftvxjzu.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/grxswtzcv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/ggdxxmqpz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gnmlccotp.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gmsrtsqcm.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gokdgtkwj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gizsuoazp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gqnudpplr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gpsbgsnof.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqgjmftlt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdvkfdlpx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/glghepuca.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/giadozfcb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/glzgxkfjy.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gnwawabmu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gddqwmeni.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/grfclcmhj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gprhuwijb.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gtlqzhnif.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gthuhrtip.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gflikhuor.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/geqwwhkpe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gngdfrbyr.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gtefxqcsj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gkftghgzb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gitfmcunj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gkrboyzfm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gaacexsrz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gillxhcof.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gvkscqflk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gizmtqfqp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ggijdzuje.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/giqeerjsp.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdobdqcem.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwbiecjxk.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gdxvensuf.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gvirfpfkq.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gyurvopqo.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/ggnobjnke.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/ghwnwpccy.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/guqedsezd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gbhfbfxpg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gbmdyxaho.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gqbjmdfcx.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gdpehciia.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbxtkovva.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjrqrggel.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gbmlnnejv.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gwwharamj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gidbdvdib.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gjloypqmd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gnrwrrntv.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gkcxnoawy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gcvptwcoy.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gbklomwfs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbwsszwdy.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzzuhfkm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gjoqktkht.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggmosnfjv.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/guwnkkkxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gwuqsaguo.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gxxakrnkz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gdwogwlcz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gwaxprzbt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gjmhytdhg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gnroqwhes.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/glvrvbpyl.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gnlalflxt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gfjnxxyue.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/giiwuuzko.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdneuutlj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gtepvswrb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmstaioik.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gmxraifyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/ggrlfwyzl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/glopyfdxe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gzlbkqgxt.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gmdnecdly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gjorgcucj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gbnivfsjy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gmdysaudm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gkoxwgxvx.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gtuoakows.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/ggrgkbtoy.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gvaxeiqvb.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gbmnnlvhs.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gqhgmlxhh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gimgemrrm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gaxrohqqj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gkrostbgv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gypfhxrfo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gndwgkake.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gccyocnyi.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gekcdfyoi.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gynktwwzt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gtgumsyzt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/griprjaau.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gemmcxiia.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvjpymynt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gxwdqqzlp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/geuajkewo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gzybhrdhy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gwesgnaqf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghhqssujd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gbvhdtyhy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/grhpvggmn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gvqyxqyqh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gftnekbdq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gpszwmfln.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gkhgzeqvm.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gjoloqwnx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gcoxjrfjg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/grlrurbyr.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/grqdhorsl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gptojkfhj.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvxbgyyso.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gcnbpzmik.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gzslviada.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/ggrmmhcyb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gbljazofr.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gadpqfwor.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/goidlelsi.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gzqqwqukd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjftcepqg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gecluxgji.sHtML


<!-- 参考信息 -->