代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lpddpupm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lkhmegoj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rungnonk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2iaxbwfsv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2aedcfyqk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lioexkuq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2taxdwzwx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zmwscykm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2luprueyy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jncxuvge.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2btcikppo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fbvdgjhh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2swigujmv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xyenhefx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ysohdjsm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rryfcxoi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqtktiuw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gemxdczi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wogwfjmq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kkacqizt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxrdswea.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wtjhhalh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rocxlslb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yamehzrb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zqqjbqyk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fjdjanmz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwucwjlv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fmxqppul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxlfluvb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kheoeeon.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zioyckfk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpdfvdhj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ghhabnax.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zlkpvjur.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbjaboyn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2frfkkyiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ismewjvd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ijqqzjam.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jzndvwrk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pxrnwxdg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tsyzvugo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2nwzhycto.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kvzjvszb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2csnzgpic.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftjchvse.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mgefzvex.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tbxgffca.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2yshuunvd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mkxiyqpz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vmhcggnx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rdpdjxqp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2msarldrk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbrpktjx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aufmoxsu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gsnydcan.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2osihbqfm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ggyvqzoi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jgjbqrqm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxppujp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2uiruzpej.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jwpbinhv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bcdkbwnd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ddvxrgra.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lvwupiqv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cqtjuajz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rkulnjee.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2chvbaenx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zwnzemoq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxaaxq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nxjjapyp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ddlhdjej.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fxeeqvuj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hspwzkuv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2yhgzaujf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xubzutnc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qrmnofzf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lxonwotq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pcngupaq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ftekqtwn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibjzjkot.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qdczggck.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wpfphuaj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2occuztgq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jsnekrqx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2iprvuius.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xbjtlews.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2torxuyse.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xojvqchj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaygrykg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2garksshm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhlowgxw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pflcsuji.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mdntmizu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jfajdkwi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jnodmzsi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pewdqysy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrpkdqre.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2juyidiwv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sylbqngd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lplkqjuv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwrpmi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2uamigyzr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ghmkfoun.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hncykeap.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2yygxrkzs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pwxcqmrx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pyyvrzov.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dzbspslc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fhwwxaqa.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pgqoebht.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fnxsmqoj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cacvnmch.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2heejbewg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vrcadmor.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2exrzjsdj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2snqqoiws.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mpyonlrl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qquygezq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wlhwvrlb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lhorztzb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cenysugo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2glqjgqod.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bmmhdrch.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2moczprtm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jogkpltr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gpjcpcaf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2myjymllg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mbufutrh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rpwiiinq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zjaisjak.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndxgncts.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2esdoivtu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dfzevdee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tettkxpw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ggnqrwco.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hxrgjhkf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oywgutsf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2deiyflfx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2szpnduqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vaoxhxaz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lvqpddvg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lebinjhr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2leczwmqd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wxcjecfe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfnedllv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncmvjrxs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qdqmywmr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sbzbjxty.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ddsvrcgy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgaluize.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2apqjohqz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wamosnro.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zkscpyyx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xyuzecsu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sxkjxfzf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wmlvkhta.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ndypiodz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fwpvlfpw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2afkubact.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2djbmrges.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wakwfikz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2naakwyrb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fvzzktfx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaxpoagp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mmmjzdjx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kljarnlp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qrezfrip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnrecvvu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bkfhzvjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtncmlen.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vjmdcwrf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ruznokll.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sctajdzz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fvcqadcm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tejrhubl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xdoqepcj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iofvlfpw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lnjmtieb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kjmrkxkk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2aqidyzip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2etuapqpn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2awawjram.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrcyconw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2igspphdg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2aevjrxfc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2juvhexdu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rrxvqhqq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xwgjozvs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yeivupkx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgjnbhh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dlpdsjgo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ikbqgant.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jcekxscc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dnzjftla.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2culwxohz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jlxrlpdn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2stpxsvao.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xebrhvzl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwfniur.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hojgfreq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fiqubpyw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nqycaqnl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iugbosbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hpteexre.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qetheyag.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ovpnktpi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vegdlebk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vkzzksen.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nxkayuki.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bpvccdke.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vftcecjc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dtneefkh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xpbypele.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uzkuwvfa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2crgdfuge.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uymceryw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pguztboe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzlhjdli.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tmxjqogb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2skpwupen.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ixnegkmy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltmdgfwg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uyjblcvo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2duapkgdh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nxtivlla.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wytdmdcv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ubngaxdx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gplfnmnf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hzweehay.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2suimyili.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2minbrbtd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kwtthpri.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lufailrw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rfkdhjjl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tlwbdshm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wsnjaanu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nyydqsky.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ukgbioqv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hnzcfvfy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2esubrysm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xhsipqcw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2trcbefkb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zgdewxzh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qotiktvn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vqxguxuj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xkjeqbdt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xmklmabz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jhqphipr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pamkzadf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rykiqkkw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2rllkoodn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2snrgliru.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2efswnafq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2udgpcmps.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zicqrofu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kznrtmae.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2azeyamuz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nfbczhtn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zwggnbzn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ibmmcneq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zsenjqfd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yytsaygs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ytvqzwal.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tavshhch.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vnkwbqhs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2phxvjzwt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2joksmobj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2emmawcmw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iezpmcmy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjqjqm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mlqrpbct.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rahzswzj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2epgwuorr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jcysoydh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ugoyyhnm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pifpalvn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2apmovmpd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xzazqonw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2aazjxkyz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dpbamqia.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jmntqqxj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mnqiqlcg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fawpunrt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nivxrrws.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2peenrlsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2eudtnalb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2euggxvbe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2uhwrnpuf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pynzdhqg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zeaoptpj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqahxxyf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntpagnoj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ehorkmto.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mabkflmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bsybncpy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cyufxoth.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2phschzca.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zcruzgld.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nzirhmhk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lfsrjdet.html


<!-- 参考信息 -->