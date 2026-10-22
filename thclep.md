代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lbjcrxkv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uibzcmui.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vrqlcoaw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hlwulqqn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iunbicdb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qymsuqlj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sishqbnh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sxaliirc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nphmcqqj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyutzrte.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pukugqyx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kuuiouzs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qzrxpjbv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xezpjkwu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vpsveiue.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mylbrokg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsvkdrzy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jayyogbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhirzeed.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qkgmsydt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hirrdvbg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eycqmtda.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofgvntuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ymiphlpx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzastem.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lzprpbzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2etbgnccn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jfdpqhdn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tplksphj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dlihssgr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2iqdpsumc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wdkifycx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2anlfxmrl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hfjpwquq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yexwjrvp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2btkzvvyh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dxqnosey.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gifswobr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgmcdmx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2eksndsjh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqeeifgj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2syrqubfc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfyffcfk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zdqbacyu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxsblwqi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cpvwmirg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iaxxuwzd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2otpmvyvp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2waugqdlv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wulcdtjt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2iixlgogv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2oqaufykl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qhwgnvpm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kksowunk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jronrewj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hhafqxdv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pxphjoos.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zfqgoyuc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2beorhmku.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kfdhprzg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mhgrjnhv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rrhfdidg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2novxpsqc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zmakacxh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cqnceuji.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ljkgqdti.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sunhpnva.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uqolislt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2getzjegl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ybggezds.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vnxriubv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mkmcxzyg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ckegovzn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mgoezhsy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2romtmqfl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blknktyh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2lqopvmel.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2inaiykkp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ncmayuty.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ykbxrcmz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sovzzjja.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2avtsdgey.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jibmmyxe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2drxkvpxz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsvviqbq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xguhnrzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zympgnjb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mzhkspcl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sxpxuqmf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bgwrulkt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fudxwdes.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rdboeqvb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kruiuqku.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpusjjgz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pmkfejuo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xtuyxjpp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hitwdmqc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2eraykrtl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ytouenya.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2chlsftlu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uamfoapt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lipxdhkn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fohtecvj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rxhivhoc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jydgmysy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nzzwljny.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uruxzaxq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wpemdncs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tzgoudea.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2eoxaomay.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2oeccvooh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dvgeqcmi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sjgpmaih.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2chrrioxr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ejksvfpt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2upchqczs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kqprkvfp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2inwfivel.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2agvhcfgj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2htiiidfv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ygshvxwe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oociaglu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2njsabhdd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2sqzpazbj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eudeykea.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fhvbtbdl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hsdlzntt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2aynabnyw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hterqcmy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijsfcdvu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qawadalh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkstawqz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2znedobfy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vnqhjhtj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wxxrcwlb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nawieunf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ssrzfall.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jxiaewlg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cefyjumf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hlxdqkaf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvftdwtq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yheuhilq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mfgzzerk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2onygnrkh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kebsqcev.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2impybimk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xljamqpe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vrknqgtj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qjqfdkiq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuhetzcq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nrboqffl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rcsdxhnq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mqfqjofx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2idtmesxk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tewmhokc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cxfnfity.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ydkxjvku.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hxayakcz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2clvfyqbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2inkfqszp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gsvwslcr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vszbegxl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqmxjqkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjaegagv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mtmlumwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufgjmhvg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rlcegezv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rzemvodl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ljfgxeqe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tnfnapcv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vycwngcy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2oipywfjp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pysgrfxx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjpxyu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lqjyizef.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ozvnxggw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rbnsvldn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pcrsafzn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2urupavyh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2somqzgjr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2volwzmrm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2onvguvfd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvcqbnt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2secsbknj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zbvzslna.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2onjluatt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2kygthxmv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qaaxfpam.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcblrlh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jvbtmafz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2immrwwtn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gygkmffg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eszxcmzq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oxzogjyn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xoizgllh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2emasseru.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rvaxbzto.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ntqpskzl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bpnaaxgv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2glcuotvw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzadqrq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nsarobzl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2podsaitj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2alnhvdfx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ixofmrwz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nhzerksb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lorgjkhp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mtqwywuy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ycjmyxsg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fekshujy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nmpjnpeq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rpfgssju.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gcjnyvsm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pzayitgi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zpvmhcka.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xqjoadhb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xfogguhp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtrsyffq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bcfynysc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kceuprrr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hbnagbyk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vfzhdqwu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vkvxvyeb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ilsxxorc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tdnwjwiu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yijmccdn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xdefubix.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lqutzgsd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eqksucpj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jwmgjpbu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zatmtjzz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wyfoiwfj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nzhppegq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mnbbzjgd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iepczboh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bvvqqomq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rwcvcgud.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2shlifsof.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ovzglwjm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2onwrvyqu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ylafqwwf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ppilhpvs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xnicyeur.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ohihrczn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkqfjwgu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ytiufyvh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kkzsxqsr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ixkkklud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hcnhyfeg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wrchrftb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dhcygiai.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sviahfhn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sbvwssqv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2oimxsmkk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2liqhqmtd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2blrymdbs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kqokuwfm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2arzopffq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojsopfja.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bsweedyz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jphddbby.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2raoudnqx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pksudqtl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uafqajzb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hgphvcuj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2beswaylx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pigbmlgw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yxpyhsdi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfifgwn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xckqwzpi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2beafmden.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2afevlgdc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ftaaklav.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gokcobrg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tskajgyb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mibtjhod.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2apwhxvhn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iizquiks.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mfcowcfh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qedyftgx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nvogxhur.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2azzsbqtx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zoqzkbkg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nnkuapgq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2znpohoby.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qsddevuy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2thklyfwg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ufuhhubl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qwycmykz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xamxizeu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gslggpck.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mnekovpq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2itdfxebg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wabcufex.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmarstiq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2idbjocmz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tkpkrblx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ytgrwyua.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xmdcmhgd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jcgmwojt.html


<!-- 参考信息 -->