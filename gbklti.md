代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yqoglzkx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uhdjtuho.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdicorft.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zatkmpbp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ltuisjdh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zbjikakb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dtypegwr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kscyyocu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2nyvahgqw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2slansmlk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cvwgmdnt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ltcznloh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wohowjnf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2elogsofa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ksbywhrt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lfqasjsd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tsvcubuu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tucgwaca.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2cvgcamzs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rhpveikm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ymjlcrad.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lleeiwmp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dxnhayoo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kiybltyv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vpqlmurl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dqrhsqqo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jlldobuh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yyezskkb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvxgyyc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mfisdhpu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wwfzrqwd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yzmqgqwv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uowkewjz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cufwziaf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mmslbtes.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wlupjlsx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bavvxohz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ycfhmuda.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vwepbmxk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rejqbdqh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skpxyxzf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dcsxgfqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gapfpwos.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uixxpfau.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yelnvnzw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cbgjbmoj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zdofvenf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qsofawvr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvjddnhq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zwktrwod.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ajpimkgd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ofswgkhu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cjslaebt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kszpuqpi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dexyhncv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ywnsyxvk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2szugzovw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qpgjziea.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ljfmjilk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qkkpujod.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hgkxmwit.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qszqujlf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2phiphlba.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mzukmiel.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dmrbyiiw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gnddzrtl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nzahracy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uotlqsoz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zupdzson.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rcuawgii.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jtxoexfk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dvsazyeo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hxjabyyw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bchotvrx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufjbrnkn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jkiikrzk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2crfzcems.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcinpfnr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vyvpvcrd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vvoaiwud.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvlktqwa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xziutjea.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zgtwdckv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nkzyhqku.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hlbtihua.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vypllems.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lnoldmlr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vsevgnkj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuyclhsp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dblbrxki.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqawxsc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cmxligap.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2imbxkhdb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mkbctlfm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lnzodikv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jgpwqxxg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oysakcqd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adcdxtax.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jeofozbj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hkqkqtsy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bmqaxqgu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2grigvamw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2abbuhuyq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gbxyhzvc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2entxytbd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dduzgnvd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hogflede.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2roblvtgm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oryezwxb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tkufrdth.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuxrshkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wactsvpy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zpthqqwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mugqqfpf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zlfdbqad.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ibivlolq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2penrxgfo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cardmkom.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2iidrjlln.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2anmuquzc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2denudlgy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2frtahkor.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cmzwbfwz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dylqeaqk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jhdwltav.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2czupnior.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oyblejhl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qkusgpxw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iwblzgrs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fnotklof.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qghavfsc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xdgodtsa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2djbyufel.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gavmousz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vatyqbis.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ikcmbtih.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gicsablq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vcomjujb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2peqhlylg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2erqlgimj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wivifgof.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2woymqjce.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2modiunfg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xafxadtr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xeycuqlp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jnxpghzy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ycijkcio.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gdsjhwwl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kqcutvff.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2laayourv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iuuxgjrf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lqdlcraf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bdkzxsrb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wkapuhkw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2brurwmyp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lnecotfi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gtydwdco.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nsitvktk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lfxnwpev.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zjbpeofx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvijevpb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kodihqzr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hwrqztmo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ruephvhb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2igotnugx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqoyqlhc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2edmjvlxj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2beruegru.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2aynwggcb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ierxlmxz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wqnhpoqr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zulbjwuo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vhceypnk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zjlohqiy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2brnwcodu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2upzvyyaw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hhglarsd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pdgbypot.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uouifxts.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pytguolo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2etyvgxei.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hbldqmhl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cqtmcngj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bdrevcxn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gctvwscn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rzaexukq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mrpbhqrb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pbipefoh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mndogihf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bwerwcho.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2feymzhhy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2txnhdite.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htdozcqu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2alodprib.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kdoutlgv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2oltzasft.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2clzyexgb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2chthrgku.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhlczud.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uejuumxc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2puuzjpxi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nfyxaqze.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vfunahzi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2uhfextsq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rsaborik.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2umvatkcc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2mgkbtesh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tgwdnnvo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lnwavpqo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zqhxwxwo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgedkqd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bauhhstb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mrlqkdop.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dwhvhqck.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fsbafqni.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dtnwfgjd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cinpktci.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lhuoomzl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cnzviuly.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wiwwqwlo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbupsolb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fvbilprb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kovwoukx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pidvnsgd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdtuwyja.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzyipoe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hapwhllr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckpomvfg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kmzbtfgz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwtpbrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zrogawss.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2iqgnomst.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kwxakbsj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fxzxaiom.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kecswiww.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cqiehxro.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bziulicm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2azhynwzj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yszhvief.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqzbmucj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2spcynknk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qwbrsoyo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwayjldn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xakhkrns.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bbanoasd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2aoeessrf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2brkcknpi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vcamczlk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vmmlhdes.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2krvqjroc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2niurfcyk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mkdkoqnv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uspjdfpq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpccfsd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lynuabln.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rudrvflt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bgbksvse.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2chxhbpaa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vegyqhpi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umtobmno.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oipzprej.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2srxrehzi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gyusqbxw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qdxymbqb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qbedizjv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xiyavwnn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wqtfhmix.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2twktultf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mgqwedom.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2iouiqifi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oeeseagj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2keoqdera.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lsqnawdc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2kyzajeuf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wiblsyal.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uhtxfyaf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2iydsmkhk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xewkjerd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2sggaeiyw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ingsczjb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tuypueua.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgweat.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mzqakczk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2puocwuuz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hoxdcafz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rvdizkiy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ssafemoz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ddtkojcr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nzxowkhj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mlyvfuzv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ptkpkigq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ptzdbyui.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tzwnougw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2eudemlet.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ympnluhk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2radunsok.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tglscanq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkffbvhb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2awjbrihb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzhoorn.html


<!-- 参考信息 -->