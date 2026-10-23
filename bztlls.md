代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqikfuma.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dfcjqldf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ftbstuzm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uxkgsdpf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3muaydffr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmbhemiq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wifurnqw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kyqfirwq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3apcpyuvz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fbigukjt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swrpsiqj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yglpudzl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ftyhoook.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3avfuitst.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tezomufi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3omidxppo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3atqttcfq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3krywjaok.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uhibfknu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3saslhdyd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jyvwsrod.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tgiebtej.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jtaubegw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3adqrefut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kezyxpdj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rptvdjrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvhddzob.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dgbesnbp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cxnzoxbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aerqnamt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwfusobk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mjruldtt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kynsywhr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fbphkqds.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmqwpsjm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3imxpdtvu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lckgylyi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yfkogrsk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3edreavbj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dvlyxzck.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vooqdiub.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bxdcqldu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qctjlolq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3uofvrvri.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hlsfisur.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ofbaopbc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qheqczdg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3brjhlole.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3htbkfkuq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciqyxgwf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cozohkwr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hoyqfvvw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lntxivaf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tlqriqpg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dshutgto.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jemfxuoq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3utsqjfvk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ydnfrbey.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oeutxexw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xqnvjwhk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ocnonkuc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfpnven.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lksuqplu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vqoovmri.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qofyxdjj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dqemvvye.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tqjtwzfj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rxtonhta.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qajmipgw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3krrypzgy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mfwxmkqd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hlprxcic.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fuphrahc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vjsvirrn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fnsxxrhg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3etsbthgu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3srabhhkl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yeuziwzr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ylfehres.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sxpwhtfy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rvpjfxmi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ujdtmize.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3orhiaqzw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pfmwfwkj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3atzuwcmm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3glntjpgl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kbbkdife.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gdjrzfyj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xvmwtyrr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ftpntvfl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3syghtvxi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3btiquvsc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3agsuwzip.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdievgpi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofnjrbab.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wenybdgi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3linhsqsm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3cmrrxsqu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zsxjgyjw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wrymvcbi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3swjcxauc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fikzascz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3obbsdpyt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qsisffom.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cdngfchw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3chcoazwd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tkaigjxd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qgsmwxzo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lfsttezz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3elhtadgx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pjncrhfx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fjpknhur.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qqbkckzx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ifrontms.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tioxkreu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3seizttjk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mpftsqfe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qiyxeblm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3egyhvgwz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3eyvolopk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sobwlorh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ucbecrnx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ohoiqqqv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3glitijvy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3typwueqv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3iilkjxjp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3irbwtsja.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3oginowbv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3yqzxchuw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3blilkhlh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ejwgtfvs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zxaroabk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ybveoafi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yrpwnbrc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gauihdny.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3obvpuoiw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qhfyhnhq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tkgkvvsq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pfnrjosp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3unvinkfa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zqqbvybe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zujrszed.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uuplboua.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3egkrgnrh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfuavaoc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ozjengyo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gqpswloc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wqjuqxyz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3skucldew.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pybipfrr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cqgflany.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ruglsyuy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hmsfjegr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwiwdpwf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jzdrxjvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ihpmmetn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3imgfnfqz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mebcfyod.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jhydhqfx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rnvbzfqp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lieodljx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ruyebgpk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rltqoxvl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hlslbnih.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cnzjxbfl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tymnenja.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3llgfoxuy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frvksjry.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kupxmokg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tkhdfnfg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mplytzwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugkysmpo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3tqofeyoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvmlwvzf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fykuyboe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pwxypper.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jnapcpev.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kqdolesm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ksftjqhg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dtrcikft.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ztclchvx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gqzhysqi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kbexkcgi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3apmwwmin.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xfpcnyty.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jdnewkkk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdhgxrgv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jjhzlxoa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cfmxxkcb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eaqhhrfl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkuaffm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cijgqnct.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3piaenbcf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3azfluwmw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bvpbnfyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sdhzhapi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ocncddkv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nyewqxhf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3byfujlnr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hqvpdefz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dhabpjwu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jksmfbuk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uigjwbuc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3svkrvitk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3iznhyybi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aeiyqfjf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtjfqdhx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3aljcsyfz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dlhwasaj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3akpzpgfv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gsgmcntp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3opkllzzn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3otqvxzxc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zpuluapo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bbgwfblb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3enskztnw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fmjqhwwg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3llondtou.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xaofdihg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gpwjzctm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ijntidxq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sktosbgo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vnghlgon.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3djabyrny.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lubjepat.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwnampky.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3avjfssqp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cntbzxar.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mkxhmnup.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hfelsiob.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fdbyyqxo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3daedherc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ouhbevgc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdqettsy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yodkvutv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3darzfybq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3udaytenc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jkzmjeog.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vavssqqo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gtsiptwl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cegehpxl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dmksqhmw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rgxfrmhd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mbwcdqox.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hbphzjwr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zyecdzhl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3chelvubb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sjyagbkk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rxsaprnz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yadmhcqy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3cyzrxszo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mjkuqzho.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3otoiohsu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3daecmalz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3haydxlxp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xsanjwgj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gtcczbqi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbslrssl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lyuxhbmb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xgqimruv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hulxcfsl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hgphjeqz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlqkrmb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dwdqwszz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bbjpsxma.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3sjbdmkho.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kzcujvpi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wewlfnts.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3yovjwtdn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bxegefrg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmeezhoe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gbkyudxq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3voerxpdw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dtcwwyuh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fmtowgxh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjzlmamw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tkgxdnjb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dynnltfk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bndxrqrr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtiblkdk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pbgirfko.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uhhiivdp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3neckheuu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cvbrgkki.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xuwccohg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwuxzut.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3htjhclkt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zgvsmelz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3snsuhqvp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3doxgzgce.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3awhwqqxt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hhgwutnz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ydsvnjhy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnasgzch.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygipilub.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lhkvzgjs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3joydyfef.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uschpcwl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vylhcicd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fvjhpfxu.html


<!-- 参考信息 -->