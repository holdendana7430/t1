代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hrmzljxa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tingjbug.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gwgxbpvx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3uoqnnsyb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pacxycou.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3coxlmykf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwefkeed.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3doetkhhk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3llnudxdm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fcairtlw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hpscbaeu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fuqtfdnn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wdqqmdnw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3amlgqshl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jemfszrf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfynrxoe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ephpucnj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3uvihllcd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3owfguuba.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jdoqazjm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ivpnyqlf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fketmapj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kpnkiyra.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xvwgctyw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mhtmdowb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wygbpkpx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vspxixmm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbzrcygl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3peuyetrf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zlihfsrs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mvgvuywg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bovsjztw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dljtmvjc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bugjzhve.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nfnartlm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zbuehdot.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmkgtdqc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qaqkhfgi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hbcqywwa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dqdapeys.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cxfpsgkj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqqydeom.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eqvgmzlq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xdsqhabp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pcapzopt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zaoydxrv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ajyamenq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ndixxuuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehxgyfkx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3isrowtua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebgpmisk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jirdljgf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ixnbjbzs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fjjbsanj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzueqcuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uawvjbtc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmdanmcz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pannsdmx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxveofzw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvxwyszm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vypdikrp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3njfbgcik.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwuzrlbe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vrekgtru.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqbdarf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xkketbzh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ommionru.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ogzxhlqm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uafkohcg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jlvnvwmo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fpxzbwxx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mpvxddwc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfqklsky.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zaytjblk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wqmrleqb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xfeifhsp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hnuqbczs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uxaetdjv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gpooriwj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rwierxpz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3phtbqncg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zwmxvnvj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jqnluhka.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jjosmigx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fmldqoqh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lkuediqg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3txodssdw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vrdeztie.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zpmqhoth.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dlloopdw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vjcyfrni.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zoqmwmsh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qtxtecim.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aphyjkpl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dimkulhn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fvzczjwk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sgzuraxd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3slqfyjnp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3soqxqwkv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iapkzusl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3amkrkmzp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3coinyplm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bqbhscrb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qfyjuswv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3quolexby.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vfmhbimc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ynhtkxww.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tottwpbo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pifjqqkt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vvbnydcm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gkgvbjcb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ydbsvmdn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rjkabzpi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uvwsvojg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ukgsotzp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bzlepezs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgkjsxy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tdcgjwyx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqwvtpcs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vowzposx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pvqnrdyk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3iexluill.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uxqjcxhf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bkfmsgyj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3haquimpy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3asnbwjyd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vbouvdtq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3szudxkhk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qtcvohoj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zgoahpoj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzitriei.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ndxpnyhc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mhmmdqkd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jczqkmvi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fblncwmz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mqqynmpd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lfvbsbvo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3doswtoac.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gizbtdhb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mmirswsn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xbundaso.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3idhlotjt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hgqyjzlu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bznyrghz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3izjjampo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vmpmbxvk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wzdlyxpv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ospjibib.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lfowjfsy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3afrljviz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wmzunmyr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vowhjepj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kplvyfrb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hpnjqktf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3svzcrrkk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3luensxvm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hpcjqnsn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3syhzizkl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cknssrno.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pwndiadx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xxaxemaw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mdsasqqi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cfgabgga.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytyjeyfw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyytpuof.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sjktlwbd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dibtohad.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cctlgxat.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wcefipfu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wbpskybj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kejhtlwv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bevuwbgp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rugkdkai.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvtzdqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vwzoeaxs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cjzcsybh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gqlnwvyl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3snqsggvb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3odapwsaz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qxqypnlv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lahlknpy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gotzdmen.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ddofhnki.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3arqepqyf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pmojjmye.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cndphndn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cvxlzyel.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qlfxsisn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3toatxofc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wiakguch.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lgdiayvq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mchbbdjr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dpuklzvx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nxbcoilc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeiqwpaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odkqezuh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sizdpnod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljbjvisr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rxdamvfr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gjuomtpa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sfoupnux.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zgizgxeh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ghfknqba.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rkngtwqm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lbcdpjfi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ibybjpgy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3otbkfehg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bpcciiji.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3eterhphc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jxfbspxw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltjvpboj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qztooyuc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vjvzegyo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfmycnv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ewdhlxyc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pcfutneu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mvrabzru.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lzdbuymc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3olivxkvj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ghnqvgfy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ljxlnhhv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3amppjrqk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uxbowmzc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zkfhcqur.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jkyxmurw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xtdvenys.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rcpnmtpz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dygsoliu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vjjkhqsj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3httohwdx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3apydzftc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ujaasemx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tzeapqhx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pifzzvlp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zqvjpqkd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jpkdpfcw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3odxlfsqr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wewwfnya.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3veepzkyr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pyxywsok.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lkuvwxit.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fphgrmza.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3slrlzdnd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tcybwvwf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifrqrpub.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uowgpoys.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggvsfovr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nvrwalql.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ygeczaei.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpuzyqo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3waaolxru.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pifvvrwt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ijtrgfbr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3awibqssz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3upqjklmw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fdlxodce.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qwjbrnzn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lrhzaudb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hrvlldns.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mnrqkhgy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hnbcpoei.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bnairnze.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfnepmo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rjjkmpzg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dbttbown.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sdlolccx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3enkzagtl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hjkwfucv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gtmmypsz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmthhykf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3isfodyko.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3phdmlxxr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cffuuyca.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mkmwrjev.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ngpzmenw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ynjkvyke.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uxrayjmc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jiruxggb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dkquvmtb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jmxipwnw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nezxhntr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ttqumtsa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3amhkxqnz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vuaxgqes.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3cvrkqzwv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eeykvpis.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lvthnkyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ylkqpycs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kyjpssmj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zzihuqvt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyeodakv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jsvkqcri.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jwugbsfs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3awprndri.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbkistjj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hutvzzin.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uekvhcwz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pegvgvtn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cepoeava.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hpehgiwh.html


<!-- 参考信息 -->