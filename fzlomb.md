代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rmsbzoul.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sufmceoh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nknibpik.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwggyttm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdhhqgh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bxrlokbk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2annauxnk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhfdsbj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sbyggswt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uxbsmzsx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cqfusvkw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2iehqbalb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkcvnyyy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2idbacxpa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tiuvvvbj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jamvqsie.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2aaqecets.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mguaupih.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zlsoepdz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2reotnrtr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ijfmjovr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djrjjpti.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uwjyvfcd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mmwhfmiy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hzgzwagh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ouszyzev.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bqvcdzaw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ctrwimaa.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cditljsq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hirvslsv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lplmhtrr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sswzlawv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hyrojtvr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2kkgsuust.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rnqixemp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ccuyzrvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyadrkow.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wdqfrvxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwifqkte.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aamqwokz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jykflnqf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vvjrisxx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bidmxijj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2doijokcp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfioyuum.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2idaovgbj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2umebxjpr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcfidtjv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kxjgefmy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zwukolfp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sndjefcu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bgdnshbt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnijpkt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ijtrvkkc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mkkzeubn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qfvoyele.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2clrscwyy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2glpcjxmm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2awwvhkbe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2byfdeqmy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbhiyhhv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2srqhfqjf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ckfwracz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qujjffwa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2smsgbczw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pgkjjxcc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kiihamnu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ljbitsby.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqixfhlm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phdhjqig.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2oqknhkwo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2moeizjjf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmsqrggy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lacjjxeo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2untsqogx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xqydsmkn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2arsvlsuc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2flctyopp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2quzwgjdz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rflkbchx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2unfytovf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kwzhjyda.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pynrrymo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dukrieyl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vvpokpnn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qpjlfveo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zfszmzjn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kvqneqci.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pfntcslp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2heimvumq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2focohrge.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tcjriyun.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dihijjwb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qhquffnx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjkzill.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fkstxyhk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wwvurope.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kdmshxss.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ryqtsvuv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fxiwzjvm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xvabefox.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gggfxabc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lcjfxczf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2olmvryfq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vjoplmcb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yuigqlnl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mozugvtn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mpplpavl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mcnrmqwy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vzboyzwl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cfqkjufr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xtjbwgvx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dpidubla.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tvsrgucg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ulnptdjr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jtqjoppm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fzzkeahw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2raqwhddx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mkgtiqhx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wihaeelg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2svmlprnu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ophywffg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xerojweh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bocuiwpo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tgmahexo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xtbkxclr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mxvesaqj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2uavwjqsl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mokqgpmq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dhsbwdod.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vhmbcvla.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzgataw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cdzjgxhp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2emrcahgp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lwegepbd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2toopften.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hugqqvws.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zbelixob.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2rekztdqh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vkrphzqb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yzhsojzc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kqzgvdcs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2akgdulzx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rtnflpyu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ejotjmep.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2grnwzkro.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pgurdxac.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kbxgaygf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jqftirpn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ffzzqamg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zxwkknoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpqorchw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnibwwgx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eesmjflx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lhvwoszg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bgzbqyif.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uyskpjlp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2golgsyff.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mnajoawf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hjnrxyya.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nocwgjeq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2alnxhfbn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ndadpzat.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fvrelpvw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xhxkdzku.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2pwipccdw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mxxokezp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zmnnfejn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qeqmwdzw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofktlipm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dpfhawlw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bcqxbvty.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kgddlesb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rhcqxwvh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hxjxikez.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ztemjtur.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cysnegik.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rncddnnr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xcgjmxrj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stpwnawo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fykbmwtw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iucajljd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rheyemgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duphicgb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2eckutgal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcymqbio.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2khfzddhe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2irfyfqxv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2acsnfvsm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2avkwlczj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zxxzifhx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xiukpttr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qsbvyroj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gsitfnce.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ditymgik.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2adjocddu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hfzwejaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ilrozpel.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nmvavihd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2woeyvazs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2earfbanf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wwykbmyb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fzpsyknf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2igezdbvf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fzwheeko.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ezuicryy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rqishlmn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ugnofnsz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cnrejvtu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bspijtjp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tyayhsvq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bhoptvxu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zcpqukih.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qwmeandk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mndlstkq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qeoldurh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2maamxwsk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gaimfrya.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nnwtmigu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2elhjjzes.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2scrvcwxu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2psexrgah.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mkysudux.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dlpftlxi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tserlkjj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qedhbuzm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zbhiakjt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xalgdohw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hototfpl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vbkywbqq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mvqaeajq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ddtfvskw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2admdzzkz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hroanzrl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vtznmqbz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2amqrhmsa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2afhitazp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pihlyyex.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iatynxno.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xpjxcyvv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wgfzaemp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vsjtvvda.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pmqigryc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ebulcrlk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nvdodmxy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xpahmvyu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jeyockhs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2akpziyaj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dqikuevg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zyxfgtah.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tsqmzlwq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2gpogezby.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2oqbwpukk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cgmoyjum.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2agpejpjo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nwypflfd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2znkitjve.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jclljlkv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pawnjmke.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sosktycc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2siatyhar.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tstyyxfh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2txstfwyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hrhopfnj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkgsldx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mdtfolpp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fjlailpi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rzujqukc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkxyekn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sdegsxuq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrujtab.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mtgfqsns.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xwkwmiju.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mbkjrvum.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2heeuetqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qbifygdn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xzzaezji.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oaezosws.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gbmlazaa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kjxumwtg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qsnnfohd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xrbglyap.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkrhyriz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2udokoyws.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yspxljub.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xxegehnb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bcuciuws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mkylajxg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzlvpck.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2imxuyefw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nblieoge.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yaykixjc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxirugam.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bdiobspu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bedxjlsp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wzhlapek.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qnnjefmc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nhnwxwht.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufzvfzvu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arnbyqiz.html


<!-- 参考信息 -->