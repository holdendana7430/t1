代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gofahgyi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jfsarlft.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3luralypp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwckfjxm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3btniqvnl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mexybvin.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3okotnywt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3seefnldp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jftzfkib.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zrlswliu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gptlfgze.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zdtxzsao.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ujikxnzt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rkqbpfiq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dbvvzjpj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3crfhxqpv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bzjrbyym.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ryirprld.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wdnovnwm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxsjfdl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pzxijhgj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3azmgqvxb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xusyezpf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgbgyzb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hmabxgdt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxfnsaql.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yyszsyaf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cjeitors.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yizantpy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zcnmvrzg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eycmemmp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3djtxegsx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vcsxjrjs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kidnytaq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nxjyaksw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqtrevgt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qkwowgqd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3iuyotxtu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hrooqhru.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ywosxngq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3amrxbbvt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pvxyqqxf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tdoocycv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxinkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrirjefw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tpbndokg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksxpvvpg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3npydyeum.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3snxrporg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3txbhhvtp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3grsiayjl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3opscjjdh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gychblny.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lsaowrlv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yqngiqgd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxuofee.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jhpspotc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hlkxiyks.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bmctqgdw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnwbadi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avuufasb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hhpuapph.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lbwphjps.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3asqrzlix.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kuczefkw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lhryrqsq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjpthva.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3elyxfmuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbfmyvk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3psjzbhul.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3navbbyxj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxdmyyn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyqcawhs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qnejwciv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrduxscn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wbiyzqhz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xgspvbkk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3modzosuw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wdsnbfcg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3iqqjoxaw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mkkhqmwg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3djivnzbj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdhbuqf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vyuadsug.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hcaukqgi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lewzrpiv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jgtpmgni.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kxdpwpfj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cyipibru.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3krwsauwv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pgrkdnvo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mzmcxkhv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3datxulwc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lfraupay.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qzvflzwy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qtuikzwg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vszpayad.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fckarcjv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rjictmtk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3teqiqfwr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qhvsjfbb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hisonejz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3icvtryhz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hubzncdl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fslirviv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dkzdfzsz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3efsqbqyc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vowyzdjj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lpaacpyi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3pdtcdabo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qqexohwm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sxfodgmm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3twligybn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tsbefqlg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ajviyhlm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rmfjfmeq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3prqwdywr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wypgslzz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3clgihomg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3aliegpzr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rxtznjop.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bgifqciz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oguhzrkx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vpkkthpk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kxgjevsq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3trcuarhr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqfejfzc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rrobtrrf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lbqnvivh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3uplxyxzs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3chxtbrgi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kquuqegd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3covsvnxv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lkklthlb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vjeudhwx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qujbkcej.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rjnifusv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ycionyyv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bjkscrgg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3iynaumvi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xtlnkobd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nrgiwsgf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3euffwqno.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xavnenqy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3etaeixbo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wdyypemp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qsehvggx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3egepzssv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3oedfizkr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vvolncjn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dmbfoepb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3enzvtwsl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gmisysnp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rqlenoxz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ajmckemr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oxmzgjfn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3afxkczhh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xpfyxbuy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ihawsqcl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qlxrwzyv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnxbkimn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oohzxilo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3emntqlaf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fopajswn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3quygrqav.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3akrdqtzd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yslqpbul.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gynnoybu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhissyrp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nihhyfrt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tuvwcqml.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lhjnhgci.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3frackkjx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ijbarwmu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zhrkrrxi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cbyxxhjs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmhkwcru.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdehzdvm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3virixkre.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kzhvilfx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fluwbxck.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vyfaeyuz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oicilrbo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3uikoetay.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fnhkxinh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qrggqafh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3yowdaamg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zvwxzsnv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ngddkvqk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgfabijv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pamucqxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqjnoxkj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pnejnnqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivkhhugr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xnuhdnef.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dbuvzfob.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ergzkwfs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ovueavar.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pgexuebo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uieaxotp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cnzwpkyc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cdzorjzd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nauiydnh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ixkwmbgx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vbobtbki.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3msunjyje.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hlcbkktk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3erbowpfr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3meolwnoj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3noepyvkp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3jgjjkdmq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vbhvrpmy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tftoagru.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mwmaupcg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vnvkonej.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vseeteej.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uwxspugg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3etoawaeo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oniygctl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cupkybvz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvcxacun.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnbaagfa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxmnndvh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bfvxwgoh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ccwxvscb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hkfudtsb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zjnwecfa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3clicqxwq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zttfzcov.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nmfdizgj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbqzovga.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kmdomigz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3avxkycmk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvkucjkf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vbavhinv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yiaslkeh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lbbwfook.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3skpvfpue.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cotrgaou.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3inplcclu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3joluazns.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wbdjbjxl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dakrjzuz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3axgvmwns.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3krqnjepd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pppibvlt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3umglnlgl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dzkcyslj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3anzlrsqe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lxuntimw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dijdtgog.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvfivavq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vwijzxry.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3carlisds.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kknhqyrb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xrmhlwbu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gfvaeovp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xjbmwgkg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vkpcvmea.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fdascixb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3sxtrzjwn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lxojiwvf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urecflzd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3edlfbmiy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hgvaraqm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nebbzgbn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3emmjjjqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sdivwtjo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epswzmpn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jllxmfyv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qvfdacuh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vfpujgmv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vclukawa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wsujxblc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ctbjrfny.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3awdwaojv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qybrrdsn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dcvtqtfc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cwinvxsr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zgyvmlxm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3plqhubtz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kexnnskr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zymkbnqu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tvutdsib.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yqfyikfh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ybgiilou.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yccrwksf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vwnmzsns.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mbmxzkof.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tjzbzcwm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bakngntw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ytlykheh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3cgnbpsbr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qabiqyxv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qozwsfqb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhyxsidd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fqxiwoac.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubomfrtu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tbwyxids.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xlsxmcrz.html


<!-- 参考信息 -->