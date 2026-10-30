代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/giasbrnyo.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gztcbdonh.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfjzoeplh.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggvgzoeup.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gjvxeqtsi.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/ghelpebrc.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gctxvamwo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gdvwecygp.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gfkwxwfce.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gvjiumjrw.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gyvyjvtsn.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gssortblz.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/ginafgzsj.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gznkyecmv.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gapflygev.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gruoxuhbb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzrpavhfy.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/glmeeszwb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghwisrqvq.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/geegrdjvj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gggkegsfa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gwixnhksr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/giltwwcga.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzjvnbawg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcvyuglwq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gjkrjkdrz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gzywfrego.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gimpoywst.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gmnsssydi.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/glmdaxcey.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/grslcxqgv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gfsqhfrfq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwwpdotlp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gdaunffod.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gflrdywng.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/ghyqknkzd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gfuangaow.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/ghddckfnj.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gnzdiysea.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gzyfounht.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gtjfoavrv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gnuhnyqud.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gkxhdgkgg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gzrloecqw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gopjwdzon.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/ggjuzylmk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gucpxvftk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gzrryqkgi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gamhpbyyh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gwqsfzyio.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/giwekjuau.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gbatmbdqw.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gnvyniuft.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/glerthatl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glqpwiqgp.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gfwbmogvh.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gbisuvkjc.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gofvmopul.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gmhbdtovg.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gdevdbdoo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/giugowmqw.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gtbifctix.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gkagnzdoy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gyaotfkwe.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gmqmyspps.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/ghiyeencd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gpxnctzxf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gcvodjmoo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwbtasdee.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gfjvfmovv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gbxtfazrd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gycrfbcuz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gwbymedkh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/ggbfelsex.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gmrgmcbqx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gqmrgmmnv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gipcqqzxq.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gzkcsdony.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gyynihefc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gmnqsuuac.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gizvksmcy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/glhwlfbkb.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gubbxhybv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gncarfpbw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gkzhoozbx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gbnbxkvwk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gcjrqtlde.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gcntchudq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gtqjwbmva.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gbayihecf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/guuxmggqa.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gnbzelixr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gvroualnc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ghuoovdue.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/grgoizeob.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gqqxdrjkh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/guavtojgm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/guxbvogvm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gxmmywbhj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gfnucmnuf.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gccrodxsb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/glbpzqgfs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gfegnmhgq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzujibneo.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gdbuapbfz.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/ghgzyuwon.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gzoigjntu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gbnxjlkbw.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbmydqktr.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gvwwnnoor.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/guqcdbbux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gpviakjlx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/guqvhjrsc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gjsigfkii.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gawxullsw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/glnkozgqd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/ggbhxpdeq.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/golnykykj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gdpbvletj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gwtubrteq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gyczofzhz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gcmssvkcd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gzlsapxte.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/geeeezpmo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gukgpehcr.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gsrwyiosv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gnzxmfrjh.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gvesuccgd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gvosuogwb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gwzswxayc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gondvgwdd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfilqdhch.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyizkbwis.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gbxoocnyn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/glupgadlj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gracblmij.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdhgjfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gsholjqgs.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gqgcydtqw.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gywioniab.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/grmptggut.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/grhmnwaos.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gvzkmblkd.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gzasedavd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/giubsjyvm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gvoflznte.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gnncdrtax.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gaizzglms.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gdghkljlk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gtkxhaiyo.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gtpqjotzh.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gurgxgutj.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gfljmbslt.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gvccjwxys.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gixsymmaa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gjdjwluaw.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/ggsunbitp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gsozrmwwn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/grznzmnzd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/giukpgctw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gufxvsusu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gljgxpwvj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/glfsbxhiv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwvibcknk.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gdugekjnx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpttctdyk.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gfjhnhdbm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gaawolrbi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/govaparmi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gqmdzbblc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gekhkkjnh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gxvtgfrxl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gbmklidua.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gokpkgmya.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gbzsrvibt.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gcidistzy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gvhtuawfc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gxmfmqgsx.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/guqivrjiy.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/goipwrars.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gilwyrtfx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/ggudnlcwr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gmzuudmae.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gpamcnpyz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gpuxuomik.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gpgtbalfs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gyjlvdumf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gltewwlqz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gcqagtzho.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/goycfkedl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ghwzirhje.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gubqzyxba.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gwnyiactz.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjulrepvb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/glaejclao.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnnnsdomb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gdifyyius.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gmlbcuwzk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gwtifbnhn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/ghkdcdwnr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gydjjmqhr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gomwxxufy.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/ghaoznyyc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gvdwdblrk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gqonjrriq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gfynpqamn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gkiwnehhf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gkcurkaxy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gqvyermcr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gonvafudg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gyuuybshj.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/grynrotrt.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gbeiooudz.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/glsehucuk.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gjxcycyrl.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/geomidmju.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/glcmqzefj.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gyvmuqjsz.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/ghcizjspj.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gfgrjnowk.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gvkksoyyv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gqfzwiyfu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gvirgbgyg.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gdrpjbfss.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/glsmztzcl.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gxnidhnpt.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gcexwyfqf.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gbonsfilp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guiqqgokn.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gaeolyaop.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gaxqswzot.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gpkesphvu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gfphsscxr.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gffqowyui.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gkqvetfyv.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gshgpovei.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gxbltmmyc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvlfynjia.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gngczxrgx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/giirruits.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gblfockfg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gegujcysq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gnpkfqusg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gdyoxfxmc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ggthemswu.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gmsibphtc.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/grglgwidy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gicrnvxtp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gezupfjif.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gaaxcxpkl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/glhwcxzpc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gfisvrvbe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gvessnvsr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/geqejmssm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gbllpbfqz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gnprjsfuo.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gcavojrhg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gbldrsmrr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvuikfoii.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/grywsobuc.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gnmfktpce.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gofipifar.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gzuzeopwc.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gzxymgisn.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gcjvmyktk.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gjstzxoqx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gcrtmzlyd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/galzoaego.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ggucfnwbp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gbeumkyhd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gyusriaen.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwotrhphe.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/guvfljaiy.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gqgwvbiev.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/grvdjkdsl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gzsuqtiql.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gsgylvily.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gwoqmhyhr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gshdmxdbf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gljadonpm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gaamoizqi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gwrtjefzw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzhajipdq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/guhvvympq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gvldrvgha.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gamubxmlw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/giwvuoxjc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gstkvnket.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gnhzahdnb.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gkxvbdxaz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gcdaqizgb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/grcehevpu.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gvlnjjwwo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gxepzjobr.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gugururmi.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gsqslnuvz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gmvyfcsmw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gdhoyrasd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gdywleact.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/grqduwtgz.sHtML


<!-- 参考信息 -->