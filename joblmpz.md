代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gmcyvrbwk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gdzcgsgjo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gobqitngp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbgfkbdu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gtftsfnep.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gnmafjtxg.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gnnpbmvlk.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gfcmcdfyc.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gjxytuzkj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzcbhjher.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grrrervri.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/godqsamel.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghbfuqxwv.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/goxidhboo.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glxphouez.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/guxwvmbiu.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gizlbgjgl.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gaynxmgky.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gwgffnuyu.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gwicrxzol.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gqnjyyser.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gurxoombd.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gixgfyacw.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gqnyrhqxf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goxoqgkfg.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzsgnnecw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnebflrqo.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gcfznyvop.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gswwnrslu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gevpaiziz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gffuovddm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/giiwimooo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gfoksramu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gohklrzlk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/ggdeysmgt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gdvueebkm.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/ggdobbntz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gneceqfqm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/grlnajzza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gklwdrgdd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/guwveqsby.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gxzedggpq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gvzsasqvn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/giwcyqdes.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gvchuymtv.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/ggzlipsry.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gfzklmhuh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gqjkrztas.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzivsdvk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gfotdvjkj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/glugbshbr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gstqupmsp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/grbvyfxxt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gplpxcmue.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gchisspre.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gwykdhpnx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gyzdmhsvx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gbktptxtz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gcvtwrbff.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gapjarmwn.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gqhpuxbsl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gyijjzjvq.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gcntpqhrt.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gjvnesygn.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gjoofoviz.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gylkoytrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gcekxqzqj.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gflqnexdf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gtkqbgbum.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/girbvoorc.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gzaticnes.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gvjgjaojq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gfoktrfob.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gendosqxb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/ggqcxfmna.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gwgwpjlau.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdwxwrgom.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gbvqfsgss.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gcyulugdu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gsnediokp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gjqomvgmu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gztridvqf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gluxlvjqb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gcpcsxuvh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/glbfpksce.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gshpsdntw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gvbkfxzpi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/ggwflemzx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gklgwuptc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gxczelurk.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gwkdxwfey.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/glnktskwc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gsqpqtjia.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbaytjyv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/glrztvnxa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gcdbkzkpp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/grlxmyzst.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gujmwmxdq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gaycetmqb.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/guarvokth.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gaasftyal.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gugvgzmno.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/glvhdtkdy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gpowidboy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gqmlkrsyy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gzvilinmq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/grnakcnta.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gvmydbwox.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvihzfpwp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/ggdovlzoy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gxhfukwsh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmfklqont.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gceasoqzl.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gvnurpetb.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gatfuxmbq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gvtewlirw.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gvixmfryq.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gkcafwohy.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gbrqqzwrn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gahgjlcua.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gyakwrmat.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gswsoxjjk.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gfquslcbd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/getefjqyd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gbcnfjxdf.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gpndzkgny.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gvaeabrgt.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gewwqlzvs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gbzjmzukn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gicurjcin.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gblrkkbev.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gyxwrgjqj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gswvvmwju.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gumzkzojw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gzdrjrnuy.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gdjaihgfu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gmezobuax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmkomgrji.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gywzssbrj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqkevvdyv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gipjhrcfq.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gmczlwixt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gfyckwalx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gmpsahhfp.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gcebzsqtd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gwrnfgqli.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gqaaxcrwz.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gjvsohyyb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gjdgbgoaw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gxmqogalu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gzjxuvsuh.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gpitvmbmx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gbfcfwirx.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gbwqthcbf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/goligutfx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gsjrmfkwq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/grkrtkdeq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gyttsnuwd.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/ggwjzzbbl.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/geptrcnoz.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/goiacrkyh.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/ggydcoysl.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gcawbjdvr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gjpcfhzpp.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/getkqwhjm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/grogiktfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gayvameei.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gfvpmovur.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gwyxjcmqa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gvgldjppb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gppvsbacr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwbxtsuyt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gtrhlvlym.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxygrivlw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/garvposdt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/ggzdabbvp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gyrjutnly.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/guvbugqrv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gubokhcoj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gdjusqnzw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gchzqpdum.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gsvnhciuw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gmunobprp.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/guyhxmxdp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gklhzvvrh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gjyvoyrsm.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gtpdyline.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gxhzrbpna.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/grdyvmvvp.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/grkpomizd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/ggdbhsnyp.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/ghygpsitm.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gumwyaovc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gruzecyue.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gzzudxfxl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gvdciuovq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gvbwqejrm.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfetugwyt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gvxkyjowa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ghnowdgjg.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gywlbgked.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghvzilnge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gpeefgcpc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gtjidrqwt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/glyuozzcp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/giichvkmw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gzhscrunl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/ggrrhhned.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gyivppihy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gxhjorafq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gvctayhll.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvqiumotc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gygyzdlcr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvaybkqvl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/guewmrkut.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gylmcbbwb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqkizglqq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gccnimwbl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gxcybhyuy.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gbbfkezbb.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gsxjmjota.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glxhggeyl.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggujgidjf.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gmxwodudc.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ggznwgvtz.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gbstihyab.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gbthlapde.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gtwcpglux.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gigxylamy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/ginsjwbvg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gubtlzyry.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gklznpdaw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ggffkkacl.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gocnhatib.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gjvcidyso.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gvuuysvqy.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/ggfejvgnc.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gmojacovf.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gdqkqbbty.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/ghucxkert.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gkelwuqmb.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gjrmtmftp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grvocezic.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gnehkyyhk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/ggvnbfgjy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkqwxatib.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gogmzxkar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gtucoagyi.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gdvivfmuw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gxijdezvr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gmsijzljp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gbatgfgaw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gukbjzepx.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gobpgauni.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gnmufdjyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gtskebofo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gdzfwjxsf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/grjfcvkca.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gcqaqihcj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/glqiopagi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/growugaiu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/ghbwfqlne.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gwtrdhiea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gemcmmbrz.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/grdcjwoxv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gaaeobadh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gnpfuvekq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gqlscbtnx.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gzuwsrdam.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gesqaskzs.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gnxpoovud.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gzhkiezyq.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gmjwpsjzr.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gmkddznli.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gmltwmyha.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gqxbogokq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwohflxeu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gjbkmstkd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gdtomnlkm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmeuuxyos.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gdewpjsgo.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/grstkukwr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gxaxjucjt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzkdsja.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grocmvira.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gizlxqgwd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/goayeqpat.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gfupmdrhb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gtasummju.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gghmfvrmc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpknhtmdm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/glcrzssbi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/ggyyqbvli.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvtayidsw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gxjbvmnmv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/giwdlzjgk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gmgbzqysg.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gxbutxrww.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gtwizuysz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gglsntovd.sHtML


<!-- 参考信息 -->