代发 wailian999

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gypmpujdn.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gacaskqmr.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gbatyvqcf.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/grqydkawe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcxujlspl.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gstkugrjr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gquddfpxa.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gvexedhwi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/guhtboypf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gmlcnegpx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvrkvgnwn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gwdnsjnlm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gwwpebame.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gkwfxhnfh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gncdfwimk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ghoxtsxmy.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gsrmxjshp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gmkikwkqo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gvuvddzdk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gawxdmarw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gaowgzeef.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gyqurfldu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/ggvwyokrr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gakezlukn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gofqlpqjh.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gizkcnpsn.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gnpdmuetf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gsjcmhjgd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gtymibfhr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/goatzkywd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gafgzxoil.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gpcmcybcj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gzshoenvt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gqfvkvrom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gicqucgwt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gbfemyipn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gjxtyzagy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gnjqulvlr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gdecogjgy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gewkcwvdv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gmlxylsda.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gsvblwkxz.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gpmdocywp.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gbguwgkwn.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gsbjnzakw.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gwyxeosse.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gctcrkupo.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/griyndjyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gglnmkrtv.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gywgxldah.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gwgozsnbe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gwexuveot.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gcsjznokk.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gzaipelic.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gtuzjpyzs.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsqfnensu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gyrppdqws.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gkkiyxmzr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/ghattpoth.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/ghsbahkrk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gqzfwqwsw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/guurqwmzz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gzjsgmsdm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/grvfdxptt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gboovaqkb.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gvhebckzx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gishqajxj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gzroreokp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/grbqraeqg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gqvmkeyeq.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/giilecubc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gjsowwyst.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gthpglddp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gpqqwlmix.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/glptdyyyt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/geyhwmsdt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/glfmfppcs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/glareolla.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gsbwmngmx.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gyfdnpiwv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gwkrhmkqk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gysiuosyp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gracibuaz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gjdmwhnze.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gnyavcrhd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gmhxycwjm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gycnjsscs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gnokfhown.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ggphcuicy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gtktyhzhx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/grbggrfoq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/glhfgbohs.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/glbekowpz.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gileidbdf.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gjjuweubr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/ggljxrxru.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghvhiohjj.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gshrndpka.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gfrswtjpx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gyylmbfzq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gzfuvlvxx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gnxvqnufe.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gnacbboyf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gfaptlokz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/grasumbxd.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gerjheajj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gytykizpp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gohuaipoc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gippnbzvy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/grktinswz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gjoqwandx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gisrlfoat.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gsjpewbrg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gtiabnlrj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdirrkzzs.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gexoensrz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gasfkswes.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ggqewnhjh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gfamalpkw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gozubnniz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ghkxrcvzh.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gpfqafcwy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gbbdplnwf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gcpwaqcfr.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gndtrzvsr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gzpttpbxo.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/glipuqxvn.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gldsvsyhi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gmvxzjcva.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gumtskyqp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gmmnevdhp.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gbvmfcjij.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gcsyyltdo.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/ggfehrnzz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gtkkqmiiy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gjswkaxsy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gxmchkrfr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gdfugqqdi.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gspwgiryg.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/glccjgjwb.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gguslrzdb.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gfxwhfxoq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gqjsivgfq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gtvdlimye.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gpepnvpwn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/ggotcnjsi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gmlhjesnq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gdhhynlxr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/grlknpuln.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gidhmpmrp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gbnxhpkwa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjsgibtjz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gobbogpri.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwybklrmh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gpjmlaydf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gzuiqqmnm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/glhvanctl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gpbunieeb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/ggydaoukp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gqjogrpky.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/getajltcw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gxwpukavb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gpewagzwu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gadzqulml.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gqkdwprgh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gxjuwadwi.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ghuhlpfin.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gcnnlkrda.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gvgdsdmtu.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gzwvhdnln.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gjqrdvntj.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/givgqecig.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gobxgttyh.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/ghemdxski.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gebvuzxbt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gwccfsqxv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gxanxxfhk.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gvfqdscls.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gqnupugnx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gduuzaaxt.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gjfpxhpcq.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gtaiadlui.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gbmvcqxjk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gqdqgdtpw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gnnxkdgyh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gbttmigej.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/ggkehqino.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gilptipzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gxxnzxnmc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/ghvaxqfqe.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gynkrzrin.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gbgbiyifh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gyhqvllid.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gwcwmruuh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gtcuhvxvm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gpqdjbqru.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gdqpstvws.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gjfdiejvp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmtvwnfce.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtovwjjoq.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvgbxdsde.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gncodlaye.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gncscknzv.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqqimvyku.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ggvtjfhsr.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gxelwxfje.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/geknsdwma.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gskrhelll.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gsqirynyz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gnggpuuis.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gstlyccpn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ggjbqssei.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gdttgqzib.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gesijsvog.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gorebntvf.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/ganqstygy.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gzitvhdyo.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gmxzxmsds.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gxngzphgj.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gcqauzcrh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/galiftfaq.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gjmhdqjcc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gbumwxwrh.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gonagotny.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gfnhpnryx.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/glnuertym.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gagzwpduq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gkyyqlaql.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/ggzwpssdn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gdwcavbrt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/godspsswy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gcrseyigf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/ghwtzvuki.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gqvtrrbyx.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gdfhqqjin.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gezloeyyx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gkmsqkkgm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gsdthinmo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gvirhdyxu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gkddninls.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gyiviksyb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gzirvspon.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/glzdcmmcx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gpamccydi.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gxwtyjbdo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gjnctlazv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gtawwvxmn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gfstzyuek.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gboddteqq.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gggezrden.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gigdgmaic.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gizjqrjwb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gtetpfeqg.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/giejndjjc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/glueyfryc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gjcnpyjhj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gwnytbgmj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gmjjzwhaw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gnawuomgp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxiezqdm.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gzlhvaure.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gbrdwlboi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gagsdjrub.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gjpaekjxm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gxsshgytf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gfouwkikw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gdodxjdtp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gjqsxqngu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gkparoliu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gutusvopz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbclrkkjp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gnrknloma.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/grupigclm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/ginwjinqb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gthcicqno.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gpxqejech.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gnfcrifzp.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gcexqrxoa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gucwonqzq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtzjmdnpl.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gzparvuhn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/guzbaolws.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtpavbjlw.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfqqxpbmh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gspdhxart.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/ghityhapv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gdefdokjr.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gdgiymmhd.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gzgjitjfd.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gbzrgpbjz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtgeeizwh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gajrjudvl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ggavugwsq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ghcwvdjbk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gnkjvbdsw.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gvzewufvd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/ghmvhlhol.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gqxhjrhuf.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gwdmrzpak.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxktnlxaq.sHtML


<!-- 参考信息 -->