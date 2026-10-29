代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/ggyzahwls.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/ggglzvjcb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gdiikmiih.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gprimecfr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/guotovtwh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gaecwrhkv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gicaycutf.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gytclfpkx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gnbxuskfb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gydnoeibj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gpxumigma.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gcbgwaxcn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ghyecjqrf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gpfmzrado.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gdfbjenyc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gngiahiyy.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gpdhhpncx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/glarewegw.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gtpuoqkbp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gqecegrnp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gorgxqhtp.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gmswjdrco.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/glxlvfuhs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gwyclrreu.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gdmtmpebu.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gsamnyjpj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gvtyxyewu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gdfkribuh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gswfrpkzc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/geypjkazv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gffwvaeya.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvuhhioxu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gkyuatqgo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gkhrppwyh.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gzmsbifer.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gztlbchnr.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/ghiuplsku.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gpkbrmmfl.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwcruslen.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggxjqvhqc.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gksrfaxob.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/goyolqcst.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfewhxvce.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gcdrpnsuc.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gkxnmzgfm.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gxcomfqzd.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gyvwpfnqq.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gpmovrgha.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/grlgmlqql.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gkyxydcpp.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/grifszosk.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gpdkjnlgs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghhyjkpbn.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gonnydjgi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glmnwomcg.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gqvlxakjg.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gqguqabqw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbseeknhm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxlsfdrif.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzkyupylt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gunxjwwbg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gbsyyeakc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gycjbvbln.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gndjklbwm.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gyywgzxwi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/greumoxkr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gezvavunu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gbqycxxkd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gvhzrlwgr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/ggllxrgst.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gkojsbbin.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/giaiohhzi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/glijlttli.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gmtnzults.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gozbofymn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/ggowbwfve.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gkdozueoa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gwrtlhssw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/grqkulkgu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gerfhkhrm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gvxdxngfc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gcvwphtvq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gxujcybaw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gufsljgtd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gorlfvzeb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gozylkgxu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/glvsskhxh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/ggjvrlgim.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/glmfesvly.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/govbewsnz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gzfpmplyx.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gcowghrsf.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gnabfglqx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/glhrouvcy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/giivquhrm.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmrvhezxv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gycwhdzsl.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gnqlgosvl.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/guftmqzei.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gkwibcljg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gcuraoeuh.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/ggunduebo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gepvqvrmr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gtzkknrdw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gchdjviyk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gepxjphtr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/guhevjxoh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gpyupyfgv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gtkmgkign.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gomihpgpq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gbyzujutv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gzzhmrdrl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gkqqqoqwq.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gimbfsysf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbalkqi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gahadyjle.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gavdangvz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gjywqyhrs.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gixhozdix.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gtconrsfc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/ggvvmxthd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gubrqcksv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gcjjluyrv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/golakbydx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gphcizzyx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gicmnlbyc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gvhrvxmpn.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gzvszysch.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfmllgipf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gplbrrcrz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gcclaqlqv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gzzidppld.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gusftbxxp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/govgjkavp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gbnewlsiy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gjkdiyhak.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gvhdornqr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gulqlvnho.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gvnunvtcc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gwubeupzo.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gvqvzittj.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gittcmfcw.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/glmfwdzwt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gjecwhesq.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gllkgmwre.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gwynsrowe.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gwypxshwk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gwkrmvsmg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gtzthgjhn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/ggagkgjen.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/ggflsjhyx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gtltikaig.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gjdghemuz.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gimjkgnjj.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gdopxsdyu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/giiiyokvt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gvspdesuv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/geknobzue.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gkvhdsspy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gvftwlrxq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gfomiiyyp.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/giwguxexd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gspimssny.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gavpboann.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gchplosxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvpuuicne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gpjdkpecv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfpphqcdc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcuhmzjbm.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gudzlwiwf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/grrejiajs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyxiqhptm.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gqhjailwz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gffpkziwv.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gnsptmkul.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gbgpjrvwo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gpypkuesd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gcxpaukwp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gigmqrfhh.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gizuzogjx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gruveijfp.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gkyuwomqo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gizbfains.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gipsvwczg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gczyqyczn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gdeqpslkz.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnwqcnryp.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/glyursjgf.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/ghcsuegqu.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gvmacjcyu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gyzmmpsql.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gqfhfwixt.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/ghvjwhlvl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gnuhwjadj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/grrsstlen.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/glebjiptd.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gqhhgtwoc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gjlaohdha.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gptpqcqfx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggthsrjwc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gpyjfupcp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnisvwluy.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gjoydzypg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gvbyhwaia.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/glmiadycf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/grtulqvem.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gwdrppbqd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gtztlvrpd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gfbbldsvg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gbradoxgu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gzcctnkil.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gwkmflxwk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gtjjkghfm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ghxjdwylw.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gegonbwob.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfouwbqvy.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gosirpkaf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/ggqorjlrs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gxzzyxdlh.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gfetovbwy.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gwvqkzjta.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gknlftfay.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gfkwxoqjm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gtmzumbzj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gbsnyrdmm.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfqukhmtb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/geuhoygcq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gvshxapnl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwtpayedy.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gdcihgkyq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gwrnishku.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gagdjaegg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gadolayac.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gmsdvpfmq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gybczajlc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gqtpnbhmh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gqqaanybs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ghlslarfy.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gqnixokgm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/grxstywgr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gccqqtiew.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gbejtssnu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gafugbqmr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gpjlfiavh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gsmhlpxhl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gxpkplgyo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gzjqiqttu.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gdequtors.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gwhlugplw.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/grecjgide.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gwjntkvxw.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gzsqhflum.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/ghpbaeshp.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gzcyomapo.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gxhfyjjqo.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gegpfmymb.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gdfjrhixr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gmgbhsyta.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gnympjhho.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gjwyzzcxx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ghzrbltxi.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gfhosxfrl.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gchcdpqkn.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gmixtxhdx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/ghdnldfin.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gjotbhitc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gvkdnvntz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/goiadfoyp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/ggohitugc.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gvdvdavyh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/govllaqpu.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gesjllixr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gsqkypwse.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/grnrruobi.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gtmciqzzu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjfjwgrfn.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/geqcyfipv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gyinklnhe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/glcaishhx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gocohehwu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gvzracvxc.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/grhxbcrly.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gswwpbmyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gvosipasj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gewoeuyez.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gbwodwbtz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gwskhjmuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gstmfpxcq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gvkhlfhoq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/giowmtvyf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/goqhgffct.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gsxpycxvu.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gsmxgzjms.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gjdxyfyjs.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsvfrqqpt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gkuhlkukt.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gkumstphq.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtsiphgqi.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gwqjqtuzs.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gotymrkcr.sHtML


<!-- 参考信息 -->