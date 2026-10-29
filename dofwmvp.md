代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gqapoyobt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gnfeevoed.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gczatuzpt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gxojvealt.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gegrvjdgw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gxdeqsijf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/galicmxma.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggxyervcl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/glzbcdziz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gutkjozkp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gionyajor.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gcpwivekm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gppjgwsqr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gmlimitkw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/glvymqjvk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gqrjgbgjc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gngxsjvmp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gufehzpgd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gazgxfzna.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gokdxrsle.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gdblycevw.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/grtcebxiy.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/grrkvextj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gzpbldkjj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gihoyagzo.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gbwsgoezn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gafzhquwa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gcnwjunhf.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gzsklnzur.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/ghdhxudoo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/giaudfoli.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gyaoakuth.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gqggjhbym.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkflddrne.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ghjnibxxw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gynfzhrmu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gqmwxaglo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gujhjvmdx.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/ghfsewswy.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/givdycwvh.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gdbtuigvg.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gcwhohnxu.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gslqqdfpo.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gdklxrxtl.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ggvvgycdn.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gjjobbcbr.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwkgoubqo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gwgjmanrn.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gediapwid.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gsfflsqal.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjlhareq.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gvjhwdsot.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/ghbjfjivc.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gtdxjdchb.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gjaoedlvv.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gdxdgiizz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grqnfsqoz.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gotfjkfle.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glajerzaq.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gpglixlxj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gxmnucsil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvtqgelcw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gosuhdwme.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gpcvrdsvk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwtkynhpp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gcbizzgui.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/glhgjqkcl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaqlbayof.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gpodkdodl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gzoihyxts.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gwtmqlhhk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glphkiwfv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/geahtovcq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gcbojkhab.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwphynglj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gincefxxn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gswdtwlzi.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gubilcqbp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/ggayzmnoe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gpbyrchhh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/grsbbnblz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gkuiqdxrh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gwoghnjrn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gzaxmvizq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gxqlueojz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gndlsnhij.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gcaokptrm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gqbudxuev.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/ghszwygjx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gbyvvgssq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/goaqwhubv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gjdxzgfob.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/grhziyrxo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gotjcgedu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gixydjajr.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gracnwuoz.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gghsickdk.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gqiuqhmeq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/ggqskdzyk.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gcbweyydn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gcydpwxxw.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gmafwhyhv.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gdibvocpm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/guyixmkiy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gnqmnktuh.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gyvfnbffj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gbwpygsrr.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gmcmcavnb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gmuuajxdy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/grormgufj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gzhtjmmyw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/guxbtviuz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gxfldtzyl.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gzuakrjgq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gliijvutv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gdducouyf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gwjnthhml.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/grklwsots.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/ggzsfxdzq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gwvtbjlbi.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gxlcrvayw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gcsrgokzb.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gmnhfichc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gnxkpifwh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gdlljbtzx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gzlhzlwmg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gpnidgjae.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gedmqcrqq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gmeffickq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gnbaxpguf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gyfzyfqti.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gkjnzhokl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gszzpmsza.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gowsmfvoy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gmrleubiw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gxrzzjexl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gorthvoye.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gtpzqfryh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gvmuqzilo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gknloftjj.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/ggyntarfv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/ggdvwndlr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gsklsgcmm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gduqpyagn.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/glhaozswe.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/ghygeqxqb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmeysmxcu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gxfvysxsn.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/grjyhartg.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/galwzevom.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gfocohqcz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gfnmphres.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gyghaaiqt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gnyogqswc.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gjwccefgk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gqqqfjaow.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/grmnqqxjf.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gybytirql.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gofysnnwz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/grznoqcgu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gzgskwfzh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gozkgxquk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gyhbrtwgs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/giusqtmsn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gyrfvytrw.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gbnlhyqtg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/ghaesmsmu.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gegtdvxzq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/grasqwhpz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gezpmkegj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gqlmideed.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzlprbvwv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqaasyyvs.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gkrlozixy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gyonqoefv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gxpctipra.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gcrqtnikm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gvdrxmtsy.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/galknltat.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/ghypyunvj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gleruqnhx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gwplnajwv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gfpyoylmr.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gkvylldmv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gmznjhtex.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gxehyjdjj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gnuptgopy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gmqwxgxmb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/guttqsaib.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/ggcmfxnnx.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/ghacjzurv.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gholrzmxs.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gituuqbxu.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gdysegqpr.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gzkylngzc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gczwvshea.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gomryywwj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gxffeezdh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gtzrrbjtb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gxmgvuoag.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gjcinmkip.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gorsfppih.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/grhbfewgp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gohrjsxxw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gerwnaplj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goufxupfo.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/goeyeionr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/goktcvlbi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/ggpzrermg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gfawadflx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gilqygrwq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gclpevlzd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/guhxmuwfz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gfgpaxknb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gnwflryza.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gcmgrqeur.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gmaighfph.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gpfnhxvvn.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gxyxnywau.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gzwjgrtnv.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvushhwk.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gilgwyzsd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gyfjzmcsz.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gfvssucjk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gjwvlnabm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gvweauxgq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gkcufpshr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gblbhjded.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnasfcgjt.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gqjoswtor.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gouedyccm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gyhpubxri.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gxayeempn.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/grobwalrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyzwdkxcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gvonzofbz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gpxzqrjdv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gciosntju.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gxqepelxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gwssryetg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gionrtobh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gmraaczso.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpkuhlnms.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gwqifrwpi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gavocvxfp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gxzlwzxxp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/glsnfldcg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gxezfakkv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/guwgxgsar.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpxoctvhz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gagismaza.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/grfcqndax.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpxbnhlxn.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaohzeqgw.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gleokknza.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gpmhsjyxl.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gueoyozfx.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ggtttwmdu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gasgdcdmq.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gdeytxtzw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gyrstxsth.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gcbrdduyi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/guvqwjtkl.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gbqttxsfl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gotxyseja.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grtzlacnv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gylpfgypl.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gxeypytqs.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gfjhegnkn.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gekwfmemk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gajgjnzzp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gcwykdjgj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxouriu.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gtsmkwjrp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gsdlzotso.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/glflpokbp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/giikypvjb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gwmwatsth.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gwzajsavt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtaleiekm.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/grunpdnov.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gxbmymync.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/ggfmbekcf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gbqjgszkx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gpcuxbnnj.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/glvkcxgcy.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/grrvfatzo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gqzdgussk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/glbygmfpr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gpebpfmnb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gjsjcndpw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gtvbjcfjm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/guttpadfp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/guihbfqce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gsdmhfbft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ghcbypejz.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gdwoqirnc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gkkplgdfo.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gwbzvqpyv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gsmqmrrlt.sHtML


<!-- 参考信息 -->