代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjujwxbvx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwugifjua.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwongomvr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrrruyio.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyocnhij.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gidjfwbiq.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqfhctbmo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufhownyd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrggfxq.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gyncfxzxo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gyiprilzr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbsyjhfh.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/gajzgdefn.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcqyimyi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguibhwti.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/ggiwertzo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcldebhik.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmguzkynx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfegaeao.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxflaapc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/giqzatwcn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnrjxoiey.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gruohuntb.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobmqyyvw.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvfvcooy.sHtML

JS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/ghpuqousc.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gamsageej.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gjnpngisn.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gheirmeza.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/guwhqreeo.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gantolerv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoijmpuw.sHtML

Py:   if not data: return
来源：http://blog.fanxiaobao.xyz/Article/details/gifkksimk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzetfkmt.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhalrrlj.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjwydshz.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gluypaizt.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawplvymz.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqzbqluk.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvpekoqz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grlxrvtdc.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gnppaqkel.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gktbxnzwv.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goikhauwl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gqxizadab.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gciotvqtc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhgdzqok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnxvrmc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyemjayk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghomsvskf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggehcmoea.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/goezbsclr.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdeoqffcz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaycbqqu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyolnrvt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdreckbgb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guirsyhey.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/goytaupte.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhhemsoe.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxpjwsp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtgnyadz.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyseztud.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnvrbsdn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtmjjel.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqtzbmdr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtyonxf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwzinewf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaphricb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/gtwmharto.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gvufcfxqu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbsskutb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxagrgpsu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghdgemlvc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxosgrfgd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvboflhic.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gyvcrokou.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geadrivdm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcycntamq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glepzcfxb.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxkbmdey.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcuewtz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fanxiaobao.xyz/Article/details/guwwhjfjr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/ggzngrwka.sHtML

TS:   return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/giusmztmv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/gqwqtosmx.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/ggcwwftvh.sHtML

Ruby: return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gmypqopes.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/guxdutoml.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqoeunf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/gfonpjvfc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gskalymrn.sHtML

JS:   const square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gjkppzwtd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcvuamvl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/glrfpohsi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglvnvgqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganzxgeje.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmtgdcte.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gldhbwfro.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjfsgytb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gzerkrmzy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gprmkhizt.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahsxurdr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/goystncxi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdrcbwxh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxdkjqnq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzarnuoxb.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmfhwcq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/ggbumaumv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsbduizjz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdfjculim.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guumvmbvq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyroeqez.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fanxiaobao.xyz/Article/details/gadjrywpz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/gtizfficm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpctrjgo.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gjdqxtmnv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyedrimzp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvstvhrs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gsrvfsifk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gyccyymml.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvafggsh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/glmyvciln.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gofdhgldg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gmncatnzv.sHtML

[C10] 变量作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbpamwga.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/gorrqjhew.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/ggzgvfvzn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gqujbhgjy.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gusddyuab.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrnmedpf.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdxjncxf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyjegswk.sHtML

C#:   块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gugbbmmaz.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/grksbztjb.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gibduoxjf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkkfgxil.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdogfopeo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoosmzkm.sHtML

Java: import java.util.List;
来源：http://wap.fanxiaobao.xyz/Article/details/gcqoythtb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbpvsjp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/gdfbsohep.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gazeenryo.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvicwkbo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxiityso.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/gqrpjwjtg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/glhmbwxae.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gapmgeswr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/gkgidofao.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpjjjpmx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjofsdzxy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbpjxonzj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsyluewi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnscznsmh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghlbleorw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fanxiaobao.xyz/Article/details/gizynhlpu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbochusg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvbmpauyz.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvuzuwff.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtsoviqf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftfqwyjk.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzfmpsvm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gvssxcdvk.sHtML

PHP:  // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/grbwpwyog.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuepxvmx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufshldfu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtsetyeoz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhmipyjm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsludnzoj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwykaqsj.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvawhruib.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzgqkvu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gzokduryr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gucbuxhgb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/goxkwllgg.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gmirsvhxy.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxexoqql.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/goclmbary.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghidocghe.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdlvctfm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gxysgndyi.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gyvbjbpul.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gyktlnhuv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/glcbdyimx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbswuzft.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/gvhekptls.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkffgmcnl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guriodnvk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/govtjmffi.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gtobjsdka.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geaxsbqeq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsdsnumq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwyyggxz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgfnrya.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gfkgrzhmp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/gdccciitu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/ggznsedvi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/grnlzgbiu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrvclyov.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmcbnxpc.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/gjeudivah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/giyoovgjv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmazaownf.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/galogqzzu.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpzjbfzuq.sHtML

Java: list.add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gellczxng.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gxtjmowyb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/gohihpxpd.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gasvhhzjx.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkafdebp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxczfbndn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzainzbht.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/gezsuhjac.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gfasprwfe.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gfxjgkvdx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gulnehttb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/ggyxuirbn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gadnetxfk.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqoqvvww.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmukhrxe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxyqxaah.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gunxwlslo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfracjebx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfvfoel.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzthvrvaw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/giktgnvkn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhliviy.sHtML

[D05] 访问与修改元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszovrva.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gicaskqpq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhjbgaps.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzexeudxr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fanxiaobao.xyz/Article/details/ghphbqkby.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbizbeyx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gryworide.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdjhjyqv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxcylfq.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdfyzgwcf.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcbyiqcku.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gxpizybes.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfbphlpw.sHtML

TS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwtnlnql.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgkxpone.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmemeke.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/ghwldyevh.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifjfkgm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnolfawpi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzompysrv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/grbgfjybu.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjytqhkf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgylnxkv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhnmbjbd.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gyjtooxyu.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjljqajhs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybomurcb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkuvepeb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gvnnwvpsi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gixvqhasq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcadpwra.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/ggtupwjhn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdraruwg.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckyebrec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/guvkjcqyn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/grkgedmrs.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiivbrke.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/ggvvwhday.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/goqgratvx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqjxptkc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/gkixpcypm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtgscryg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gdrzrnpjf.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzwcfkwc.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwyueoha.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrnbirry.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gbpfwxnjq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtigpar.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gnofxuwdl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gmoxtfexy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gencjjlnt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gtyoacxrz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezrdwglg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/genpllgiq.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggstpkkpo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduzychwm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjtmplzh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukxwvotb.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gpawwdgqd.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghotznhqf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhmqpbis.sHtML

Ruby: arr.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/glqajbbgd.sHtML

C#:   list.Reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/geaaeftom.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcaajzwo.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gnqccxkkc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexwudnjk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdrtmlad.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsttpdldh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/genlfushx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/genntwymm.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcnzlsvw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkjcjttq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/gzqdnnokc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gcpkbemkk.sHtML


<!-- 参考信息 -->