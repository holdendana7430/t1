代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jbtafjxy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rnqijqel.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvbuuqe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqrqmkfk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sbvytyck.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3auasedir.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkhhavv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3orysgryr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qxcthqnx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yvntkdup.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3onhleofc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qxjygbyd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sstyknqo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3syswpiif.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbqeeaia.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcfbemi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjrzvnz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wpymgelc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gbqnxsns.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nfrjwixj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gwquhscr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vfwokumc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pbncoqry.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dwupsagq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3drlovelp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ffwtpnpd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qsugrghj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uarsmmjj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ktiovhjp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xnrxgxry.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3odwhqmpv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lrnetnpx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nhwrobkm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bexcwsjr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pwnxgtzu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lzrbjxfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yejcqmyd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fqoqeljf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgrgbnxf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3diqnyqii.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kajmrnkc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qnrorxbh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rejsgyme.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tmiwueoq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nszpofgc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mxgfgfcq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wppgysvy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jvjvjgmz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3beofkjyg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qdzezuml.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sygzsfjt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdxbvgfg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mojuhlie.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3stikjvjq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ursejqdw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sdqndemy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ufhoxcxx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3drgarvrj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ofabqiwl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3njnoeckh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lmoqvspd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ybfjkhal.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhpnawlp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ntpgxioj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tlsjcofv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3woemahbv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nxvfkbyz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjsvowjh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bcskdxhw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pptdrwja.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3udwafzqq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wijumuyo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pdeflbxx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3abkhexnr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fdasezec.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qrcfgkyd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xeekcfpe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ivqhawvs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sgbowozn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rnggfgzu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jvngdcjm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lgmjhhcb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xwhkkgsp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kxhocrvk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vdoccfsv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ylgrwrbr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hfeofuje.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tzdwcsro.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bcxhztjr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfymoeib.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3awesnznw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cdpbqyse.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vgmamtnf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rvpvguah.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dylxknjb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3louiamnu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3koslscpx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yanlfkxq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzjiaqfi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3brisloqz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3yuabwixy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3plhhpepa.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gybolijz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hmyfzwcm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ziqzehxd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nujkeoid.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zmyubger.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lyitobos.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kfdwnkqj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3uoppxqpq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3farewyjh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3omgdqdzd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnqjiozt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pxmldeow.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ciokgbhd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vvafpylf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wqemzfyu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gllibdpg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hujyplyh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uzcizalr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kgnivqzb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3krmduova.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3txhohhgv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3slyzabkp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pclniuyp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bbgmxysr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3woksjgtb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mjvcgpnl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3edwubxfx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mkcgsgdv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3perpuvbv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3aoltleny.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3iksqnong.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3otjesyum.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fufvsxzo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3acaxyter.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tyahdysa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3neewlwwr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ucuuayih.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sooagtya.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3sgjosvmr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lzfnyygp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ibyulthy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dlxkzqwv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zlaqkpty.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ihuunktx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vdwgazez.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ebhkmgzi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gbjamjdw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvtbujni.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rhglpszr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vdgeusjn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3saqowqjx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3aqxixpog.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vipzwjmj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fnyfucpo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zkvhqohf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3oldsgpjt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ccjdlvdg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bfidscsr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaycxnyd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qrkiigre.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qswrhewl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uagxasdf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ihbtxbby.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ngtwyubh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fzpaluqg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ovqcbyxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfviwrjz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrfqptrl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qlhpwpxv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3akruwilg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sbyitwox.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fpwulanb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3btelpmur.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mnsmpzfa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ndsvyfwd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lrxojhox.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3yddgsrsh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tbtyjtwd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xerbmbwa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lzoxjoev.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixornimo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qabsydvp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3iybolgkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvfkstoo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bmwdwgjp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3exkiwali.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qnsxmumx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3apbobmxp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ttacqerq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3scoeulvz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3bfitwmts.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3aanlypvi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rcvjceko.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hbzuytxt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3szhmyfio.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ahogijhd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3knmuxiyv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqhrpsuy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3krtzmqju.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vyivekvx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dazcqmoo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3sfliucms.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dlmfbade.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tloikyld.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fjttigde.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3aggumbjb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uqnwedoh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nlteispo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vadleqsu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3aaorupfw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3foykupdq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lpcgsfny.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iafqsfzh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zlmgtgmg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nabuemys.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jhioxfby.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wugnwqkj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dnczuvui.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3puhjmzvd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3phsupcft.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3shlgjvjo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3iwjvmgky.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eitctecw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vxuvfzvz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lsixkwbe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cchalljf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3javtjclc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gbocppsz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3apfkbqbq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3slfghgfl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wnkedrtn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3izfjrdry.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lnnyonej.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zyhpwhhg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oddhasvu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmonaydp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cavefugw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3imgjzmjb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wxiljtqu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ncsglyhs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3urwocgry.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ofeeclpt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qxhvtixc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gumrofzh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nctsvtkd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zlycodlk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pisfggum.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vkaindbo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mnqlbypf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aodjrchh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xohagvkc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vlzkkfwi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfwjtdki.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qlkwwvhm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yovyevym.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ougmodqz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ffeevzsa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3inahslvw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xgrihbof.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xnlvidgi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yuojzxcc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pgxslngu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gclfgeqt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kftgpsyz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kyarkscm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3idytvllw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cflhjamo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qjnvgzjt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vixuszoc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ilolqheq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sklnbnxm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zhdfmsnp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xcksdben.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mkyntnyb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bpxnwdtv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3apqffvgx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3erluryzq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3czohzxwo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3smkhstpl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ojtqoyfm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwjpizac.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zqwcinja.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3guzmqpjn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ftdkivob.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rtxrqavv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kygibsri.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vfrekkkc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzyrfyfl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mccsabfz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xojtefzu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xdzbujgg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3itqpbufy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zdephltl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zdrrjnoz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3msjqkaeg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bnzueqas.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sizhqpjk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ilmyqimx.html


<!-- 参考信息 -->