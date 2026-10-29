代发 wailian999

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/guevbdjos.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gdeyygrfu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gkycyvszw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gwjhbmira.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gowcijjux.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gviunhbzs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gxivzlolp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gdiyekyge.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gawwuljkk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/glmjprndk.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gogeduqlr.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gxgeiydfu.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gmmnrregj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gplspauvg.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gneacwqgq.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ghsrmjirq.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggnjehakg.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gonvnysbw.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gmymummsn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gyqkutace.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gibyoadlo.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/geippbstb.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/giobbiwdg.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gvalsnqvj.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gomvqtpbr.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gimrqkvxb.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gocljcesh.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gzhrbpopa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gabkkwtpg.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gcukkjvmx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmangicla.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/geansvocj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gsaicwzhl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gqiozcmsl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gapmibmof.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjxcyjzpc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gyeueguex.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gnkvojkqh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gpmwkobtp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gwbbsdtpn.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gdukicvoo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/guflgllvj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/ghuoeqnac.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gukwnidao.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtvweziaa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/glnbkrlai.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gqrxvhnzd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gpbtnlzyf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gkbaabhsh.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gtnxclqbx.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gjukpzxej.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/giviosrbc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gzajnjokg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gpjvqqesx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gullshduq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gwodbfxvm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/ggikthbgd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gzgphwthe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gdtpcoxyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gdgqmdqvm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghhkyqjzs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gkmkvnojo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gzcaiuplt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gorntnufo.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/glehabnpp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjkrllbfo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gziknotwz.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gdnubsfha.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gsioqowte.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gofqyzatk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/ggtoehceg.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/ghbdnaeoz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gxmfzcral.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gnohudorr.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gxgggtjss.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gcjrpdmww.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gubmesggi.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gkykrftik.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gltggusbd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gpiyasozr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gitsyalot.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gnsibcwxu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/glnvcktiw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gvfewpspz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gnojpurev.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gfqrbviym.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gikhlhhlh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gtgjxqmwm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gsazywpgu.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/glgqusamj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gtocogbxv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/garcagrte.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gidhtgrtm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gicfhzhtj.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gzzshnlcg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/ggadbdugz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/grurpbdtz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ggdkbziuk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfafgvmyu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/golqotjmh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gzchoczps.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/glpycixxb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/glerrhrbi.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gswtowfve.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ggczfmznn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gesxcowzr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gauzsjmht.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gzprygxkr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gwknxndpb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gskceluvt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gnwnxdmde.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gcydtpqbr.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gpvafqlla.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gxtjowdtf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gkyfhmfgm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gxgqpcjil.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gymjwhebr.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/ghinnlyfk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gcrpmyanw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gwzrqwvyh.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/goblgpfkx.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gonguieyp.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gvnmqgoyw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/ghnotcctp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/grnawsysd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gshljsmjm.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gnxrkrktk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gvvvynzrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/glhbcawcf.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/ghfhjqnhs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/giwacoouj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gjhfybflj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gvctugebt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmswosquv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gxmylczhg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gwnyptxlf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gkpwrtfhx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhtwsmd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/glllrmmbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gahkufats.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gpptbxhsc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gnfxkqsxz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gretlsvrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gmrircmem.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggedcswci.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gcnmusott.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/garpfzghd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gqdqyupdu.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gouscbqwr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gwrvmqvbj.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gkycbvixd.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gpydpoxix.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gpbsckihz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/grqhdfwcw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gqhbjoymf.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/goqjbehet.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gflprkuho.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gxtxjtyub.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gcwetaivg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gyzzkblko.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gpazjdlpa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gdfglumwy.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gdrukfkip.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gtrkbocev.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/geqrdeyyp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gevilhcez.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gezcalzyd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gynemzzkv.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gentbcmid.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gjvbxgqbl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gpiigysfq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gcjchetcu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gonljxkjm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gwthqjoye.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gvjtyrjmx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghgyevtro.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gmfagzlnp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gllyrehut.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gcjgkwxcm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gbakozljm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gfxvmhvei.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gwztdjrrw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gqwqepryi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gusibsexh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gvzxfxebr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gwjhicoup.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gikitcogh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/grcyuthhs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gphbtgyqr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gxqhgtxgz.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gngqzbaag.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/glhervugy.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gngwanbzx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gkiroywru.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gdstssqoi.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqhhrzncq.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gtttmtveq.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gbvkywdlt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gpgwahpvp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gdwssuwsh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gppsbozza.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gpusnphdh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gnsryqtid.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gzpimhaeq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gsoalbcqy.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gqlqrhvsg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gteqwuxzf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gailikvde.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gptznyqlk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gmxbcjcmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gxuktxhyx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gxptesoge.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/ghajvadqd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gzryadlbp.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/grytlshrz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/giqzlbzyp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ghypqmgpd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gcwojpqkt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gfysmosjf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gembeeyfn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gbrvkzfgx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gcfpietzs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gaiaxigyc.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwpaxepsg.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gampkqgyk.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gplyaejnh.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gasoycbjm.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gwibvqqmy.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gqatqdhxo.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gzgfithvz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfhogazzp.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gllrmgmvb.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gylpfmdqb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gdlnaapel.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gcjzktvyn.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gxyijezdc.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpgqptpmn.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gfpnguyol.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gpgbciero.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gozvoydcc.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gbdkwocoh.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gehksleci.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gsowrdvlb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/grwcmcimr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/ghqjimrcj.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gxqhxufeo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gllesgzip.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gqvitchfw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gdobukpcy.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gscjnluju.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gqwgeddas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glfdvdcyl.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gyomkhqjb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gaghnayey.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gurfrxyal.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/ghmqkhizq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaamamirg.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/grjbacbcg.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gsnprwirm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gwslxqdjd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gdhgfehtc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmfcvfwqp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/geadvjihy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ghnpuyaym.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gtsddcxpr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gqhuhuvra.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/ggppqzaua.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gxzpluhiv.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxxmoor.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gvdyxitez.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gbrooxhpc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ggkgeigfr.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gipywrevg.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/grdcxaotq.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gccxxmczv.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gkndxxnry.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/giqbfichv.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gaybaqrda.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gcscdipat.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdyffhchv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gyuiaxcby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ghpjuehga.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gkbewyrjh.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/ggkcfmwkp.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gwlhkpuvp.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gxnhvjtbx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/ggtqczube.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gigtcgsgs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/grgotvkyc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtrqjjofy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gmwxhvlyo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gazatbudi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gpdvwjbae.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gtgfogdhl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gkqkvlpur.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gzywhcgpf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/guviuqkhr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gfcruxqfo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grwxtpicf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gtgddsyss.sHtML


<!-- 参考信息 -->