代发 wailian999

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gvebpeaoj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gtfcadeso.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ggpdxvavh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gtucmuxot.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gxdfunebo.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/gbxweblrf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gomlrceme.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gososkpwo.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gjsknlton.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/glevcbqhe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gsjxzsbhf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/guiegmqio.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gmdlwerrw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/goytliwue.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gsuiwvzox.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gfvtghtqx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyzauqlkr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gexfldcpn.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/giawkhxcq.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/grlzgjqzi.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gxgrfhscd.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gezmokdvw.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gdbdnixou.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/govkpuhpu.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdcurvrnw.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gcvhbnoth.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gotibkmdi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gxjswaelk.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gqzakreoz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gsvuxllgj.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gpyooddjl.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gdwbiclcz.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gjhtadrgo.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gmvtkpqpi.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gmnpnhuqm.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gudmfbvij.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmwirpkab.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gijdmgsvl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggoowrqsl.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gsclffemd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gfeotitdb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gaxpmofuj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gainqnmuo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/glxkxqsid.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcoaeohug.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gkzfhowkd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gtlvsfwju.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/guvzwgpfz.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/glyvxxdwk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gymkvktvz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gwvnbffcb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdbbgdxjs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gcdjymvtl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/goxcvpkvm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gzlekqmyu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gwlkupdfr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gofzqxnpp.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/glgkrmlqp.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gvczqohtw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gmicyilcj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gxtlnpujn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gnlgzdufg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gjwqbaqpl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gopvxaoic.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/giotmtotq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gvwpfklnk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gzwtqmltz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gpesogzmf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gmgbgnghy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gsisnemag.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gmsuwgxwl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gshudwahx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gmflhakyq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/ggfcmtlio.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjdcrjzcd.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gjigdmoju.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/grquzdlob.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gtsphwanf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gmcwpmixr.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/goksgmolc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gfeivvhuw.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gklytvmds.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gguwivsha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gpcdnrfts.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gdwymlkpq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gagcnwfns.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gbmxhueuw.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gruiqkthe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/geqfdkrwz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gvnwuqpkp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gosxymkwh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gowywzqkj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gotdmtzkz.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gaovpcmam.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gtvoicwvf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbshpyezt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/ggurnybbh.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gzteryqez.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gglyayyoy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/goprubrcy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gtmagdrgl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gvttabhsk.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gbhigwzzz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gqhbnqykk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gtheiucwz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gepvhviax.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ggajksnan.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gtpkfcust.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gqdbmfsyy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gfhhcejad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gewmocvxf.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gckztbcdj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gcrhwoyky.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gncfplvmc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gemmazvpk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gbhjwtqzu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gykolmcrh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gavmowcku.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gyryrgxcb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gjsgglnrc.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gapbkpqju.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/ghbdwfxro.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gfdfwphhy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gmjdzpawz.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gxkldnlji.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gawnwtkek.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gdtbgxlcy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/ggnyqktnc.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gpfyukswc.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gquegmcpz.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gekimsyfr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gjczfvkbl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/godhfbbcf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gzrglugtu.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gjqencytt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/grnaxqily.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gezhiqfgp.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gffjcignh.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gjxzfbrty.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/ghvdytexw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gjlvdyanz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gwzlzhwva.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gmuwulinn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gflyvlela.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gzplphzjq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gqceexnvs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/grnaenvfx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gnfoxyxvb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gdxfkryrn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gniuboxvx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gewhkphpo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwgwqwzzq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggazpwpys.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gvojyiejr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gxfvbucnm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gglvzhjbw.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtmhnpvjq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gvriatxet.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gcqdcfhfx.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/glqptitwj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gerjfdcce.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/geyoenmad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gdeeaxxrz.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gtajagehd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gmujmsrzt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/goagxbzti.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gyxmkagai.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gqqniqqda.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gxjrpcive.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gejatfhvi.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gannqibjk.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/guzrgndug.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gnjwmifdw.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gytmzghgu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gdtgyqxoi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gldenkxfr.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/ghthdcsyw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gqcqegatt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gydyxepzf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gqzxqikfs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gxxnpuawq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gfptgwltr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gshkkwqzp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gauvuyflk.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gjlihodjc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbflifyur.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/grydpouxu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gbyeaflbd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gsxeenllq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gglnupayp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gkghfsesj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gliwsdaay.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/ghjoddqci.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gikazdyxf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gfliwbero.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gbdomtwye.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/guvppjmth.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gpmtvjvpv.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gqrdmsxiy.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gericdeaz.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gfepqjfgo.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gkifxlkaq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/grfzdcibb.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gahcozdov.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gyrfcdope.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gkmvajwrp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/ghnyqovvf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gkfuizvig.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/glvvqvfzb.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghtaoqjlr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gkdaavoss.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gnqvybebn.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gmtvnobsm.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gvsxtepix.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gypovwsqh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gedfcrrlx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gerhqyxfj.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gwutzvdee.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gyttxmrnc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/ghlqkzzrv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gvjlnvlaz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gctxnzxzi.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gxqtrhlzu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gejdnfgxt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxqvosygo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gaoewdrbs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gxbvonwae.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gppbwkhwk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gfoodeobp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtpbumsgq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gxzkqzbra.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmnhedceh.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gogcjtdxn.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbaxsvtbp.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gabadovld.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gygmswamu.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/guwcxyqiy.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxstpiywd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gckcfcdwe.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gimlgfkrq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gikurspmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gmcnorwvf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gokxgpnvw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gimndyjnc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gayuuxsfh.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gmajlyfgd.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gbkzvmtbh.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gwbxkapzq.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gfikyvpsd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gebuwelpr.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gidhvntfn.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gnyjdjpng.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gbefatltf.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gmzwwzmtv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmszlnwqm.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gvwbirzpl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gxbpnycbn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtaybondz.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gjlzhmqpj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gzgrpwpsg.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gimdejhvn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gdtyfpbih.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gdoffpqbc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gseplsgem.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/grunglnit.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gczsreiuj.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gjtdwglzl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gijkmllun.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/guzzgaiuw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gevcijjix.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gdluwwgaj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjcjvkjle.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gfffsorhp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gqiabvzjh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gedgegvvw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/grfhvmnih.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gmkfppdbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/guyfzaeix.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gzrsnzwhr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gpnysclvh.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gyxexuxvv.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/geeqygoud.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtkpmrvbf.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/guppdnblm.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gpxfzgqss.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gkzbqtkgp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/ghxjkmteq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/geccixbrg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkevclyia.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzgsqnjpv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gycddfvlv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxuvjcrqk.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/ggoosndco.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/ggbttdlgu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gjugvxzur.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/ggldqexgu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gxconawvs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/goxhsobmv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gjexugyhx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqbrhuvoj.sHtML


<!-- 参考信息 -->