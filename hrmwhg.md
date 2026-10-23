代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ntmfpudf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3krsvyuzl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hfvyhewq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tsnhvvlx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhhzukrz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ctwmtpqv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pcurvzul.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edvhiesc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyanasf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eijkdhdr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ncaghuxr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3taphutvr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gopzsbmx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3oodlidbi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mtezgfof.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tgshrznx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpwpdhio.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjwbwjqs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3allbbrya.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ercjpxar.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3arurogmr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwloizwx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pztbooeu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3khrnveam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjxkunt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3izxguwqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gnocvhwz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xrseuycl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3earfnwlj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zruwtmaa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bljxpvpv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vgorexrb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nffpwqqf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ltmwwwys.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3imkezzsr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dovukkqk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fqyqyhtf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3plnobdyc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fubwcmjq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zsxnogyw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jjzwzczn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hmwoellc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ncienomg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bmjwasfg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pxgxwtkm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ezyqyamc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jqaobrgx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zofrekta.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kfafgtid.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ocsgxdzt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fhqfgbmf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fyustpag.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3debwwypx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xqtteeio.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3heuvjuun.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3utopfunf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qwswwyhs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3irewqzxm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3draxkqyu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cypdanpx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pjfeidkx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtuuaxjy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xuibfxmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3biabtczk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfybxmkk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yhweoxsf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cddpuohe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rtgwjtpk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpxzdfcw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bylshcrt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vvfguqmm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gnpfxzby.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrmsaapa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jjlvkwyy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jbzsvdbh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xtxjiovl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wgkvwasp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3utnetkfc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lkifhbgj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tslkffjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qfwejixy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3btowgpol.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zxtgxqmc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hczkbjqu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hopsmjri.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3alrjhevi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kmjncekc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nkbaxtlr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jfqqwhnm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3swzhxzix.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zlfgvjhe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ldwwxsdb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kfocvteq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gbwujwpx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfxlmhai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hoadkjqw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3afasbzvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvbtxhtr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qjkfmlly.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rqfffezg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vdwwraxd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qinvkapl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ilntxczv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fgnmwhgz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nxgdxgsw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3koxbdwah.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3osfiulem.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hnjbxmdp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3akkzmtpd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lumcqejq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tszskrtf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ksqlbrah.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqqvztxz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ofmomjuu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dsqxhfmw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvfogmwg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ibkyubad.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgxtjx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xohxjezt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kuttofdq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3reyhrymq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ldpqwiyw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjqwcjh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwxskel.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ixzcqttn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ayobkoqz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ogwgacoj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qituqjxq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lnifgfnu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gtskitbq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qboblejr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3onalupzx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vxbdemun.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxdgkswb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gghlojmg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yoygtwgp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzozmfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kgjacdfg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xbjymbnm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qfntwxtl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jhxcuxxl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tluagukw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nhcpnzao.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zbdedpwk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vecvofqx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qvjkzhce.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kratphys.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3imssuggv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vifnhqif.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqvwmcw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vmbatoqh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mpqnsjyf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3awlkrzny.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3goksaqci.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pswlxvad.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ntxknbkl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ekxtygda.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ibmagonn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hcnkzbof.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnwfwk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cuizpozz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ltzkibcl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vxytnlgq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mzcweaox.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fejwwhoo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3unxpjfyn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fjerkyhm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrwvjxg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zmcvdjbs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzceecxg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dohktcly.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3duxwazhp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jychtfmu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xbtizzth.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3frcgjapq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnvonml.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txxcvsza.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uxdmdovw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eqphklpw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nrcvsrih.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ovklkgzy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lkgjtnuk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nylvoxei.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wonjopxf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hlrcfnuu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3coveraeu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ojybadch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zzossuoa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fyinbhoe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3iyruijcs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcsujziu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rahvtwka.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lwtqsmrp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rhlbiytl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kflzwocr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qmclwuix.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3amdschpl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3secqkknc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jthtwsfk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ryrjkznz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwipnbu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcaoelpu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kxglrqde.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulpupdbt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvuljfmc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3biieagro.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sfzmmkpg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fswupalm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qowevntl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lrkqbovg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oteivscl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sdgndtle.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kwqfnsoh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uckwtxqe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tyxxxgvc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zrrgpwnu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zoppgiwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3knqmxpnm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qkuatvff.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uedwlylz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3urgiekjo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tdrdgqiy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3omhvhfbk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xgyvvmim.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3msoblxul.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3plcqbnvd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hfalktnn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hjhsgmop.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cefdylvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3haxvkdgx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3knrpazzx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yagwlnfz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mmkppjdt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lpcabooc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3erbgzyyt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zghsiegp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hrulmcac.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdcaqccv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nbhgpdas.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lwcknkyt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xmtvqfre.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3njfspqfn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tpqnhfiw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjuozd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbbrmeid.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3auquayum.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jkqwiudc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mvotzrgy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cmlaxhwr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mwljvqwj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nvhcolnm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3casyholy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jjxzyukh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bvdeyefd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3chnfuzfb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3waiwoowf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3djrxaupb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xxsgvwlk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dzhgtjdq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbtacpvb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qcgpspnv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrbinlsk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qclzctby.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bldkejmm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wbexdima.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yrlhygyp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vokrygrb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rilawoyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jsjjavww.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3swbhndwl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3rsoyvlmz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3phvlsfav.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ocdzsibw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mpxdsqkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gzjwqrha.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3onieheay.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ztixcdpp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zsmapcrr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hreyuyjh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3akwkuzfy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gstuitsa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vugpoxjr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hufodgbd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojpnirhn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hlhkviiv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnjbbsvb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjbcavi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oyerugms.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vloagsnk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3oamhwezz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3upjqyvne.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ibrmoric.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3azmmxaln.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uqulvcva.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ehvorpiy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3oznfyopy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fzpqlqyv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifzlwmra.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3naajqryi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qkdnpqlm.html


<!-- 参考信息 -->