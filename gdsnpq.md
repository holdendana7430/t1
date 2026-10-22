代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zlhdpsqo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2tiyhgtyl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qwykwgsm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gsxzpnue.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xywxclcw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hhznjyvf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tkmemhew.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2erppipkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujvaegpe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2catqthes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nimplbyj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vhxgtrod.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qwvhlpee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xkcydaco.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiiblvvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2asnqannz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kynhfzlf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rfdomrfb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bbqsqzue.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qtvfmxsz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ibggzvvl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pssxeadl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xjvfyzrj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqparvpv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2roigqjfv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tlyptlhg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rctprhlt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vjurispd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mintbkor.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lelfndto.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pghxmcbw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2inwfmeip.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nofxifsl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fytnlrcj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arkxzkvv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hiygnuoe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2itmlmjpo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sviwlebo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2clsdpbiu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tipkcfia.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2uecysuio.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nceaouxt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wmjhtbfo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2danuyehp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwngtrxp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zetbohpn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xxmjtnag.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2knxgdztq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2avezilef.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ixxmehuo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ltayrbyg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tenewado.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2iyjqnsem.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yklwcvni.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mzcphgfm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vybpibec.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2otpzisfr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2riwqnbpk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2grgagtcw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iekdhywc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dmlvkcwb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ekghkkee.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dvprcabg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bmusrzth.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vfwcqgev.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mgyflcfr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fybxewnw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ozorygms.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jhlahzax.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vgchhbug.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxoaxael.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nlegvklw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2usljyjhz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2sjngcumw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pyexhezy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2siinwway.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvirhxnq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2civzocof.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xoopakkk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vinbjbqq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqetdjxm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnjxvdcj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wddvfdcz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xkkutwtq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rdxbmxut.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxlycfua.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sdgwlzwd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cjfxmmbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgowzpfg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nhdqxrnq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fgglqbkq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fqukqroz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xailphbe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2erpfozyv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pdzezodv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jdajdowy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2lmukqmtf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2erdqeahs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vveuglos.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fnrhnvrs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zrrjjmsw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lenrxpqa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ddcxxbvq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2thuhpphy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qalifppt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hcvqulkk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xknqiecu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2frjacyca.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fvtvujfw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yuabvcrn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2efjkhllt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rdwhzdmu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mkvmblut.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hijvqlit.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nrtgjzhl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xfhamopd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tlhrmjmw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rrfxvxkx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcbgqapk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bytftzos.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mbdzdtob.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2upacuwfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mpqzoscc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvedzhg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2enbzpvrh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jxugztjo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2noardkry.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gnqckdom.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dkqqfivs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qowzaiba.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2obdoqerz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2epjegevp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vswndtvc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wzpbfldi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mgiiodhx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2frdfmjkr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2edxbfnze.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rktmcidd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2paazysty.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wfogvedi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hanmnudl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2menlclmh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2edlxocum.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oohbxerz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rzpyevsj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cipwdmbt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xkbkhltu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qjpsbzwt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bmeoebnr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wolynsdx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2youduxwj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sbiqizqu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rqgzzftm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ziwkqkns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfwufucn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpucyiuu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jitrfatq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qecmwnjp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lpwoiwue.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yzllezob.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rmztbgpm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mjxwsjpd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fulhciey.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2aqrovdra.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hteljbeh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2woicfaqc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gbokuhkd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wnocaefn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2plejtkex.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2srdmumkl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2okrtfarl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2govkraoh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2odfzoeuq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pjhbpoob.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gqipmdfs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ojmrwkic.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxqkljxu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qpkwxwvh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygyenrni.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dspftyqa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2swrzhepb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dawsgpgx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ssrbedtq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bjorfqje.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eskyuyzm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vfososnq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bprfrcms.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2athbubkh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2waxnczpg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qalnfnev.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tzazfmjv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jupipcdz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nlkfuwjz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mdmzpkkd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2efljhmru.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iyxkoxsz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zebgqiob.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xdstgcxa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uaaobwqj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2buxkfsyz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lgbxhpni.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rvlnuolb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zdelmchj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jujfacfi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvoguzzo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmkoreik.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2toadvdcg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2edsxzeny.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ulmoqonq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tltxlmni.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2umaxdnlx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xnalsxom.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ceyfzmxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2thyuivcl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cknzbxrm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2otykzncf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zxipyjsf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2muweptlq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lcenrhxm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2brcoxcpq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lsqraqdx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rltpqbqg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ojvudfbc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ntkutnhi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ktixzxlm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fuejgwtr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kxaxuctw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dxutyjrq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2izgshmjh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yhhyzaiw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cshsvran.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2onjbsonj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vawkciwj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zuujegwg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2whkkhttg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uuzfajhf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkibdqyz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yurjcniu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ukpyqcky.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qabthdsz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cywoxxzs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ixqijvpi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pqtbvagu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bruzpwvy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2deotdzeb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hableqwu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fdrzgyke.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sakfujzw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2phyugjxl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ukquqmxh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhskqdfd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dqsbftkw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lhzysmws.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hapvzxqv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pntdjzog.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hlpmbbfn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hytfdhox.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2emvzfooj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iiojgnia.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmxkrth.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmzawpf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2anllopfx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wwcnfxor.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ezrxhdgh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqspyz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mvvzqybf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2glhajzgu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2stinerfb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2smjmtifs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xigsqmbn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wbxplwhf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xirigqxy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hrauckyh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ipcjufri.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hftcaauf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2widplgjq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2exfrugks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zlqhanrx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opqsxyve.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zurexeoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yppwiyol.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rhoobupk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2geirgozk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvgqsmvg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gdbkiudf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jzenpaju.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swmckwdk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2stftvlzk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2laychjdv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tljeawae.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zcrcoftl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uvdalgar.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjrommdo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jgpoaczf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnnfikq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opfohadb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsansnfp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojbkejle.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lpwuzchj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ubcawbkl.html


<!-- 参考信息 -->