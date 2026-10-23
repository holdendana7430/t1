代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3felnovmc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nxfdbjre.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fldywzld.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3saczxbuk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqmfhotu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lyimyjry.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3frmfuqvg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lpscxkzj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3aofttxsv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cpzchhsw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iftplsqa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oqrdogyf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jufsmffo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ljbxyaui.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hyayuilp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3auqlldsn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nowyhxoo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3obpovjka.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zibhpcyw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qynxxult.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3orzykgvx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfyatgz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pxlpwfzx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3erroqizs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlbycgpk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jhezpjqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgzyowvt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ouxscbwz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ijsngfsr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrcreso.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcpqcwlb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vcpziqja.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cfsqtyfs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oulcxvqz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgdvptse.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vuqpbnny.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cafqohtm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jqdnubeq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vusmufxl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3glvwrrye.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzluijam.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yyavkyfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pqyfstzk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xvigxrtv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qkeujpoi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rpbrxadd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hisbvibm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ckjnedvc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3galhdrto.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cakbdjrn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wvufbaqr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bamoycmm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvhprbfy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dxyikyrb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qlkjksff.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qahbrwee.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hlahybkj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzmtuuka.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bjgbprdy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3aiuzijnt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3tctwxjtp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtqafawd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xgnbnwvi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lpkdggsp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vwpzesih.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qlycvycp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3supthsgu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nhcabtaa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tiqdgsvs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dissavoi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rvlxbiwu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kvsdnngo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jcvakzgf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3svdwoazu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lvsoqoli.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdzpejhv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sstwteok.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ahdoomnm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ajzfaorb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pqaisgeh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ictbyzgs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tqmanmoa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3enykxcms.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iuatzpga.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mxswmroa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fgqgfnul.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bgrpcvbe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sjdlbnyb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gvdqbaas.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mkkgmxhc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3aazhgpwv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pnjdlfyz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3sfwdfjih.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jlfqtevj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkpwnhmj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3otzplotr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tzuoftuv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpizkrsp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hfdwxsqv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cxjxjlak.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fbbvwwfg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpxreezm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dusmxauy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3aecohirt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zamnwywn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jjianwkd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3elxobyfo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xlxrpztz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zyybggni.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gehrmlyv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3srmmwlnd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hkqocfxv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3heqfudui.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugfswatz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mzrmkcpo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3smwqlzba.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nprpyrwe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rdyvjgvy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qdsugkie.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3blgzuykn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xpkylgau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lawvvcnr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ukipzjdf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fvvcasfz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gwoeeidt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uqjyivua.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kmbaqxib.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fbqvjsms.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jdzoxogi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nmchqoaq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xpndiknk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xbvhihbx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xhaojubl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3cmbohiad.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qkyotjao.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gojsxepq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ncvbdhnc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3baywzdit.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hkynpngh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jszyzdrl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeteaahb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dplxfoak.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dwsiymwd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zqylwhoz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ehdziivd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dmdghqol.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rygieywj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ekiumfkp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdzrpfvz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhswvhjs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nfdlvxko.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bxbyiqoh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ikoejzbh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yusqlges.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ikitjeny.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kibiersa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3afbbbmyw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njjzmuyw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3esrcgdmi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tbemlvnm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3iuxgedyw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eubwiems.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kysciggq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3eirwtimu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nijxeyuq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vraqpube.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ctcnqget.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kjpjutyg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3goucsavv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewkangja.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzwznqyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgdehoey.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3oakuchew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iltgrurg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vwdxjgwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kylkuusw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vnsxprud.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ogjvfxxl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zceuglda.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3scckdajs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mjuucjxg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3adafkank.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qyjfydtv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3urjeemnx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3scndninv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3shlnbiey.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsjfcsuf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ocezotdc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwaznozz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3yaclfomn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcthnje.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kzaagafg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yglhwkue.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3eklsiwoj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hlvftnfl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gkeajsub.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdxfiuol.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eiwsvaux.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jnbovksk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xovenjjq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vvdiplna.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hidnhpso.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xqvjqstv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ngyfqypx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vzgekxeg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3foldbwga.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amwcsfzu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yfrjuavg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3drejodng.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uwaxuepv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ewhgcwyr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qwpohawj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fluwoxph.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ygcjyxaw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hafnrkgb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uwqkomhq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qtbrjknz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3olljbtem.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ftrwzapp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ohazmjqs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kpbjgfrd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dxlvrdqu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jisnmdfj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bilcbopm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jbqdwbom.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eeyqtbyr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3idaxehpp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tszzuuxd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3iqxevrjn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wakqddnd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fkzfiwdt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3whzthuty.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lsgqxnlk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3masmxout.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mifpcara.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fnmdmezp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wgaaamqx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3pirxtadr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ykmovanw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3azwafgmq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lszoenez.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lbckukxp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpvkcmnd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nxansupj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ohulsomq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlcaflyl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rlzohfir.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rvojugjg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3njoggauc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xbempqwm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3taoqkhbe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3uxtmmvar.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crsznfbk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mdznfoev.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xgwwvidc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3btlysers.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvzpwut.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kdoxmajy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vspbdgij.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vdgvlsrr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3fxiwvqlx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3frdsoigm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hrudvsrf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lwpbthow.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vnshmfju.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nrdvfwrq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnjkuxzz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3omrfoiqb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ifolmpco.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dyrjhpmh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbruisou.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3heizvzon.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vftjnchg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3brhwvyzm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3paaydkbl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3offjmjxi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oqefjdha.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ogwxxpjm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ruhtbtko.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3shnpfvyb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lghwgyir.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3bbibmgnf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zhxbvofk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3whmerqnd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukjtfswa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kqkihhxh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jeaapcfe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wrkapyig.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mltlmrgq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3grwjfsoz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3beeqwelq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dthnnhoq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vmrjeltl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ppfmcowz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrglfrfj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkrgatqd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xzxlvnbx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wakiptlp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ukwcnnsw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nuqeyczc.html


<!-- 参考信息 -->