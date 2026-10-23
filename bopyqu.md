代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qvjxbqqb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hadxslai.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gsdtuymh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lfvzsseh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3znfherjf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sfmtgjjt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jlmftzwr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rnbzhupf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kupyybul.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxneyxrf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3esjhpake.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ajnnjnue.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wkufscqo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gszrmesh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3avbtpcpg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3saetpmty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxzlazjk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wzkqogvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvwogmyp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3clemmrzc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bonqiqcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucygtwax.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kygxiwec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kodufuik.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pykypujb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wtxcxajm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oesrqijt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svxwcnxs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3gqxkjkpr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tkujrjvl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xeijtcep.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rupmrwgh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zhzhtpcw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hxbbyaax.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mwvtgbcs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dnbjnlcf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mbhbveuz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvxvxccv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3reguukcw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3usdhdlrk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dzolacgh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdcibjts.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3toxtgtgu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3oilhglsb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3iozwhnyz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fqqmzvqu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mbtievzz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3equvpyhs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tsneyszp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bcrldtsl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rmjsswqe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3aubaslht.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qdzrskyj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzpfmms.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfznbegx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vsunrons.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xhucedft.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3emlatyko.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jxioocso.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yhtddkww.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fptrvkrh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qlqsilbc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3gzkktnfm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ordbxlus.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nazfwemh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3pzmagoli.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vmyykzuk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qxtljmte.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qbsamwxx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3cdakzjia.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eapidmgv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cdqmetgr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bzlyjdfh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zznkavnh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cuamunzf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3alngsrov.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zgzydzwg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sphckgur.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lkcuezgp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bqpfuzna.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqdcefv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3daleosnw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ybycpdio.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kfmmapjp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rewlzbyx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3llopzhlm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wampuiri.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3tbhhkedi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfyutbjg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3iyqkkaph.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xjndnbvh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3aribfhja.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hspysdif.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gllpjxwj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bgtlcokq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oaezgbnk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qpljfwlh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hswlzckv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gsxdpmir.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ontrsqto.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rzplwcok.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wknnzpqr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rhvwoqio.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xppbcict.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3idusbwjy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mdsrloyr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3odqknldt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ucbcyvbx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3njnyhlld.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xkekdgnb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rzdumytn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mrjvptxb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dtsmbyox.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3puwxoczz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3umpobjxv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nyezywta.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gtmqoguu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ihedichv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qrerrxhb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tahpnrrj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3quahfhvd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zntdewgi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aacmrrca.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3osgkayjx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3muksltdd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kijdrsyy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rphtrldd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rquasigz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jsfuxnmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dzgjoqfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ryhckqxe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqpbynrq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zxzdwqqt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3csunytdc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xgiaxknl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bdgcekfn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vfhaqogs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ehvqoedg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dqqmxmpa.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dauiqsev.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3gbrdowhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jaqmidoz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xnbevptv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hustmqis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gcglbjnx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zllzrcdg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vmunhzck.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ktttqmvi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjqkjuob.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qzfkkadq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yyfxdhvc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rrrhywxs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3netcfuoo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qxsqtknh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3upcctwsq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3djmcbimq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vbppgwqy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3udddpdih.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ghloiulo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sjbpcxpb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3atqmwvdp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3emgwkolz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yzcinyme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwcdorth.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3welryqtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvkjxygr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rdbflfcr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cfjfaxwj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aerbluuz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lyxhzihr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sbqygsiz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3oyseqwjm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kyeoacob.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3karnztqt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uapqcpsa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rhloiccw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xirgvdsz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cqdyokoi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pstbecsi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3trsbuxlc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kkhjaoae.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3lhqzacsj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zcctfssb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxprmjwg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uzioyuke.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jiiatxqn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3afvmlsge.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xydhycyv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ptxvecxd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3apiozjey.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgtrrjf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yuylfslo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mtkxcvhx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3emuvleso.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3eupjxxhd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ridsgpio.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3swbnfzfw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xcjltsxz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vfzutpam.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ncaqeziw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3selajcjr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3owakoabu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fodleheo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ujexjpzw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ramlgvit.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3njlqpyjx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nfzilrwg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjnfayw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3twjlbequ.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ldofadwl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xomdvysp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3avtyqmvd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pftzzlol.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wmdslkvv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qylwpcyu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3grufywef.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3uoarxnan.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dyhzfxdx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ehkiyjrt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3shmdpvll.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rqfynusj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kthvrpbm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iohkdnig.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3utnjcsbv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uuizmvvb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qtlmojkb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3eggemrax.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jvdmokdw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jnbihftf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hfvipchz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3powfkkre.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3znvgkbqk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fbosrodk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3yuhzjxng.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hfherhvr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qrulcege.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhmefjb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wdizuqrk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zxmzyvmu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3paetvuyn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rivjgiuh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cjuxxuiv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3iswopgva.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cmuennbu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wycgykaj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cfwznirf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3clbohoqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3joxrfjgv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3elqjhisa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3owvemegt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3idalrevv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3euururbu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kibtairv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rjzezkah.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3clfbdzdn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3sajzhbtp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qyhiuysb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hastlkqh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqfklywh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gomyvesc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3aawkwqic.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zfflsfbf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3txbassxg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vnxfuyug.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sxkakwgr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hoyyznhh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3awogqucb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxcgbqax.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3foxlvvrt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nknrojkh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ydryuith.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubwmoxgh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kgdmentu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vmnxoctn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vnilfqux.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lsgntzbf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcytqnvc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3naverzbh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ehusxhxx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pvqubrvi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bmrbazlf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pdueqgug.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jbcqdacd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3enwhdqgb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fsjfybef.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isyohgce.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lghifrjw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lothikdj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvhebiwv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cmfcxudl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkgghtjb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3feskooqi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjnyvj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eavcxpui.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkgxppzv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3birbxahh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wainrqny.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ypugtzxx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ozzwcoeb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dnkuqdau.html


<!-- 参考信息 -->