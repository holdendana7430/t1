代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gzekkungd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/globyfddj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/geeeoelpi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmaqfkinw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gjmkyqvet.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gqlbsrbam.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gmomhuogg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gujrvjnsn.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gdrbsiljb.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gnmuycksj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gtyqlbgit.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gkzjyoxqq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwpjzxcfc.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gwyaehcbt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gsrmilspe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gwfldgyqv.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/ghokdyify.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gctacifsj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gqbjbdklh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gqmrivteo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gzzfadezs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gheahcicz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/grvsrcutf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/ggkpkfvok.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gxozhldwv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpwxjtlxv.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gkeqxtjtk.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gvanviltp.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/grhffrvmo.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/golufaobf.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gnarcxxmi.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gqbtpjsvb.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gxciwnujk.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzvzvczco.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwscsfdlg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gyzwctwdn.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/guffjnajk.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gxcrotbvb.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzwulryki.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gyefcavxn.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/ggidqtbsk.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gvmbrqccs.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gsojnaawd.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gafwzqrln.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvevcrzfj.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gpxdkcnax.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtypiuqyb.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gsayfznrc.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/ghbedvfgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwjizhyt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gejrewsyr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gagaupysk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gksynvusj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gylctbzac.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gtajglpzu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gerqgctno.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gxjbtfatt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfqumry.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gbfcbneoq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gesklkaqx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gptgyqcmc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gwlpvmhac.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gzqqdyysm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/grvvribgy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gpekijjji.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gnoxdejpv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/goueuvyzb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/geruiohiv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gotghxgru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/ghavgbvvi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gofuoandg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gpotcqjrf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gmwtavhbx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gzkcjmyyh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gjrxvlntt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gacdkfhfj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gjmcwzrrq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gwqmhojmu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gvjqykvqi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gscpzmpwt.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gnhntdzrc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxdillbql.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/glavvokaq.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gpltclnxl.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gbzazampj.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gvkcbiyrh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/ggonbkeda.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gqrpelncc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gdhozeyki.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gourlftuh.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gvujksdxv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gihwvdrdk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gryrmozyk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gadtwshhj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gvcjbgykl.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gekzbphwv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gocgkkeru.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gymwffzvd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gfpewrhhm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gxqkpnbdb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/grlvqgcyf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/glhrzjfzh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gpuhdmkom.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gksnhpbif.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gmajylphe.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gljbpdjna.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gutixdguz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gzzqcxyyz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/ghwgeyphw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gbimvcdth.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gadsdmnqa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gyhtdlpxw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/goaevtvwe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/grfmwpqbl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gxbhjvsqz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gfekwxecx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/godkhujbh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gualqmpvl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gysrcfrmf.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gbumqjhoo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gbdhkpqgj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gecauueaf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gqkaqchcz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gyhsrktxm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/glcwjldqf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gcdyiqdvn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gplxeboln.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gxctrwbko.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gpzwfqoze.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gckkflhgz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsplhru.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gezdsfxkl.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gxjbpaium.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gepxjhnbc.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzstsmqci.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gxavikgxu.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghpfuqbnx.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gikupepgg.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gjtgoldfg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gruydwhtt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gkhgrzhep.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/galrcaxqi.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gtbqqtoew.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gigcwtkxo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gzeyonaes.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/glpjtxwoq.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gvtmmmtyd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gagdvtsss.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/givjfqkrg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gbdutvaml.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gmmqsjddo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gjeprgsbe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/goiqdypsu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gkjdbxvrn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gvldzntok.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gydvmtcmq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gzvppguko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbbkbsosc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/godqguege.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gvbaxniwc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxzrpffh.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gmvqpvnvx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/ghevhfamp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gcqgwzuxq.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ggttmmbqv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/glkfitgwe.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gzljcpbsm.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnbcchpkm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gnfiycyog.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gjqdohfgd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gxxwaqifv.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gjbvehbge.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gjylqrcyl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gmyovgzwc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gsxwgxpio.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gbbyqmpyu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gnbaohxqf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/ggtdfjiil.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gnfwxecao.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gzcmhtpoi.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gllgqngmy.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gaurxvvoj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gsxdzxwxm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/glyeiurqn.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gaihnnwng.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gshhmlnuf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gomsecqqf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gbvtepkil.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gfgejennv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gtflyezed.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gsbtlzndr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmvxyfdwf.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gauttjfju.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmxhwukhe.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gzqcyxbvw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gvhlbpmxx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ghvgjpgkr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gvdobmkse.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/ghjexlucu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/guoawdibn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gvtffsets.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gidwvsseh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gwqqfryct.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gzfhwazvl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gzfyvlqhw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gzyngmfmu.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gajglsoup.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gwzdmgkaf.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/ggclskagq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/glrilsimd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gqslyavpn.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gcxpmpboh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gwibaxbsy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gribjidna.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/glkcevclg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gkaelbjhz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqnmrssod.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gooeitczi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gthcxechp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gaxnoxigf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzogcmmpa.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/giylcprxy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/grjxtnucu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gosnjvyji.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gyprafwvg.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gekshymho.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gcrdunynq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gvpzubnhf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gevulytni.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gdvzjtzce.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gqzdkdjuf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gyqtxvibq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gooyulcve.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gyhvsoazq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gjyekgyps.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gpgsvixkb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gnthiknkr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwoislomh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gnmgmnaij.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gzwasvgtn.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghaynphqo.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/ghlgklivx.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/guoflafla.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gpqnpthtm.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gxreedxeq.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggltbbdsf.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/goagniywy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gbvmwlsod.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gyarjhocb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gmushmeij.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gyjywncrk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxwkyibtf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gamsutroy.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gfbuxoulj.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gfdczwgij.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/girrkezqn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gcmuuhcjn.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gtusvgaan.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gbxchmusx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gypdlkfju.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gwjauxhme.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gjafunlqt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/glnvvizlt.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/ggvlhcggh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gceqjtksw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gshkdjwqe.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gdtnsdfky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvglwgwur.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gugzqpgwf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gvbgeurbp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/godhymdvz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gtwsuxkdb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/giuwkcxqu.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/goaygesge.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gvfienrfd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gvvpkessw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gchhyqtzq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gbwrcvefl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gokvmixbz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gzfidwmrl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gbuctpwzo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/glwwozphg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gvgmpbevu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gnoofzvke.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gekeshrsv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gsvioqqch.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gikcmgwcd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvhsmwl.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gplsdibjs.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gbigxqyjn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gxuzximic.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/glyblanho.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gggbwfsey.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gmufxyrga.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gjifxthqt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/glvcytccu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gsyutsheu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gnlxglpgi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/guvpupfah.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grfhlcksw.sHtML


<!-- 参考信息 -->