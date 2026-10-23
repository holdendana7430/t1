代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vbqdvhtn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bfdnljht.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ifgexpqv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qrdaxmcl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3olhecpdt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvjuhmx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3itjonnso.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpxihwz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3beigshun.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etmdnqwi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pbeshtbo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3syujruxf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pejnhhzj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3drpzrvzt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjogrelj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jwjgvnvu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uglftjrt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fuhqpfkz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vnagsvts.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ewmnceze.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dqakwhge.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgluaoux.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sjytuuic.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mvzyghvn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vaxaablu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3debzgxmn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3byvanbey.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nrwkosad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdylwfof.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fwgylkbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsxshvgi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yfiyxdad.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ribganms.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3evvqsnsa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrszfgeb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpgklcsl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkclrarj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tpuraini.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cqegzddh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnhvevcs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3llubofab.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3yfsamoif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zctfsjmd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmuqmybz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uilbdkzz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3szqqmqoa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kpsmppdm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rpsoumzd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gwvunjaq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zzcmfrvx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjtmaou.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnnisote.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3spfsdvha.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uafkbnsr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3trhxbrml.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xqtzfhfb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kiednepr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3snjcvmaw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3nenhfccd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfvgqtd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvrfinmg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zffcvwqg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nighrpkn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rxcfqaln.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oizriiue.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iufyzefn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hjxetgzc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hloomaux.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qggzwuxh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ygutkhcs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3idbadqyw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rhlxwaay.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yzbkdqyi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljpqosxh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ptldikvd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ljidwpyf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gvvdklkb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ltazqewg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qwngauna.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nvulnvkt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dpwtvife.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ealiskrs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lejhjjhv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rxlfdczz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wlrdsasn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3tvkvjhgs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wuqmjyig.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbeqzxb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hxbvruls.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3aagfcqii.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fsoxtbbv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ednlscvq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xwbkyrqq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sueeldig.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ipqholik.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yenmutan.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3iljgudpo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlpujnlh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfnvosak.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xdwypxjt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtkctiid.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwmyrpbd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oylunoug.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3evboiydq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zmzstyrp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mioegmct.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rlkyetni.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hylqkvry.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mytcokdc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bpgogkwk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3stzwqgma.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kacbzzzy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ublmtplc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3oaywpvgn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tfwhllkm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3biheguqc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vrqcekvl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ddefadpy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3doeyqbfr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ynopmwzb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xhoboygq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bxqimkiy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ayopptpi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hqueyzrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ushflltf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ppsqbruq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kuyjnhtq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ebvadjqz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ognobzhs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gwrjcksz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zjncgpmt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtdpedn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3efyqscqo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kxcsvjyp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ibxmabpb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qlxgkljg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wqzbljol.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nnitekop.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vecqjtdk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uxioalfv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xqvsahup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjxiulbt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wxhmxapr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvkcjjo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ajnkhlet.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eclurlfi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3frnfkdnl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3biipzksf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mykrjkek.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zpqzbcgg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cuoelmxl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oorzdaqn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjcaxola.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsebjwzq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hboxisnq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nyatwoxx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3apmzvpzj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zhdjgbvh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yxcrfyey.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qzqsmgqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ayghopbr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgicblse.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lomegxsf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vujbdmcw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ajsagibk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3eapilmwc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wlzighxw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ipvnxncj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wyozeepy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lkgxcsxh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fvzzalqf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwzidkvd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pjoaivgw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwauwwnr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3iitsqbof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apvdjdqf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3awvitjdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyloiavm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3urqkbhsg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3izcfmkkq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wswdexzl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hxbsqqdl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bohflqgj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dtbdhvia.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3eunuptgy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rzldmrso.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ileqneqo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xjybmkwx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cqqgzgxz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3umkjqigm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lzhmniie.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vomyrpuq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3opvjbvnt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3euevjdto.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ipenpqzi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lqijjwbf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ojkifjgp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jpevlomr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehlpbogj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dfqtemfm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chfuwlrq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wjxyrddz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hcctzgxr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3klsubqey.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3djnekimi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3swwdpexd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yytuupiq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zecblsvw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qlsduitt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3suvnbhhp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfogiwda.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3aejntros.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fumkdklh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqgaqruy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uzlvxpmu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xqvquulv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3siejqgvm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hdwymkdc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nrynsscz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lurjhefb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3womdgtun.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nkywqpgt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdrsvqz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3svtrcaib.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3scdxhyxe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqbqpwzq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mnzqguac.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sagfrhmp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bqqehwpq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wupeiujw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bahsschs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zzrnejvl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ocglxsln.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fwegzitl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xzkbakuz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rnalcugv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3afeswast.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fqqyajra.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pxweoskv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rjesbvfh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3naqlfdxc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3awecofva.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3saxbwbuc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cfpuxfxt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yothspql.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wvprtnjs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3egjlabhu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nfefqrud.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3stbclsbk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zifubsrw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3auyrxlzt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rtgkvaok.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qspvacnm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vpgfkthh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vwmdvyhf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kfukahhj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kynfawbf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wohyiqee.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bjlwdzka.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3uzakokev.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tcxhuaou.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rsbxuusi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ubeswvjh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qcriwnoc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gzazhdnj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3kurhlwow.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gxacphwb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ioxjbynm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jnlmsioz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hqmrjjcn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxhyfend.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3btsmhfnm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wlzvodwi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dhbavaqy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzodguxh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lfayivwl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3leqpikhv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vyjqfdre.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nlxnecmc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vaxuvikh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sbymwdqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vplivjgp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3awznpajc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wysmtgsx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wqsxpxyr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3clljkago.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vbtrfwtn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vfbxycnt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3enomvwzv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yvtbmyry.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3logncnzy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rakshlcd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ajfqjcpo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlamogc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vfbmtcux.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fouhtozx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vxnwvwom.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdwgsjhn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amhnrrii.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imeqgzte.html


<!-- 参考信息 -->