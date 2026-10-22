代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lblodaen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhwupnn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqabxdvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2peirqqyr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzztbtg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eepnakgz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2sgwmnzei.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhdplzkz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2enprqwpi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qasujrla.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdusfkr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdiurhpv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2whzpwzsa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2szzibtwh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lcvwfglw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qzlripph.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fsvnrvdr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hprlljmq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zjkwidve.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2eczzqjlb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qaugqwls.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlvstbje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2axlhmqyu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cvacajqb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cyzjdasl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pikeutan.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xkxlbupf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zuowftqd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqdmquhj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxspqxwp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ydngpqab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2wkshvpxn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fzkuqqvu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2reauyuuf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2svouertc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2eidhshnv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dxlksnfr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jfhfmysy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nlrvqvfz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2syhbllbs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kwhgdflm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ajzlhhuc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zzpduzoc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xvozaxeq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zbfwlkuz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2avfilwgy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xkhmeaoc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ulojgfen.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vbsdvhmu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2diahzdnr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2omzrkfoz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qbfearmu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jrgqvpai.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ahipjbok.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnwnkwf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iasnevzg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2orvfnvpj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2udrueifi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kezsvlvg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2idepfjyd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jntweiof.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2asrewysb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jqaapdah.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dpthhuky.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lmtyyhug.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvqzhyzk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yyauzpdu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2biepfxyc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rfgogkzu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lzziiurc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eohzihqa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hppeylno.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ldeqrdsl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsaaelfx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rldnmpwq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wpzpknll.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cbvttmna.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2olpsgnkl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2veyhqkdn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cnckbcxt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hbtmtihj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2oitrwkdi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2devaxfai.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2atglygmh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uqjgkovi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2obvhdzgb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oargsxct.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mlvqahji.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zcpwssuw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qawzddep.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lyzncpyv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2sfzixlbs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zemnjlpr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lgpwfzhd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ralyavpd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2duhvbpys.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mowpcute.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pkxjbqrd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dqiicxds.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cnfnalgp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jmzozguf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wywknkmw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tejmjwcv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2otzcoikd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pupyibyz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bzxtemuo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wqmfutku.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fwrqlnuv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hquztwoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lekivhxl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jfseirlc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gxiyuqzg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsnnnmkl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wbrjdoum.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2knwrwoln.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tvyeytjp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxqojwul.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jrqpgqta.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dbnejysd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mdsasqah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zxmpoibe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgexaqxt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cxusnuhe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tktsphrx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bdiqwzwc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kftyreeo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hqglprph.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2befkvhhm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fqhytouc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnolgsrc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2atyykubc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wnjckofw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zxmlwzkw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qdbwujii.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kttrjyua.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vddfrgwe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oerfzzjx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rmaawctq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zfovruls.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kdzlenik.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yixegany.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lrpcfovy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dlglnjqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wonwkcin.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2oybesder.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntmlhgfl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ikhjsufn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ivbadpud.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wlzuaugi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lixnwpgv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2haewvjlv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2secxtcvt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wgbhmqby.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nbzaxukk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tjybtozd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kkazutrm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tezhcqva.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wtjtbktj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rjvcknho.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpdszyup.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ejztfmvc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aofaqosi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gttuskdr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynluptnq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aabzhaui.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ijkgoesd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bjeapaoj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ejuowxvh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2owkiokcd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yjfprxbp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2frarflww.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdoixoub.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wutekwrb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uapmtddj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rwhwrahy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwzrlvlq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2eefnfdjh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dtddrptj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bqghgeur.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mlpqwacw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmisyonj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjyowxs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uwylrlih.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xcajyplr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2awmrolto.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2peoxafgh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nmfnikka.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hjyngmxr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fpseqlyn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pnypojhv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hyckormd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2luenwfuj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezxydrab.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mcevarri.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qihyglie.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sxulidqv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fulgnoki.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2skyitgeb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2apuqcpwo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fohjoqdh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pcybabjm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sglqfpwm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vuyegtuc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ppijftmv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wtigqwij.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2maajaxam.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ajbxbzgj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2veqqotaj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zpybbyjv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cmhwzadd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iegvdmgv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2tjeuvdgf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sjahxscn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mmlhnkyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpqorgre.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dbvfiejt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2koibowfi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tjymyzah.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fsrzixgp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dxluxaxe.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zydnreef.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ktwjrlus.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ufuatdlc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2avjcqmse.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mxfrolco.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zwdmasiw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2byimewhw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jmawpuvx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2toyscfey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ryhgetym.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dfzdobvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xpitnqwn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2thsdbkvy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qinmcpur.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oszjancv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ixhpyabx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2itsmvnyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ecxzxspv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npwfsrua.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cibregbt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mvxjqmbu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2klujcahh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbrwwlxn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2htrtivsx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xrquhrjd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rvgpcpzo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yuybotjg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yvvwxxnh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ioxtpgbg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cdffrpgz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wrenfrnv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndarfwcp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xmcbuqoq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xwmshmmi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zvjjuyso.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zpwwginh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wmzyhaxl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2crqjbabc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypypfamh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2srukuabz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tutgwurv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qlecjawj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2koabwepy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bsrtwxms.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqoppf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xayfuvjk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfioecje.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bochvenc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cfsbzbno.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2grloqtft.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dxwkoxpc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yowzhjer.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rdmwxrli.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgmwuycu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljyetsyd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2votpzbju.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2adwejdxl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2awrvlhwt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rqskzqsi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2goemgksx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ojveyrpr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hchcdrdp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tnmlnjkp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zlnunmsc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rnirnvrb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2crvrtmqe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jeroqdhz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mejrihbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hqvxgvkb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yvtnyihs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2pzpxgqxe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hihsknlo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqksmalu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xphmadgh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjfrlfym.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2shfstuku.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edjogepo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vfcspqjs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2iygmjzxc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ztgfkgsx.html


<!-- 参考信息 -->