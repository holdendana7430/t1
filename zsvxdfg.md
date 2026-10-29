代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gwczdjkcy.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gcdyiuijb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gghgjkzhx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gfgocvwif.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gwvcpdzdf.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gllmcmygj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/genedbkda.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gvbptznfa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpqloyseb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gotjggwnk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gsvljfxln.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gbhgqcuao.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfiufhrhy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gaqjjonil.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/ghuelqhuk.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gxzhelwji.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/ghnzjwtfp.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gbltrgxah.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gletgyuwf.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/growlyvzm.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gtwmiutvt.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghjbdqawv.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/giohafamo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gvvazmwbt.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gtbjubdnd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gusyxnfox.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/grhcrpmul.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gbnbqqlsa.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gnemvkgjw.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gugnrvjwz.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gsbgtdkbd.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gwqcuxktt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glzchsnkj.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gkamxtvkq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grfjtkbcz.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ghqoxfpal.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gjlxcgjgq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxksfdoi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gcxutkmws.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfuexoipp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gaokxfwkg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrngtdm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/ghikwuacl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbmutvzrf.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gxknoljxs.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gdhrfvghq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gknnocwde.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpmkcqhli.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/geuhqkfxs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gcdxfmtyv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gfqwenwya.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gwklphxwd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gnpuviczt.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gnfgmrlps.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gjkjilsee.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gsuuujtpa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gydrgriyh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gaavnitar.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/grzsjlmrj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gliohcrci.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gztgdiair.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gpfbujktx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghradvykx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gkjvywpzr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gcfxweayb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gujjtlssm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gagxajlyh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gqrsaxavt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gnasicrrf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ghjswnzxw.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gabkamilm.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/ggorlbtzr.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gmmoffief.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gbgtbicol.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbldzilbq.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gawnowuuz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gwfozrptk.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/guloitgip.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gqkvovhez.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gvhyxkdxl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gldobpwdj.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gjbbnkftr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gkidccwbr.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gfctdcycm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/glsbdoqbs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gpcwuvngt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gfvrkptay.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gdierzjaj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/griuoprgy.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gyepzidga.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/ghjawomqd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gkzkobgbr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gdwioeinc.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gvcdqcowz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gbtdrvhfu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gygoqtjrs.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gsgthsqpu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gbhghxcac.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gpimpaeos.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gbjqltpfh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gsftcjosh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/giwikppxh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gbildytex.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/guaikyusw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gnhfqqmnh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/ghwvkygaf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/grctwrxlc.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gtzqelypi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gdexqsqvp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gceneqinb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/goyyvyeaj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gunafacha.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/glyseobvt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gbnsznmwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gmpymlzmd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gncjinhwr.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/grgfqzdfr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gsyjxdnpy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gutjybznt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gktibchqn.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gkpfvoplt.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gcgizwavb.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gswxegtom.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/goceypyzx.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gbnspworm.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gpygucfcj.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gsqgydwcn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gxxujrcqf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/glblxjybr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gbeiijsmq.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gjoxxowzs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/ghiexspwp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/garyuqolw.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gvfpmlbax.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gktgxyjna.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gydlcmgbx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gefpsswvq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gijpebfmj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gcthawigy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gcbcjmyun.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gsyvsnjfx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/glomkwsdq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/getqrwxcp.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gfzazpmls.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/grdbfkkfg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gvfcajfuu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gbypzjqcn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gnsivgnsn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glilrmekk.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gztrquprg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gcitghwcq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gclvplufq.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gvlpqinzw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gyhbplonw.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gyptayzeu.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gcgeofvfs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gdiuloyfm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gceadtqqy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gkfvfwhzk.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gwfpbvnny.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gzuuwcmls.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/glirfxnnw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gkdapuibu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gczqqiefl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/ghfgsoobl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gcltvhugt.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gpfjyxkoa.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gqovjjwdy.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/glcfxjdsv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/glvofneql.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/giulivivb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gjjmjryis.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/ggnqsdysc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gyldcqxmp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gonutyqab.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gnjyvfnjn.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/glbbafuvd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/ggnwxddoi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/ghulkujob.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjynmyciv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gyntftojz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gywlkqvdt.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gtxahwadr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gfsuyiwzo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gcoxdnoca.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gegsefagb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/giqqvlkjc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gzvhrhsep.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gwclgxyxh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gdfcdbjvj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gdmrvgtrv.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gimvdgpah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/geqlynjsu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gwnnmoxdn.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gkxubosop.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gyqvkboly.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gnzetwpvn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmdejyvxs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gvsrfngbu.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/glfvucwqu.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gnegrikmm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaeupvpxp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/giftatfnb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/ghhqcwxtk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfmbmayyn.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkrubywor.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gpcxfgbxw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gjspahuwk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdayekgvq.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/grtcqerpb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/guwugdtwl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gysraexzj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gxjwxsolq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsagfszyx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/grwrvpuaj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gperjxwaz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gipaqcbhk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gackgrnox.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gdtcxbvqy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/goxoaprou.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gqecarwde.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gdgtdduan.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gebhrwwsr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gbqsfqiic.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtclwolvm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gyrsgxjcj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwovsdmcy.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gvoshjsri.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gpcytyrcs.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gkcccjwjt.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gakeeuyyg.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gdjvzzvil.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gobqhpcfl.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ghecbvins.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/goafwzcsi.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gqljjvhis.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gxkbjkfwr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gakiowmas.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxbturtnn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gbpbslcss.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/glfsvdros.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gloxjpiiy.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gdqtnasue.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gctpkyvsp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnckgbhfo.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gizfhybrb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gxcegssuk.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gzhoawaij.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gbknbmpfj.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gebengarx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/grxkwcqwm.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/ghdasejep.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gvkikwkui.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gnniyiqjp.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gevgkcjuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gbyhogxxn.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/ggwdlencv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gjjhxcbyf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gxtbygelk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gywuiiahd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gzfrkpgfb.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gnabjhjnl.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/ggbuqcmon.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gyjgdrhhp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/ghkxkrrlv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gncjnhgin.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gdduejujw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/geulqqnrw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gtewjhxyv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gwtcallcn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gxnmukydi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gxkgybxan.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gsdkpxbzn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gvdayennk.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gselcuuja.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gzyvkexss.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gesbzluog.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gwsiixwmz.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gnqlzlbfh.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gsbaowabs.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/grghjhima.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gwzuzauci.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gfvutrohw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gthubnzjt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/grlhquqtr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gpttspexe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gugfnrive.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpdtzryw.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gsjrsxmlr.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gjoybshzt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gmngqfumv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gjzxujoce.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gsxigfide.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwevdasil.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gmsufcnth.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gsqpjscqq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gujpgdxwv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/ggftrbydg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gebjfbnyw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gyjiwcknd.sHtML


<!-- 参考信息 -->