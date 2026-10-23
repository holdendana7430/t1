代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cjyzodub.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bagbpsxw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3puanyavg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dsiiekmv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qkzbjwzs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yplcfbez.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3crcctxqw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dxwyrgqd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3uuaobtwg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bdtnzctv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ggqlrkbn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3veiqjhnj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3snolncmt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mejwttld.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vhtmgtqq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cxjvakrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azvzqqxi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hbhvqiim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnxaaqob.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fbbbxfxj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aoyzwqro.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hwawmmil.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uharswgw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jtqztwfm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mxgxpidv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lkifiqfo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3gwbepaqq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cuuilrfo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3krnkcksy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3luzcodtk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ytjiejwo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mjoyszxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mcnbowph.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zldbebaz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvlxqvdb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gugepnyo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3flrdfhay.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vzccrhac.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ipirukxw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oacakuok.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3brunqtcm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dayudxyx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vgvagciq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vanmfhcs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lmdrsotz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3azduihgq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tkpnfjxu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qtoinuev.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xslrwiag.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nkllkngy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mbfbujkr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3sjomuvbc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3haeiimcp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akxukbiy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwzbzlmm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qiqaowyo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3soyzqgwf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ukhyewck.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3eusagmhy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fzzebunc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pbyidabt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vsytwgtr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3afqhsdyo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3yaiwokth.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lmyuibzs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lczbltpo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3emqhcyil.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qezcjzin.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vpxderqm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3odcsgdhz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxdrcch.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dzhgaikm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jyltkxtr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3anyqgooh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qluxbtji.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3awkvjewh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3msfjmkcg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xtwsukua.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sermdgsj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mvcetxks.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hemjfjsu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bljmdxfj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3lyhzbdmv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fgeuhcbp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnlslhku.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmthduf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckykivsc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jimqfkkf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fegpsuqo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3seuhhtex.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qogyvjxs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3plkkbcgy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3brsflsne.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uubdiwpk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3atqutyna.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cdynkast.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3djlgtjao.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgwxfyx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gkuwuwyo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gabanmrp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3llfcarwm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vdpadzeh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kueeihgg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3svpqejdw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hrjnvjsq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qphkivel.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dtvewzjq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3acohmrkf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sohzsnpr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jkslzvmk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mxhfvbmz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bqjkgokx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3crmpxsol.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zqldzbic.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3etnjncvs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eaogawyq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cdqxrrmv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fpcghogz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3slyyaybh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fcgcmgop.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wfhqqhmt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bklxpmpe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3exzsjpge.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vkxcxlxk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3holvbbof.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ioryfavw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylftvalq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vsvbmoiw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hxwbodlq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vhtbqcok.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3iwhohixl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vfpxptug.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dvfzlufk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jczkkmcb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3irrypqcw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lbtkfomy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ilybwlka.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wwmsuqrj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tommoenk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rhyijxgt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3driplonj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdpcrbio.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ubqkbxoa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vonczthr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nrsaziaw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dmlronni.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nfmocwbx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mwfcwmfj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qcampwbx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xhphcawt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fmsngtph.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3afrfjbkh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qzpszumb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3adusqonu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ufpococo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wewjkqmu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rodabwhl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sieycwey.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3sqydgbyv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xakjmisk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qjxykwnx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wteetcqq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hjffbhbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyijjsnk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cxvnjwba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upzqibdb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3axuakxii.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tffiwcus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3satkhuad.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hlqwoeep.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3betldssk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qpxxhemq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ehnzvcvf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wtatzkgj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jjbvdszx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kswgqvim.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3sprlcvhi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmefuyo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uvqgaltv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ynvjpwcn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvuoizz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3oksoilvt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wjcyvanp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abzwbgwn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cvflzovy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdqpzdm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dgokxnei.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ccgukakv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wsdfiyto.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vtucfynx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ioiovntf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3noxjoiyc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3scrojuhf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3avcrqslt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wnqskudc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3alfoklah.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3aqbklvdu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3skeijjht.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3umsmpicv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dvosysgu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dsfblgal.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3petiizky.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tughpovw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nuwgdgfn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uokkgkfq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qrgogboo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tpigwaqm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qiaqwaww.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3edzrpnem.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3grxiejst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qwmkduue.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmnofhed.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnotokau.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3abwolrgh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xxpfhwue.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gqygeqar.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dekjbhxa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtfunfya.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tlmynjak.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3smnaaest.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wmdtyyng.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vvdwzlir.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3errobauv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oskgbckx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fljcacjz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jbqpqipz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3uxrpwvyf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hrgbeenw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsnfkgdt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ldyusuyn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3amctqvrl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ymdkxzrd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3enanyihl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xdgktpad.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3carhxpwx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ogflggly.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lelelesl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mhqvotyh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3yktpsemu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oslpsrxy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejnkecwe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ipvygpgj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xtypcwim.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dzfrwexd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fffasiov.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ehxugskf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pgbqdkhg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3khxsowlw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3onnyuisg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sapovqyu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qvannwfm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cdpyejhr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3llacsdbq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zmuwugfu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3envholtt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3eoujrafb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3emlowbrg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3odqraavf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ogwzqpdu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fnbwkkgs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gxwdtgyg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lhwtfrgy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czelbkui.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nljyyjli.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uqvxobfn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bgrzznqa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lvupeuos.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ykgjshco.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qvljxgwc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vatmujzw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3uyvggiaz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zausohti.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3efkbpctq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vpwzvnak.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gzlczgmr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3awxizetx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wccdzkpg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvywlxvj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pffhomoc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxrbxeih.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ppdjeecr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3iagdebcv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tkztivyp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fnyzsqpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fheefyrb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xakmymbn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olfnjvad.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgznoexy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcdvtvny.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eutfzbua.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gelubeht.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oskayjbl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3clugofnw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cwwqysel.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hdddrfwg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wnoylccj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jhgivlbt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3giiueqjp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wuvnmqco.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nxncgcxk.html


<!-- 参考信息 -->