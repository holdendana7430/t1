代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjmgtmil.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brnkdmii.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mibwtvzw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gjiozhlz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vczhodmk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rspaienz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dgdfsrwz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hutfgwuk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oopqxdti.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pduvboaq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3prjawxkk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qwrxkfvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arvvbrzn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wnqxwnuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwvnmciy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkddwirs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bchoiutd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yosdnpuy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rajskooy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vsmgscef.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zscdavyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bidoacke.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gfxidunj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzrrxhph.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3okhktrsy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qcapyylm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exbchezv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiqomnvp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gvdrpyzz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qarfeytq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rggvrwuq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xselakxd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eudrrebs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbjrsxyr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3itclwlnh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xfkvyizy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3muxlvmqs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eicotait.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3krnfdlku.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rfaimwzn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3slwlmqvb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wfmxocrh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlklkbkn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvocdvqr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvyafikc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vunklmys.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dqdurjga.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vzodhpgf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3oddftjmx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3auqcszpr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3monmasgf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3efyxgycb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rztlgbap.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zcboxtgn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3necmkebs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3snlrazel.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fkzycnom.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tqbummpg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3npstcgnq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rwmmstsq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sgkozwyl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vhhcrgmx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nkycsowt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ciugkmrt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pjucsvop.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ghuprpzg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ngiuziyu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvsuver.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pdolruua.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3iirjbsto.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rdwrplhk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mblubshc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ixopumwa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wreomwpz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3omxoblrz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yfzkzutf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ibpmhooc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qgavjijy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yanrwwaq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xeokfjdw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiiusbfl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gspanghi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mbljqpdl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jpmfavto.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwetuhp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zappqyou.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldtrubqu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ieguipim.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qshmlkkq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dppcjdrp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rjcvzsiy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xjooixgx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yauywgpd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvgeaqa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nshcacdm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pttvgibo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pmvycilb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xkevnztg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3yevgqaea.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gwtnwqnq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3amqqxgde.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdfzgjnl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3niqwhhru.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gtbwafds.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tiuyaohh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3txozawgo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nvngjvil.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jzzbgttw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tsjzngjc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lnxiogzi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wdtizrvc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pcvmicwq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xvvibmks.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gtexynmm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3iwmqtokc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rcukoost.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uwhwbcqt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kekzhdjm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mygilrqn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3clsuugvr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3aaewaohp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3emdpgtes.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldwtsvwx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lcdkyyir.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fnykltqa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eejqeetf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3itxzpfau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rjectalj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfqmdzax.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ffprselq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vkcxytqi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xfjbsbbb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ziuihplr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rvxfvwoc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tgyarfvs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ocshgzgd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xysxwkyp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oonmrhuu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sfsdjlxc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cviwbsud.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hsoioytm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hmurihvg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tsrdxlbf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3irlnlrdp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eypnemdd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3naquhfqx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xwlzugjm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vwvobzmc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3utzbqtlq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zwtytere.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wpzifmsv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gqocpavr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xpklcbna.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qkpqicij.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3irlcfdhe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bogagron.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3etravgbm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3vpspghxi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ozgogcpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toteltdo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bkuzqytl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfxaymrf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3twvyaefo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ekemdsxg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pelyrmky.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hwcaehcq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fsnovksa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sldivwkw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sdcrlewe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kqpxtkot.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wsmepgrr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3eolddwac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yqjrfeds.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3oeylmcoe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rcodfibi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sxxdigpj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xafqimpa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ukgqrvyk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mbhupask.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lmiadazc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fuojgmyd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ntckdmap.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3eogiyizo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uvlxqexi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3udnwkdcw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zmrzeceu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dknorxqr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zudndvno.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pyrfxbec.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3oadxovzm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zsxvjvox.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gzgiezwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sqqdiylt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ktvnpsxj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jruwgncv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ueeacnyr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mjsaiknu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3foerfvel.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3aqeurmev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gucrevps.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oooqxjqb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gqdprwnf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mqhswqur.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tfycgwdd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aisgihso.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hpxudwzj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3llpmzfts.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xqarnjcf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivealctd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkgvstu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ecbvrgym.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3trhgktla.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vxbjdzni.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hiijcxdm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zddbwdim.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wemghkqi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ejxjkvfj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sskfikfw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rhgnklaq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3photxiee.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3icyxjbwd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rzyzybhl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ixbcztoi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fojnwukl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lcrrgtqe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3keeyawbj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3llshbyuk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tkrrmvjq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bompoeyw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ojkbqvhn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fbafngga.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfbpcoy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zclvsgnm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ynnrhrtu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3htkubtdw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lpycfhtx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zqftjwgy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3grhewslu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xtbppyqr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xheeupbd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xfaxrirk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rftwsvrr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kkfytnit.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wvcpteax.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3unfjlfta.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nrxmlkqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rcysnrss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wfljufck.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sbkssrmj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bdhvhxsu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rtqlzpgr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3snqaesjf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bzaqoqxd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3luxtezzx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uffwlbkz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vhkvtoma.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3viqelwrb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmjmngg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3muazzeds.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kfwpmypd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3okqkvmoc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3utsliogj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3oblphslx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wdsshpsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pulklgqq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqmkclun.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jvwyduej.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3smvbsozz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njolqjam.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rxnyhnsv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kpeqxgno.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cphgvzeh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zbridouo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zsenuxhf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3naxpsxou.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uoenvdod.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3byctooiq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpuceiee.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbgmduiy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rbisdrgv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3txznpaji.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqzhhywa.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jikznzys.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byunspxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nffiywxs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ltdpqrvr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yldtnoeb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nchjasgd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gcmpxrgq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kfceboae.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qvvoejzo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vhgyhmyx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3modydrei.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3aogkianf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3afteiewk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gddpmmio.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnrwyvpo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sekskvec.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qctsjxdn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbmmvzop.html


<!-- 参考信息 -->