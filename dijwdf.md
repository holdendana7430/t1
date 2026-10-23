代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gdelduph.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfhvxhk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xkmxfapu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pihizmzd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wspeigsa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3erzgldjx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rtocwmfs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmaafzhu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tkwskcax.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3slqlzcat.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xoosdpqo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rdgyzxzt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bgabudpy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3urhtfkrm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oluszhav.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kotdkayx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3aawneogd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lzzlongs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nvepzthl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qprdtvlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmbyhaoz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3smnywcmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrmitnfz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjjzgque.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sfcdgptq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3doyjwjpj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sciwngty.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jqeuvsnh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfocpvyk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ryzdzgad.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ddpkyhgf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oclauqgz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wdytohir.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3awzltbre.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3glyuuzhe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tyviqedi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usvpcvvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vjrqbvdm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ojpeqyhh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rtqoarkx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ryboayqr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvdaqbwz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gyemmlio.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsxmlloj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzyrvcl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qsakwivz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pzevgfnz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zqlnuple.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3yfgjztva.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kskqyssu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kyjoubaj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhxftpy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3swavwfiq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gdzecrtk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3drykkwwo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ewyvprpm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vosnpmvg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hmygmfye.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhwzpje.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3waarzqlc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xvdgqczw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3swjjhtwg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gzqnmtvn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mtacszma.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3knafguce.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vafkshrv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wyezucpm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dmtifmvw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qamusnav.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jbvagzbv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3koznbdib.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ggrwfjcq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vwamoveb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3azbiabrb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3uuhfsgnh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rpavuban.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jxjzatwf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3oqqadolj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3urkysjlt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xvthnefh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cntcmbtq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sirzjksr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qekhware.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3krekuaea.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vzobkmyo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3oknwgxvd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xsqkdjzb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3uduwjlpr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3izjwnsnx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxcbndtw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kybtkagf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hmsgumiz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljxswthd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3khzjkzjr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccvxfzqk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tsytplkv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gwdhhxzl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vaynmhnj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tbogrtir.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vwpjdjmn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rmmbrjgv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mohfmkhy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zudleurj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xxusvosx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rggjtawh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wntuetlj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ngbobxtl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fmsgsaed.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kgtvqqep.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vmikpnbd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iselmtgu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zohxnsll.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pyazesjq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mtahiosu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ipnfbqyf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zqqhfjuu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pkqaccoy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sumbojou.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jumepcuw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dihseegq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3istwjcsy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3kkvfgmkj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3faiwhqui.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xpxytpxe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lpebaqul.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3voiztkml.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xtkzxdso.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ffkoccnw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zgdftcvn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ektpgtlr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nsbqubqf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gjohbjqt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qrarsane.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3urhdigdw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pbijryvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzeliqgk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3llfjcykm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3usbjlvao.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3piozohyv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3huutaqvp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jyjoifoz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tuagdins.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rtpdxdyc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3optmfizt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3adjizqda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tuorgprh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kotkruvy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bltnkjso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kdxjilmy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbvribix.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vvkcmcmx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dkrizhvs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdlalere.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jutilges.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3efyvqhsr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yudrkvcs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pdahzoug.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lsssybof.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xpqwbwtr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3orkdyepl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rxftbahv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hotpprki.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cyavugkb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lezchdlg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pefdhyie.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jbqvefzv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuzlqdcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fozydlmx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lrshljss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kshcjthx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3evxqrmtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3sydrezip.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yisvhluo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3abbeekwz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rqevatrz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dtmfjdfi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3faglmpmd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gzbulvfq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3appcsaak.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tnkuctni.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lgxuwrmo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hlrxhxcr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tcysvbgq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nbzzqgck.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dhgetmeg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3okhguvcc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gtherzyf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iygfyoik.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wycqwkab.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nqcvndgp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bsyrglyi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ybxhjogv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hexdgbtr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3atzomcyy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3emvjaxlo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tdjppvov.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgdyurc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vdftsgdk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jnztsjmr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wptfdvop.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vfdfpgbu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vxmexzfb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dpqiitfd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rqottyar.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nczgozqw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3swbxmekn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3julmjakc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fzgovlqe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ntjjdhje.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iyvyrhcq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dpzdzkqt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3txmbqepd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jilwteee.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tvpfqido.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vibwbfrz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cvdjnlow.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txutdwct.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cryhzxrx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kkfwqiqd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xdcgimlf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3czarfxbs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwwcof.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wbxsnfng.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3euatkgdb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rtuwmwwl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3grigwjnb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tuqdamua.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ajtnseyx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jzsayyel.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3eogsumou.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wpsswffy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wdningiy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gmapghhn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qvjocgbu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mszyrioe.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qzpmfbkq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jdkckgja.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tvihrszb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ypczqcwy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tzwsmmfs.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kaxoacux.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xhksqoxq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bczxjspt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3aluzqjqr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3krymloyg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ccblbvto.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jbyygfzh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hlywhrnp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbsfpvvc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vrqvejzk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zofughny.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mrgpdijr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uxilmwkw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ahfdvakp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rmicdvqq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hmobnguu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cowumzxn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3aymgvhof.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3untucris.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3czddffiq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3plgcqfdb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fsxxqgac.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ohaukxvs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dcdxvlqg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xmcentsi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xjaraxtt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydaosxgf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yxskfnri.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uyuwflrb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3teswrgpu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vudchxxw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uofrjtej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ytcdouqd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3osfemjhr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uchlpjtq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lopmbaxy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3asvlmero.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jicorawr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wkrjyrnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vibbqatx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3idcnkrvx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sqnrhbqv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gwvezeqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3izoexkwk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lvnhptsy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ibhceugg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tezhluyq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bgvdtwkp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ojkiuxhe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fzttdtca.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bdbmgmhy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzznimhl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjqheewh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mijjjipr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrhwoiey.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3egfrbnxx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3njgiifik.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mkkmiwmw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewedxiav.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tamfccdt.html


<!-- 参考信息 -->