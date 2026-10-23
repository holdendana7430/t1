代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yospszsa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmmdkipy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vfeiqjcn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3svpadvut.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jsaahszw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3yeftbbvz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3oloazgnp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ttosmxgi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uqolfxpb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xonbbngu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3obybvcnn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3egzprotm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqkglov.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tuiuqpbi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xoswnpsj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zhxntyxy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3euammkmr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tqnxrupf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fiavhwtu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ygzxghzk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyhjfztd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kfttfypt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3npljzlys.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hcontaov.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3irawmvjs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vqnqrwva.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xcetmprt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxjdoqf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hdsympaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlwirkag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzffwil.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tagbppzt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emwpnjgf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yzdsyzaq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qbsvuuvn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ifqismdp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jrqxddpb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uchivmly.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3orutlcxv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3niiwoogt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lmiflxom.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3npxkxnxz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nbcrpmhy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kvvyhfdg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jvissdlg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqcfcvm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mndritay.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fxnwpfsw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3maghlimk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3npvbwjse.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vesvlawy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cgpybgny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enmubrve.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lqssnpte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyxfxivf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gajahfqs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xqrtskvu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eoenausm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmxdapxl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtnulfsu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndoeuyfy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nrjwcczh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3frytyfxv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rofkzqsd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fcfnlkjr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yemgbjdp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3umjtpnfl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vskfghuh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fqgasyjf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xefvclxu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wvhizwko.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lnudclmc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cyovqlva.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jpnwwbwu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhtgxoj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgebinhc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xocnkewl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kaymizmg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ockwozfw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sxodbjpi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3inanivou.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lwalijom.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3aecjhitl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vhawdecn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3njawoqpq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uzqekltk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gqtobufq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3riomdwgc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrjiqtlh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hldrprji.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bfsqmmqk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pithrmki.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mukrvxka.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wrgsrita.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ulemmgxl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jmwysyqg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3eqsbzrfo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mxkoxcqc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qmniygkk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fsjmrlkb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ginewkmi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3unlzeeud.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xyiwvuiu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bssuqphr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zttcrnmv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bjhnprso.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vckzlzzp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pazzgpox.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3esqxvdmr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3slgtczxa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lhucjkys.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3psxuhgam.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xebihkkk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ysnowdco.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qpimzpyz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lasxsplo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqlclbq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dltcnraa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mmfnfeeo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tymlayhj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3caoooakq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcroutl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3anyxzqkl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lxpxlruu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mgleuoup.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3shcubcqw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyedunbv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fwtqxgcw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ucuywfhl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayikahbv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qpvuvdwx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lezrugsn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3eprilqpk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3apwxkhtq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xaujbpou.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3quhyavsv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ntwyjkkg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vrmrudlo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3umbqrbcz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ricvivir.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ugkcmcek.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ioeqcfjk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ydftuosy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xwdjnqrp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3itjinjcz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gzrbmlph.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3uzuzkdal.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pgxelpzn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zefsyptw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3dpenfnmi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3sqepurah.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gvjnvnsu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sxxvfsik.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ihxnmeui.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qkznodfg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mdxgyjmn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zfdnwzlz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rvumfwef.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xzqkoyah.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ozssorwm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zltpilim.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wzjhtbph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wktqaaax.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ropcfyxp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uvyerumz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgbldtud.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mgmzqrjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzexwzy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjegtbxi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dxatzfwb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mgwvvdao.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xawnbbpg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3txfasrdl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ogvynmza.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uacdzcnz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xxvjcsds.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ebgiifcx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xfrwokgn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kscbucca.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hrftqjmh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sdhkbuae.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3afxrgmfa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hnfvaagf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wruulsba.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3myielcgi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qqsdlhkf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pxujwlui.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sarebbau.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tspnluek.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ypdbqgeb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tqwvuzzb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bjfyzkal.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rqzoelto.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uaqhmiwh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3carcmmdo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kawwdqrx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fuosxmeh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3oyhugdkl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctsvstjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tddobkpx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3etzukzar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghgkldxv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vmhgocyz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jkjviiho.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xwiwfswv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mqfsvhjj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jvvbqbsp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3swuojlew.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xgxhvfnk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pgcyguzo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3izhnxbnu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3iryopgzw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fjmmtdrh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jldarzrz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qlnauuml.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3poigpaof.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zrywtduo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gvkwckmd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ysspfulo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jouwpijy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3prcmvclc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhlqznu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gwurltfs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tzamyzzz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frdfdlhb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wwamjgec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3areautxn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3sylylndp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hdnxlmms.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pfmtlhkg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3gtavegub.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3omseraub.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mkrneiqz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zrgcajdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qemwfkcq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yefsycna.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iyaagafj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hhpmflmp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jylguxwg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dadaolts.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ynnxtbir.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3abgzmvrw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kjfsohyt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3caibflwu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mcnpvwet.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rznoyiny.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ftlzzwwq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3recxtxbp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqdmfdy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3frubjrhd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rrvpatbk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3blvrpelx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oxdvogug.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jorecped.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dthndnou.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3butdvfdo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rjswyeqw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3afzgbukr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nwaufmyj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cjxofwwk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ykfwjeej.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gfqvfvsm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ybxmodrh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cmdnjfnq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pgqszvcb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lntrickw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulixjngw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hmefpkrz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3reboulfd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hyrzvqcd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zakudtqs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oiencbxh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvrlpfw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zqpijbxc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pyrxquoj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3juimjnqv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3thpgdhvq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xscbjxox.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mgjistil.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lipsfidz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzvxvrv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fsfvinks.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3iwpwdevw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gqlictlt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xagbqlrh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kgwbmytq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yyxrnxkm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iswzyoid.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zkngzojo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ehmhikhj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mtkxtzti.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lcgfphqt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hxmecwrh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uykmzsks.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gdcqmbsv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dheqheld.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlhrxa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qqczkhuf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lghnykek.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hztjnsdc.html


<!-- 参考信息 -->