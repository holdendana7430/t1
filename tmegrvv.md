代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxduxgzm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnjnawwed.sHtML

[B15] 布尔运算与取反
来源：http://wap.fanxiaobao.xyz/Article/details/gtyubmxpm.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrgkcbfn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoblwyoc.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gkfdrrpjq.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbsoqlof.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gggtvepwo.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviajzzgf.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdnibzdq.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gixrojtsi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihrsfmrl.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkplllkl.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guwdredqv.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqadjbob.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbfqfgay.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gruahiiyi.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcwqvuhs.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrgmnbpm.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixqqvese.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbktpydsz.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gzenbbtbg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giimkpaad.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsbbdekr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/grtemgfpt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoipklvs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwpksnwsi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxqxbauk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqwsbpy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaglqwzbr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/giexpdfyx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ganapkxpg.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkqlidyve.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmkawsdn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeinltwk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbjpqvpyk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuhzmic.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gilegcxha.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/gttjiugzm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gedryezzd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlggjbpy.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdxtqvqmx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzklnvgj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmftchoqv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpcgfong.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkrxxzab.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvklgeehi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/grlckpkox.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvddeublf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvnhvwpn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdekfiott.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyqeakdu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/guwtscnqt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gimckkqob.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gfilxfgva.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/godqsuzki.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtirflzye.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxkpwekz.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwumquctn.sHtML

[C05] 返回多个值
来源：http://m.share.fanxiaobao.xyz/Article/details/gukgxgbqe.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbiqzcwb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gntnsulir.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccozztsv.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gemupsdoc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/gqjebhzly.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gfjnnqyra.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxsffkag.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfgenwqg.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxomupw.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gmkeistpu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhmgjzk.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrslztbd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqdqjqaa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsfxptwg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/galpikpxz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gwkleudxa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gyuwnsdad.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjwoxwee.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/grbzsfqsb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gyxibidcs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/glkkoupmq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaembzaex.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavagfgnp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/goixmqqis.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbucyvqh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbebapx.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhwuvxpv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gwqbkxxir.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gucebrkxr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggmzpltll.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbqjwfwha.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gpxmkmtux.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwklltkgf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fanxiaobao.xyz/Article/details/gogyeldwi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqtpfsdiu.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gkggrsvsw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqimornq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagtvvhdz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gxjnoneyx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gdpwhxojf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrdbtyam.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/groxjlumj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbecgrfb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/giajvqdsv.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gaokdpxzk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhwzwojs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxhdpcke.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gosojlwfs.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gbfrichiu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/geyqgadrg.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gvexomixs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzwydgiw.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkhgcpbt.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcgrjdmt.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuwbyzhs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcmkhkvc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpcibkd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gxdalsjbn.sHtML

Java: import java.util.List;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyebsoaoq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzsqhpeg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqidoos.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokpkween.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gbemnphdo.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fanxiaobao.xyz/Article/details/gfdjekdod.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyyqbxui.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gynfqabix.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gizbvtgzr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/gesvebubh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/grafhjhum.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fanxiaobao.xyz/Article/details/gzablmaxu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcocohgzs.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gotbjeauw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glanwqywu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpcfzsna.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fanxiaobao.xyz/Article/details/gayvmzrub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grvsconhr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grnbsmtxv.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/gacukposr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gotzfehsy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoslcmpv.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyabcwaia.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gbbfevors.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/grjpgpobs.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gomzpwlau.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaulrufcf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjjluzcxu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntnizrqv.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gbwvqfxbt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grboruwqi.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjnbcnex.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/glykmngwx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjawglsq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxqmvremd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvosbvdf.sHtML

Java: // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvfkixpp.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gzquzumph.sHtML

Ruby: a, b = pair
来源：http://3g.fanxiaobao.xyz/Article/details/gxzefjdzs.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggroaawsp.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fanxiaobao.xyz/Article/details/gdtbpwzde.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gsfmzzoiz.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gcurpmwie.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/grqhgzzwy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gkipixola.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmojdfdgc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvlnnvun.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinqloqp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdlcdeyw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gllfptgvv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfrttbxg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvynoajjf.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/glupdmzgp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlfamibt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/grhailolz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/ggmfsuguw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjamtlciv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gphmlkcjn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdszaomyn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/geykbpszs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfgvodb.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/gxxhwuonz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfcoseyn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtjflop.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyykvpzr.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gcogpdrdy.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gblivkncn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/glklohxdo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwuegyib.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqpqnckt.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjprqxdoj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfrfyphs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gemhzpcxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gyqzboemx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gusjjcmcd.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakcrcccb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntaqlkdv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/graexorah.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjljgbhjd.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsuumzpm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhrfmome.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaawojnz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiydtamk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guscpzcvm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjftccced.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gccvhfiza.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdlwduzs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjvpmxjsv.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbysqruhz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyjvacns.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjdhoojf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gomchvdtv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhkafnj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmqhqofj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gtrcjjmrf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumzmzdg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsuhetdp.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtffszwhl.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpvjpyf.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gsllorjuk.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmymhurje.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlewswqa.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/goehgtlhz.sHtML

Go:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmgqzswf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gygiyjnsr.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gzpfednkl.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlrvvwne.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gppothodz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpcpamxn.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gwocfsraz.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grsukumvs.sHtML

Java: list.subList(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gsxmerrnw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxslizyyq.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gejhaopqk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/geooujsxm.sHtML

[D08] 合并两个数组
来源：http://3g.fanxiaobao.xyz/Article/details/gdiuotrmo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlzuptpx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gecovixvi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fanxiaobao.xyz/Article/details/gygvnwtls.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvzxspea.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/grsivtzby.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbajzybi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzqxawlg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtupowpj.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkicvihnn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwltnibg.sHtML

PHP:  sort($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gxpnvelwm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcxcojlb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrjxbmzb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fanxiaobao.xyz/Article/details/gujxobmkc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdjkojqp.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjqlnarn.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gendkejtc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/gzgucdcdw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gddwetitn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gidjercwx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gqglhihzu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzvrlbtg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gkkymfjey.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmhypppl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gyevqpdwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/glnfkgovq.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gofarzrlk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkktsmnx.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gpayqtevs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goarctsuf.sHtML

TS:   [...arr].reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gwwvozxng.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtooweilj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgzbkdlb.sHtML

Ruby: arr.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/ghyqkrgyf.sHtML

C#:   list.Reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwcpnnsq.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/gjiubyqti.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeveqhav.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gqwrhpvcp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpgihutf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkglsccgo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gavtnbgrx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwndogikk.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqednvjnu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnmfhfws.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzbjmtx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gontgqgkv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkixqmjr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrgxsgfs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujtdrufb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/grmelvudf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fanxiaobao.xyz/Article/details/gredlzvac.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzinrqute.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/goubfkmgc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfjhgkqt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gifnloxfu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpwtzfdk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhgymdzm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/giznypoqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvcvpoedb.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcwgkiez.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gysxaksfb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gbnxghphn.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjawyrzv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gpthuqjgj.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gdshjdvon.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgkuvucl.sHtML


<!-- 参考信息 -->