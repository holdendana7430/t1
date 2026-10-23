代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyybfhxv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zeynmvrm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsuwovr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpqrazq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qqjxvgvt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nhixxwhm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ldufrgjh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwqdofn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3spsealrb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfevvwn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qixoqlby.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wyqpeskp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zacvjxur.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbvpiqx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tlblxsdx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vsfgrbvh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3iqemcnmt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kmgjefej.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cbmdzyqe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbygazvn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3innjkiti.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nwvggezj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lxdpaprt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qfgkqdmw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xhomlgaa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bolbwmzr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ntqikjcf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3emzknmqs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3efuokevw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ckcebspb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3otbmroeh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hqanfcsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdqkykaz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3peavzjva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wklxxgwq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wrgmmivd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3enghlctk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nueyxhnh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3acomsrzc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bssynlku.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gnsdhxbv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3idealjru.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ytklukdo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gueagibp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dmkzuifi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kdqyxyfo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sizrtokv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnxysrk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lkwdhare.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qidtqpee.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ngmfdcdv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kuftagyt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hbtvvlgk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3oiczvvng.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3coojgsou.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jujpkjdm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hbfvhpom.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuqspnb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xmeosncw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hrugslyl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gamotcgz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdwitj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ugshyplk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bsiilwxc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uupiyzyg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xycdbmyj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kblfskfz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fjtxgmpy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ubaprgka.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3usmxvcad.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tnoxlsfz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3akcnmzam.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ietjyoev.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3afftnuir.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vbqtiido.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mxlwzsiz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qyaosqbk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dqlrttrv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ejmylzuj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hapwmhzu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wzcnqgyk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gnpnikxb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3unmwdijd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ecfjjulo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rffbmier.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydkcrdoe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qvnvreav.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3upcikewm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zgdxvope.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3grtgvzir.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3liojqfig.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iuoacyrh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgnasku.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bhctzadi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tatoaiqq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bwdqyhte.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vyscxgil.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jjugcukw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ryicnhov.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3auxjczvl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeyveken.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hmqxdnyq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahwxzusr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pcuqulvt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jojzlnki.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3axffqyby.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3omjegiqm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3muntgzrz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ydnhuxsr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uchwhgtk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3prkqpvlx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3urglmgrb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3akpqgmtk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3duulgyif.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fguslkyq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fpoexrfx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aaxqmyee.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ocxjxzzc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gcpvutnb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xpuwiqwx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qkcyithy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jukctxja.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xhlfkjyc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3natljwpy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fvgdpyws.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3npxayyka.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3midkebjd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lvmootjw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tvonjkum.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zgitjgem.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ojzmppzr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mxazdcwr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zytwfvee.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rzpgqdxp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3aghyeijw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jkppplbo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vclzwguz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3suvfhbie.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zjzmjdhe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3csezkzln.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wnkmchqk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cojffszs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3acclmfiv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ufzqzpkr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jnafnkze.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ixgnfrjm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qnyrryyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ouphaheg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cjzpyrid.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jwhjhjfb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3aujiosdu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qxtbyvxh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pukvkwdr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hgmhiovj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rrwefopf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gpskinzn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvjtbwnn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3syttlnpx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nhkjaopr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xejsveuc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3aoltjqnk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vcmcbdbu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uxedvbnp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wwuvayti.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wkzgamnq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ksyyoamt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hrpvhflt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uwjpbaua.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3blkjaarx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yvxvjcrn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qstzjisd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vrdgvijh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cbckcfde.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qobmmwmw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cvqfwqgt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bivwibkb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3leefttfh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3usnnfygm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssdzvsag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aggxlcfp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3snxzyrte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbsflall.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jcnqijyk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dyvwofuo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yiyhbere.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ibofkeec.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nhneegtg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qzssyxsi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pqmvairp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3znrjieph.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lvqdhtgk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bnwxccfi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jlmtakaa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ksawpgsp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgycaiy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nyvvsqsv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qdqecaox.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hboigcak.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pavglnwx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wyetkfnf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvdmjgwx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxxqptg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3iylerlwl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3awjbxclt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bggklwmi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ryxicsuu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3quczktse.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qqewtjox.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrfxxgh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rdulvkbv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3peonyrft.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lkuayian.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3epxtmkml.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gqysavem.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hzipskdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fvoahiky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jonqcrze.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiatrih.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3shaxabjj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pdfzpukh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gmkbvaeg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ywksmknp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3whqlrjer.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cccajbhm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pdyxmtge.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qepdrrns.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yuznbbsc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ftanpiuf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzhdpdnc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nlecdiln.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxrujdko.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nmqmqtzr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ygiazptv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibonmarg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nhqygdfk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uwtqnkoc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bydvmjmf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hlaiqpft.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nmojxmfp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ytpadjnw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pybpgzco.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jdgldvor.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rgipwgfq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tpiklvwk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dyxawxbi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kgbogbmi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbsedbqz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwppvkt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tezjzhin.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xsernjce.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppxwaghq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3flygfwzh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhimcib.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqpcbjgf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jareuikt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jgkbaurx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eozuogev.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kfiihuxe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qwqgvrao.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3efjvqszn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aytahqkj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yoiohskt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nqtrunji.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3svxfkwws.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3znhrcmbg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ukdflinx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnlfhvd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3emnjxsuc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jysaubjm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pgkrxyqn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3htmlomol.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hbqpnema.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fwllmhlw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pwafxwsp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vdnkvyup.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aqyzsdlv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3psgyswyh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qknuvutj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rginhxgy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jnapjueu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fgbfrtsu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3bbkrevnz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ekturcpt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqqelwvb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3txggvsoe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3abogsyhn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tiafgyrh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibtcgoja.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xhfqeewb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3myamstbi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fmnpladi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pkecwtvm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vxncecbg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3urwoovea.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmqqnbjz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3auklhmad.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3amdqocgf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3birjqgec.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lvcsqbwv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yhvjruom.html


<!-- 参考信息 -->