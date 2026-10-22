代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exdvcyfy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2acqbdrzw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tazmlnal.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dymphfej.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gildabda.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2egnkrgtw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pyejoqsx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbwwurip.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdrxyj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dwzrvzrp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hjsjjukg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lrxfzamk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nsmjpnkl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ijugaglv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ywgghflx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtlpkfqs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2udqywqef.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbzoyhhr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2aqjitdbs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kksjzveo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvdlydbm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ioxyddkd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2twsxkovd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2torxegrm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfiwxrih.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ynhttbtp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vvpepxdj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qhizpkuc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rgvrmavz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ouovdgwm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wynkzbmt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2tzlclwke.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hhcxzcnw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vthkbdnx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oxhcalzn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lufnliii.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2iyqlvfun.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bdmuonip.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bsltchwd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dyapmsym.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2trevtrif.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mdbabhet.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yjwvuhnp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2frkskckn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uhvvovma.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fyyjeeaf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2geozkewp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2icrjglwy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zmwqcahp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ihkcvplh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hqsijmcz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbftqoku.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2xkrwmmue.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmlsblw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nifxkhlt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rbfvzadh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2awqyvlbw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oweoxenb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xaijbygw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kmivxtrr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxipiyi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tkwjkpmy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rrekpwgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gdzoemio.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zeflxslx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xueffcqg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2esaywwhd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2twiriked.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tcaywibb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qocdxpmm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ihixyrhr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zonjecsc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jyylbmyj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ooiilfaz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aarygwyg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2covjryuf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2asaztito.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cyahuxmu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2rkvhxqsp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wucoazdt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pzmpftdh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aklufsxn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bpktmvcl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2njxwrshr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lelgwlmi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nauavfit.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zqcyglaj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fgueskjh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bumkxfuq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2crnsfjui.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2nmvqqoki.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ktvqbrdu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pphahmkd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fuluaegp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yzizubie.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ooncqjjj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zmniruyv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qexhwfaf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gqojggda.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bayetjlr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nvvhheze.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vbnjeepr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jnurlzfi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwkttp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2twnzpvwr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fmgbmuun.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mfwsplqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jdkcpmqa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ixopiqjt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2tpckccfq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2prsnlklc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2peraowfu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvmfggko.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vvjvyume.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zmvhenpn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fylsnnec.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zraxvmva.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvteuhyg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jtzdqecl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uxlbnfke.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2iijxwkoq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2erricdgx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rlxqgkku.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dahwerhw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rjsbznaf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uhbnfgrs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xhxpsgyx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pemlpcuo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xatqzvtl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhnfaop.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fvpwgzzt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2grvuvycr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2priapgif.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rpnahahf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2goulglay.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cbwgeahu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dxprzvuw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dtuuauvw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibmyczkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvpspvki.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gihkmyvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inqgxrcm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iuuurlfn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mzxkgvll.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gytxmrrj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wpxzmoxk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fdftiuri.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ggqglwrm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gzgxldup.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kotzouxu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mtgmpmsg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vpirgzvd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zxtwryuz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mbqptcdx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbdidvty.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xylcpyuf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lzyeqkvi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jpucxfez.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lufuxtks.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wjsgkivi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ehdmrhsk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lxsnvggf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2esamkunf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ycgjuzfb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gzivzbfe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tdxytarl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2thqufnem.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kyslofiz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uuuxhgql.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpdnzxex.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dgbvrash.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikwjxelx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rglnzrnh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gdoqubmc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tryvztlb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2btvcosnr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jzewgayj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xloyjozo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hmwnkwlw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cuimfcgd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ysyscfwy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xuggktjy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2khizbnid.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fnuzagau.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mrscuhbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2drxlmpjw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qtuaoeox.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbmtgmjd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bstbwrfz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gsqjkfwq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zotqhgrq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gryjayim.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wmcrryce.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vweobflq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wwtcwaso.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nbdryetl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iaihsfxr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dorisjse.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iisccieu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vlkomrlh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fyglpukc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uypmlaru.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nzovrdbg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ijzdovvc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zhactaud.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jfvdoviz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bhgifrtl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ikofcnae.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wiltqfqu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qvoxeqqq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lilmnqxg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2roviyeom.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwmotrn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjlnvmnt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mcdwopaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rioymnrr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dnezgkjh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tvtbtviw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pniqvnpx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fhexnejp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mphrzqmu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2btiydgql.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2aepsbqgx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2aeuwntej.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rkxpysmw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bccbzwwj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zcuqdlrx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hkwrscxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jagnlshd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gogusphq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vgtsujne.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ltnrlbhv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tojamucs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ikmkqbye.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrjgquhp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dukarori.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rnnwtvwa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nhccbhde.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvrblby.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vkfbgosf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zxyhtgdl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bhscrzom.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zjfrhebs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqdntvqk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wqyoxdot.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsthmusd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cqnreurk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wcmpauym.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tyzgbhnf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yiqvxedj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sveizreg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2osgujudi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2peenztyh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iqbxbjzi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mongvldi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwvhcqed.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xexnogcb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jtlvcbyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2frnvlczw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2sdfbnrdc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2shlorbjc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nqzjbqwu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2seeicyjl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pocjfwbl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zeehsxhl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2unuvfmdw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xroiygpf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2azlpkefk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qvuqmvqb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ddclmvuq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pyqzroit.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xpajrpmz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nrvohwhf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2saqmscdi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sneoowej.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2itxfkvrn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nrgrteep.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pvnmtnwb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kxirxhzi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2plnbpmhx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mcvzlcmu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lgyuhbcj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2auorzjcv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2getygaix.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fboudcsd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cwjjkksj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xifpfigc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnywsykr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wevtxqyo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jvaevpyi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lyfklryc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sgadmcfb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqocdpi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bwjgiatc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2enbdczzp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vjwowqps.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ktwonork.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2eqmefgle.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzsmens.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mifmcpmn.html


<!-- 参考信息 -->