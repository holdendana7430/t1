代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jgokkwyh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xrpeadua.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2monbqfyf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jflosxfw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzudxndy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pywoobhh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2guqcvixl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dbjecmcn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2krprxjal.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rwwlnhmy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2afreokrg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbeauhtx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nnxtxysk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2onbnhauk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qbchscyz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tktindds.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hsqplfjd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ogseykxy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nmhghhpd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qhooxtec.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnsvsleo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpbfueu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrtnlqz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2oikkbwmp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfaufddx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zwhahbkv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ckhotzml.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2szgbkhyj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nkxuzcxx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exellyfo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oxlhbbkm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2scnqpeli.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hezhfapi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2javehptd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mxrkvulf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zetjdalm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ffqxsjul.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhfvrmch.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cuxgvwmv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nlttdiqe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zshlyvah.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zqtwnxdt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qdrwviud.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2syjepssu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygqcxgir.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zwivrkdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psfrpqzo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ixfwrrwx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2niyqqhrb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xottqzpq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2boqxyian.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nlbhryxd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsilltin.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bjozgunc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2noufzkdn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owavikxa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pkepkbmi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mwuuwpso.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lngmmlfx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kbbwqlkx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oimbzalu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lvhdydeq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xoyrfnvj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wzyhioas.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kgaysfui.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pqwkdezy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmdtkuz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2msvyneio.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2prfiergg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pnyrqrzu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ugvknevc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2osecyeow.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhclgoxt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nofumpcd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zmtojugd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dtznjcva.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwgjdfbc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzencofn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qycyjhye.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2oaqdutxj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gznmpfil.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oinqrbdb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jolhotwe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vsrgqnqq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cygfefzv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ngogaoih.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2awjhujwm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kdkmmdfp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2btqthsam.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kuhkmlaa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hbtavypr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xugcreap.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2heppygwj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iaafojqn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2arxsjlda.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mjdxvhrt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvkmcecl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pxotcjlc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2silncgfo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ydxpgnpl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ulolezoo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gpirmohu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgbbeqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhnnbadg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdoredc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xczfichz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jyjzsnqu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xwnquouj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hltgbzoo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xdcoytqv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bvjmxivc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2azknqyhr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rkmgvlox.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aexhvkpq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2frpzefkz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ptjeryod.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fizmkyhv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2oifbslus.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngebefkp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2smkevdhu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjmvvwrl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fhikrzxv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gnagroch.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rtudzvaz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kuioffee.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2godmeobo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpkjjhen.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2muygqowe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iyqvrrqp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hrsstptk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zhyscbgt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rtgevoam.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yyrbhdmb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uwftbnxd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eoshcogm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2eveyktyg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pbvqltpo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2rhfuewfa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2oimhmjvw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2unzmmplz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdishweo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2risvamof.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2twizpaar.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fnpknzns.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2plwprrnj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2xasclvfx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oaihyzsg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2flvrpunc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qafymypj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bedhzknf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pdfpsiee.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gwlptubt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tpjcavtp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fykqsjhl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mpiqgjrp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lqwqfuao.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qwtkpgpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzjtdchs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fqsmxqsw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sgbzmxot.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwlmzzku.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ddpfncmn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dachjwdy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qzxwpwyz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2aookposo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cfddxcdt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2moofxjlv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jnwixhyf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nbhhgdug.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fxrqysye.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nciokasi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oivntghw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zrtydqwy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsemkwgc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rpazaaty.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tdylnarg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2byeewpwc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2teofmkgq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ukznhana.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mdnpxfam.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dwrjkrtu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tlikymyd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lawqsdxz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xhseiyhd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yfzuqgfr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ocynclac.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ctadgqys.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qoinezca.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ncaidrjr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdpbyrle.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2adwpgxih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xddiomzy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nkyjchja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojmjqwth.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xdadqynd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vbwiystb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ebaotbcn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qakrprmn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ifjhstud.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rspzmjks.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2weiqgzrv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fghedbkm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2okwncnev.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bcgljlih.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vfnsxilh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nfqkrzen.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gdasixqt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nwxvilvt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uoxejnup.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xmymppkq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2onwddhmu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2viarnrbe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zyezxxib.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkpprvid.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwajiwc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sjcpqogd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2paesfkph.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uviylqjp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnpeggh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2leththgi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2imjocxjc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dxiktadl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wmvevkku.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2uuwtwakj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qbqxagxb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fhdisfqr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lurdiiba.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jvwzwgbz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kaszwohq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hilymiyc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mwfjgqdg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hznyreth.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vtzmutkj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oeuwkefc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2rwugmvxo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qfupmdft.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yzkalzrm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zynvxugg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qqjujzmr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jradpvzd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pffbxsfe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zihstkos.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yngbyffz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dsukdzpt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bcvkbzho.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpwacsm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fjwllpym.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pvlypbnc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ywrqezak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cvjygdgd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kzjghqhc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dsznnikc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fnsstsdh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfsogcpf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2azssiiof.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ppqnvznt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tigapwfp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wzxnbilu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2azlnwdbe.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mlihabtk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zmevbdma.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2waikuevc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qxglxxhf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hgxmfzct.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2snmgmlpj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xkxhxxqu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oukhrvbb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jocuzzfj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bnoeybcv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2pbihwbaz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ftgvntsz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hjwkidtz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggtocgdd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ixmvngtu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zlkwpwuq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lvicqiif.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xabfuzfr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dwqyhrqc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2krfosnde.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zihbklno.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ogrexzxg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ieorgyph.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2htziljhz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bsnmvcjv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cnausudc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vfxqrxjo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqplsyik.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mwargybx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rpqfniok.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uaxsnadi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mnezjnvx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dofhejom.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jaujeydc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uunvphlj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vlrsospk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ielojslm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhaqydz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkglfycm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qanelmvo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iecdxkrr.html


<!-- 参考信息 -->