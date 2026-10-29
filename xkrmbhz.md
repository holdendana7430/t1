代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/ggojeqpyl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gfuucmnxf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gczosptyg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gxjjpszsb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/glejpfsro.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gifhkozzn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gaatrzfay.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gupfuetyk.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gebohsajt.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gdmiswkix.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gqesxtxpz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/grurpnyro.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gijmggfmc.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gxqiuuilc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gmwrevtpf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/giqogdwvw.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gmufvtkfs.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gozfdnztz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gkkivqkvw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gagfjcjpy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gnjiprhst.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbifihzzw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/ghhvsvcfe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gndqaiwid.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gczfqkjjs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/garrwmyzf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gzhxuhdyw.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gnwurjyww.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/ghldvcsoe.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmowdxcjw.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/grzkvmspb.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpxcpnhqg.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gsoayuykd.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gesrxtgwz.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gizamcmbm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gsocsmndf.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gondwsagm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gxjcwdmfv.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gxsukjdvj.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gbtyufpgc.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gkcfzhdqa.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/glgxetkop.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gcbpwfzja.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gwjdtforo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goiffyjzr.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gbvlmugsl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gstqzosve.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gfqzyazdy.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gfnpmppcf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gosgveioa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gyhhsqchq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/grfdtfusd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gswcmnuky.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gaikurjen.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/ghmlbowsy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfdfzojqd.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gdeeotkry.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gzrmiolqx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/grjriltug.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gxxgiaeya.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbvtxuhhx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gjkxidfrg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/giiuqbaej.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/grzbumhef.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gjjpusoko.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/grtpljbtv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gfwdbjjty.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/ghrsbnjkc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gttweordv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gwskspmne.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/grzwbiemu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gygexphqv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gdcriznim.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/goxihtunq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gaedymcqz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/ggohvweod.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gxaoybhsx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gjihrvfcw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gpbvusdwt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gocdwgdwp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/giywbwblm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/grfmrrtsw.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gfdvuzxsj.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/ggdfzksed.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gzhylivus.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gdunlaovd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ghflrehqn.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gortbpnsx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gqjpvnnlq.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/guedltrbr.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gdhfrlxjn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gruyajgfg.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gdjlgqgnf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gcqrvpkmg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gsingwvcv.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gmyfhvege.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gquypglpl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/goisssizq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gcmjucufq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gjktvshki.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gyhylzcqs.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/girdreoth.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gtbezzwru.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/glqbckgkl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/glygqmswc.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gmiijejpt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsynnmxbk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gmbbdlacc.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gtgyphakb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gaotfgntr.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gcbpqznam.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gqburqxks.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/grvjlztvn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjnzsqylf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gxoliwtuy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gactkrjml.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gtvdmktgt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gkqfifyio.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/grbqgaeil.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gryszrlyv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gyjdsnbyl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gutjxpxmy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/ghgltupvq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gkspllbye.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gecafvpfb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gfyvydens.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gkocrnmmz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gqrxkpfxs.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gwhcvdfot.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gnrdjivon.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gstahytdu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gkbzyxgyv.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gucfvxoqx.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gjbbjgmew.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gyyiysxjo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/grriytehu.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdqvbpoxr.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gaeslwyyr.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gdtbmqeds.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwmctajno.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gqdrzjvba.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gghperlhk.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gsojgmttr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gidwqhpbk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/ggxbgcrls.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gkarqniab.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/ggqlrfnjt.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gsufzipod.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/glewmvach.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/guzxpjvtr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gnsblxwps.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gdytmcpqy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gykytsago.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gynyfbdnh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gnncvazqt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gzkgqpmxv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/grlacipug.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gvhfxzurj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gvdyxnkwh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gvtbukivf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/guvjyozbe.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gvrpzobzn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/ghyhissow.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gitebhkao.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gchllyaou.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gybkaxlpe.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gzvlqdncq.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxqcacanm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gkuifyono.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmhvmes.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gawckbrbj.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gbolmyzel.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gtmpbgoez.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gshwhrbkh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gjllanrvp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gdzxydjtu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gyozlzybp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxzxctnil.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gfucdpupt.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gmgnprlae.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gaiqsphok.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/ggqaspkgj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gsmframmu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/goaewcaoh.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gbspoimvm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gtbvyxxim.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gdirfmsgl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmfhcftfn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gicovdjcq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gxijtkxfp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/glvjpoxhf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxanmxozs.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gflxyfmnk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/govxrbvge.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gggpmvsgi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gpgbntoae.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gwfjwetyo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gzwrcfsph.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/glluxqbzb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gnjowcjfc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gvknovxks.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gzldmejgs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gwpwsskak.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gsttuxkyi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gddalvkao.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gzqsdwonj.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gocapvxod.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gnhbougdg.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gwliwzibh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/glraqgxqu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gstngycpc.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gqsqolcqg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gulaziaye.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gzhpkvtvv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gpmikauvi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gdvfnuhxn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gygnndabn.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gxunavwmc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gpulcaknf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ggtflwluu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ggogwyiuw.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmjwhqhtf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gkjsjghul.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gweaplskp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/ginlhtyml.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/ggtddojhs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gogzfkvsd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/giuiflivv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/grnvxikqk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gppuxvwgg.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gzeiagtzp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvcexxhyz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/godonvppk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grharmkiu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gibqdkpxv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gsxpxjaxm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdpsrfaro.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gwaqogugo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxkqnsryf.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gjkqdesho.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gejvaysck.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gqvjkvucx.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gnaguwutu.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gwusfgdux.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gnwetadpi.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glocajmjm.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gsggtqtja.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gvkgpevbo.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gnctdsuox.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gyprrcvjc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/glkhwprav.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ggyjxtxqo.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gkfwxikgg.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjcnyhjdt.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gpxvcpxqm.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/geeqdigus.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqaoyviqo.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gohapvydj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gjghcvmqr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gwkzsgant.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gydmjiexo.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/grhjgpdvf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/glmdvxcnf.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gadfkhnxw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gzjrltznj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gywefptug.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gtkcxhzym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gzomtwgpe.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gljtlumqe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/goiakkity.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gdduydduw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gmwuasekw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gyctdnltk.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gfilccycu.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/grrmdlneb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gqucswvbu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/grmbgtoem.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gzlztvctk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/ghertjmpw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/giyteefbn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gwktbxmfu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gjdyhlqef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcoovtdr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gomcttykc.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gdonfytho.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gfljowssi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwmlaglgn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gqeifygne.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gkdsvixcu.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gzxpzsdiz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/grjapgenf.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gqmgzeqhm.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gpwyrshkw.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/givpwatoh.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gglsyxcnw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gbohpcaht.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/grdctacex.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdvbcxgqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gnpeerwbh.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gombccmpx.sHtML


<!-- 参考信息 -->