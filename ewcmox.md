代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wswxumtm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wexbdnpi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dpofbsxr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pmzkarfv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fxmqlnba.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3idvpvzrs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3trwezjop.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jxoczyan.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ypjmmovh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gxojuvwj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kgnfkdrq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3flffluah.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gwzgxjja.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hgrxzwqt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3farfufht.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbmuoste.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3oaegxska.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3azphxslu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uvvuugqv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mxrhrcvn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvwagpr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xpkcxbnc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nonqmrhv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3iviotmpm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3aawrshdw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gnhtxmts.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cijfexgc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3diuwbyaj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qjfqkpib.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jegkqiae.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rpbyvsqq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ccxtoaxy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lzwcviis.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ihwhnlmd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qchapkro.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pssrdorj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zjrxsqdt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3uhzeuvjq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vdkhufel.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjfjyw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kwxcwglb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nzmvbuwz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tusbunzv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yincvgyb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jfzlqhsu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3frezcliw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vvyzjrit.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3adeczxjv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qvdnqukz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jferknfy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3awqonqwp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nibfoqoj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vpdmjeaf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wucfpjcy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vsbkuuwo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3atenextq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uygeqbkd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3toqihjrn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3huuvcqhj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vnyjmbpi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xohpspja.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3buvkncxl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3byeltscx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3uracooib.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uultvlxe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3apwddqfv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oppretjc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pktajwlu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3flwebypm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3haknsrga.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ymswcput.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbetgceq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jznhvzyv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3csqhdwul.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mvszdwli.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3erkllary.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sljkxuqo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nedmmgtq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3olevcnjg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3takycywk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zofnvleb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pklgmjvm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ktmnqoyt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ngrwbrvq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vdnqxinl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3drfhnfrf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnxbdl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vmgankmz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qogxambc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rueedmpv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gsbtdahn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vrkwoqxl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hjqwumut.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cltzyvdg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3cnieqxjh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wjbftfhc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jtgrbjhh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qlabmdpv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jgoxozrn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cutzdomm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cntafaik.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3weoiawfj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ooomqaxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isxbsdls.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fogdhgry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thhylshq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mdjajrhw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3srxjaldd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bacogswl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aqygofde.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vcnddlcw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zxxjkhds.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3awxrsbmg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qxoywbos.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gjwkgxlv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xrzvemdd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pcbvaybi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gbhkqqsp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tztabzml.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xjfxavba.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oltydlmw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ftzugjpb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3opvapffo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fojsghew.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uillrwgk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ascznrgq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wqblbdbc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tvozispb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvyrfnhv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bkgjtflp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dfcipdgr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3epcsuxsy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wfsgzopf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qxmolvry.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vipqdnqz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufhamykj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qcxoqblr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfehaqch.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pcitdxiq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ikbmcild.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fevagwgm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ngirzihq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fjwgnjmt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gnetczrc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3frnewelt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jtnkzbyi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hggrozqr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hzasrgee.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lrwtrtyz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fdjhdmzk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zooaoegy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3orbyufdc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlruibf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxyuunzv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3syevfnbb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nvjzzrpm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3awchwnmh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwzkdwgz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jjbpquwn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tgkihyoy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3omeqlikd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3gpvsloqa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3taltxnvx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vnufamqy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3unndlgic.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmdunlcm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fblmucxc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ihhwbxvr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jqquqeya.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cqfwmfir.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3arwawuso.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ycrtqdyw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uyyqsdop.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3owczyxmy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3crofbrsc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sqvrpvit.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ftxfozwl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ubviuoyz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ouxyxoou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qvaryenh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dljnnuhs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ryclqhcq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ayvxwnre.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xwsesumi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lymoodkj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uigtcdnh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hnisccbf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nxskzqln.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tomeozoz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ptadtzzq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjnxxtg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nshbyqhf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vlpbmxos.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3elimuryn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3leoyljlh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wmbefzay.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nezyawkw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dxhamakq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lqyxuofm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mdphcuwd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xfiuzcos.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qmikiqam.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3avekfrak.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3aduumvzp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zmnitqmx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tvncehwe.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wfhkpofu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umunwmht.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jiorxqpl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3exfheffh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qyteheod.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsgetdm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aycwccep.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3asvxubuq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nnytvecn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3smoaftdv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3sllsyuqo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3scdtulux.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3smdsjbxl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3reggldwq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3klbpvwpk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3eictprbg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pqyvwoqy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3abcbxyjh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tgffiaip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpmhcjpm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wierexiu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3aarchauu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ixzgjnfj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cwmidspc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kurvvwjr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdiucdeh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mfbptpjn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3awwebxco.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fuchyucz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ykvyccia.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kafnunsa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iighdjan.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cuemviip.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kobbhohd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ffartost.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3icfnirbv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgthepvs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xabqgftw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhwdcdy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fuetxeim.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gwhpfrcy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ttstrkft.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fpnauigp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mpalwkch.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cmxitrmw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cqzldgao.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcdhcafm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwzniuog.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtbbbvak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wdbotikl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lsgmzkdm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3exvutkvg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qvkgynxi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tadrishq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bgxitvzv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rhqasphc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ogppulvi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zhxgcnco.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ujakvhic.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3khkparpx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tpkggckg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tasuzalt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ejwulqfb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rngtxhjv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ldhaksuw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3utmswjgy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3soiibmrh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3buidzqnc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zlawqeoz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nixhruoc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fmbhvsfe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rhirtprr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfmnhxa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxgxuypl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jgpqbamp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xmmvpjlt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jbpsqrdw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hlghpeec.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3edtfipar.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pbprcisi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fbxmzgpg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fnujyqba.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gsmcqpws.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvtppsad.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rsickkzv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vpbrkadp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vbuiudkm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fpyhimiz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhsjmgij.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3knpaqrij.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzadwqg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xulgfjcl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bscxzkyp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mtnkxqks.html


<!-- 参考信息 -->