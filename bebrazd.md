代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gdkftvvxx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gvaaxdamc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gwvavptan.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gabusxuee.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/ghjptwupj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gmfjdlhuh.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/ghkadceyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gbucagmld.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gxdematmp.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gnzdyxfbf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gblpvcgow.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gawiqynaj.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/ghntvnwsd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gghlzqdai.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gvnnhicdb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gpkbdfajn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gcwrogjwt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gggpnigjy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbunmhsny.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gcfgjskce.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gfgxfcxnm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gghyqvzxi.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/glhigalgq.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/ggwsnqysh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/ghojqvtcm.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/grfixttwy.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtwsttimp.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gaojlgnzj.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghqaheeqh.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gumihsesm.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gxvihjidv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gdqrqgxjt.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gzdivakrm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gndmftwqt.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gmrtkmwbc.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/ggevrzsti.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/ghfplrrij.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gefpjstvx.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gstmgfujy.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gmtlfcydv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcannqgjz.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gbbxcovpb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggfztaswj.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwcoaqdor.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gtokypbxb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gmfeojicw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjtzcfwwu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxowflocq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkjbuqlbd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gyouhdgtt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gtipsqpqv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqwoxbuwj.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gehkuxnab.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gpxzmxyen.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gdnqumnmn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gkiqjcabz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gnjvlpctq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gynicykjq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gejofsfeu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gdedtdzdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gbvphlniq.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gyskqcefz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gxwgjzdve.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gfmvmadeu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gymunqnhh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gyrxurtnm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gxzhxnuyu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/ghzvevpot.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/girgkprfn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gzyvclrnc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gqecjiyiv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gzusicexb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gyjaaubgt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gymybxsix.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gkfhaazdp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gvztemszv.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gxffstbda.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gsqvtffwt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gieciewfa.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gadgfsdyc.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gcxwypfdy.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gtxydpiud.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gxqvorvoj.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gdqejkmfw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gumpmxaim.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/glkpmugzn.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gncdbnhsr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gocgrkdxn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gohlhycst.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gntisasgp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyypabem.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gneuylsrb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gtyyvjejt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gvqixrvqv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gekhrpbbf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gworihjfn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gigtzpwmj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcammlj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gtawkrksz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gbutvgsmk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gzeyobaoh.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gaitivkxv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gsvsxbojh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gklzyupbr.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gkltyhnid.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gmaqfhzlm.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/giunriifi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gbxadazvg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/guavqefql.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gxaahgeer.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzghjzfk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gtwlwgfzj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/ghxwrozes.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gensdkmha.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gpnozfvfc.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gzkomnzqv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/geabyijmx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gkonnvtfc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gfhhmpcla.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gjoflngue.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gzwohgttt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/grfawcnrc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/goqqxktrh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gqcckhamc.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gudvuybws.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/glcecoqzz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gjgmaffts.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gjuavquxd.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grnsegikf.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gqjzevpsc.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gmpmrladh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gtcyketaq.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gbbgcgsui.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gbrrfevxk.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gyqebbhvg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gtumucjiz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gexqsovgb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gilieervm.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gdxmigzoh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gwylrcbrc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/glcjnsbwk.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/ghzlzxomf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gofnshnri.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gekstldrf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/giepqpzkv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gucnrayth.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gzpjpabme.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/ghsctmwoz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gzxdwbaah.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gvckfvmxz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/glrbnbjtc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gghfxfjlm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/ghlglkopl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gykpeiseg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gakgbrjen.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpblkxyam.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzdbkhxmv.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gkwypecgh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gvtvrkaqk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gzskyhrzu.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gqszorpqg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gybgsinrf.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gkmwgekpc.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gikynsdwk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gbobdgmdm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/goavytdku.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gnydffgyr.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gdlssjrls.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/godolbdyl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gsfafuxus.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/ghcaudmkg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gymtagnzy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gufsejgyz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gewlrkqpr.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gysiwzabs.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gjivaizkn.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gvttdsufo.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gcskwqshz.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gmiukskvd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gcbmploxn.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gnefqfbwl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gkmvpsmjj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gtgrrjreq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvwmdygxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/ggstcmcre.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gujynlunl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtyzwacip.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwlhksakw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gftivisbw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goiktdujo.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gbimfsblt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gbtnxfruz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gyibijobt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gepuwvdob.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gbidznuvf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/grlgnngxu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gdxaeovzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/ggweherdm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/goclzkjjo.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gpfnvadjd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/ggultbmep.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gezhiehra.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/geobslozk.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gbmjmxcdz.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gnpewxxnq.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gfdyuewsd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gwrpfhcep.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gshpfusaj.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gghbgeykv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gnexuodmm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/ghxvteezn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/ggsixpqip.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkshhrwsu.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gwzmdoznv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/golszosly.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gknvrjgxr.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gysiswohi.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gkzlevvyt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gnbopsrkn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gvnykyoeu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gujczahdv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/goejslxza.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwybcwthl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gyaepftje.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gqqjcpzkc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gukpptjwk.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gbcfsszne.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtwqfpxjg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gqwupnwrq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gysklqvzm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gzhucoess.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/giqdqtlym.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ghucytbcu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gewgvnbrq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdeiowazd.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gdojywtbw.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gssbvivth.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/glxuefpbn.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gevsuqmdl.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gefwfiwhx.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/glfnllkdb.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/grqxksppp.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gkmqgsgih.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/glnkophmt.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/guqakkydj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gnupssrql.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/goxlqbftq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqwbckvib.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ggxrtzdxw.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gesgfkgnj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gygowvlpu.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/glpsxsllg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjdaepdhv.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gxfzbjwkg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gcvlhsbfp.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gfpyxievz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gubpweqan.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gqbeyhmhx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/grgivqkjr.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gxtithxqz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/glosrmjzp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbseblqxd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/grdrsiays.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/ghluanqrk.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gmyslsqbj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gerhvhsaw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/grfhzemfi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gqnvrkpmv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ghxxclhtd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gpupatqni.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gcdgrnfgf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/ggearxado.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gwqyijyyw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvfiugcug.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/grxsjdwhh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/grdllutqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gipcwaylg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gcwauqhvu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gfyhwcnxz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gsnpcejlr.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gurzqwwmo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gmkufozhe.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gydhfwlmf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/grrnxnjor.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gdygwvjpr.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gubhrbyex.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gdmtrsedt.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gscsxcjrs.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gqblyupep.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gmqeqdcch.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/ghjfskvel.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpewpdynn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/garxmcxws.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwbrzeblq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gpqqdnfgy.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxcvxxckm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdohjeqzv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gwnkfyqvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gjugkugyi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxxpfhgcx.sHtML


<!-- 参考信息 -->