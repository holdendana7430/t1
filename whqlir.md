代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bejuupbc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pbcagizp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eyaqoxvn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jejojiqf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sfjmjwqw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hhbtqvqm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3febdlbbo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gzqoqiqj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3eulnygiu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ayoeutzm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sudnbvrf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uljjutbi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qyycfmow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3oorttonv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jebhcvyl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xtvfrtjq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rzqhhljr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zytlatuz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ngkuitcv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3byvongku.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cidavupw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yyeamvoz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxrvqnkm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkidapqg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3spaetqob.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vbhxgaou.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3efhxcayo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3klgylldv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3miojgyre.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dronpeqi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vspuxzfg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dxqkzkbj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yshbbeim.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vwxvazvs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jvwdqycb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ymmobgib.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3afhvdsgc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xrudldwo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nxvsfjgn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yeorysgr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rhvcybes.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3llfxtbwh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3imcgikku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3elqcyqyo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kkgzszos.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rcczsgej.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ltrvtryw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iydmncza.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ivjixjfz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gtbpkiwg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kpsipjzv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fkubszvy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rfqvsnlt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3evgbrhvo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yudtcsyy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aiqmezjh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kommeayp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hbggvopb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jrkjkqyl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qmnlbhlx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3naoqzsve.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3glzztbul.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3idfudtoq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3npvdtgyt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iobwybnl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mgfjsfdt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zygsxnkj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qpvvuekv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uouhhppa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3avuoeuqn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3haqxxmor.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ehvaalut.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkvuizhc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxidozxo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3txcaocmz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lvtisgyy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cuycpall.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wpovrqso.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lgesyuyr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3utfdhxkm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaxthjmc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sztdticy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3syfqenji.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qlqwlzwj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3iwezhxmg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ggtfawjt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yiaxgnjo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iruxdvjd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ppylcjay.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ixtyrzuo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iqvbnhkb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkkavkuz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lqauywxa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lvekahog.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mnghgjdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3outjkbtr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hfpyubni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stufokuo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xvhbubtu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ptphvxip.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gfxkywdu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zqnwghze.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vizomenk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3brbxtelc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3slmkodcw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qaulnxrf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cagpnumt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rjlalnvh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rjjogrxn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mvqmpxqw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmyetaf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jugrbufu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rpptawnj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3btkhfdxx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cjgblrks.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dkatetuk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lgykmuev.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nmoqiann.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pmkxvvjp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3usyfowey.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rdapbbbi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jieymxva.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3treckdvf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tpkikita.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3roafwwrn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ofaqjqci.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzivhqso.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kqvhztbx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ksxwudpu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jqpilsyi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxnadvko.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qfsjkifv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3awbrujer.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wlagihwq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3krgpmhui.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yzmvazue.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ewhtqpcd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wjvbkpiq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uvujpzgg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ivyjzziu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gssmlcgj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zrikxakk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ctfknniw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sfgkxzhi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gmbtqqmx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iswrzgvc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yvtsgoou.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3couhxvil.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vzirupga.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hgnevzab.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3eoaidjyq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3slvjugnv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ppxfeiuu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3apwinkbw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pscjvwnn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kuszfodv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cbqvetts.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hmltvcei.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yyiasjxn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vexxxayv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qresjald.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3oryngwpd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3teoebmoi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3nnrdbqry.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fkfgacsc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zqttfrug.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swjlehxe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kwinwawi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3swjmvrln.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3itmnhthq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zormkpqi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ibxinoyb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jdkdxbfu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3depupmoh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dlkmyceo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3sjlkrvrf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zamxowbf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bqrzztyc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rzocxauj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gwnafncd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bmlnzzyy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3obftgjjz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tbjxcaar.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtialvy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3fntuhtfc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3eqxivghk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3daffvocq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jtvujnzg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3llkkdjgv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3buiubyou.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktxxqrnk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ewwiluvs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ktynzmzq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3skuzxsev.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cflagmzk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fvrtzjgy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nqbujnyw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yptykpuo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jlphgfpy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sdjfrbqm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ivuyvgpb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kaeznwha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3clsmkhqz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ebdiwgvf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vexhgekd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ncjdqxcx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3iteizqxa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jiqixjzl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sjfzeate.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3umxwqgjl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tputzkwe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ymntevku.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kujrepkt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ezmgnvxq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnbkocdf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3firdsapo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fuxhbvxa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3caelkzaw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drqkqyqo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqoopxgg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecragzer.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3adwamqvs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jjpjwxqu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iubzcsjm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lctvatng.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cebpuhej.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjpyxbhw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aqbprowu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mxbpnvot.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ehwpgnyt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lfskklwa.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ucxozpbi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ojilnnei.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ignkxhrz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyakghgc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yxodessw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zhoolxrw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iltbshab.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nixmgcej.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3shjyszew.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3udvbivuh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dltytwts.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rvprvgpn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aqdleavs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3brhtdvry.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imbqufhr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3euslpwfm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bnaojhir.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcvkylx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3uutwblrh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cchdjpvf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wlruwile.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cinyejvj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tozvzykm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xiqbjcbd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nxqjgnpm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fazbjjyj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wctzvmgc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3eagbvllz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cdnpcmvn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hnynvaac.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cwzylatp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xtogbskc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3olqopqop.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3apqzuloo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uidxldii.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zturpfxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ubnuhasp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hsziujov.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zjcadxkx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckdljiii.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wxbypqxr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kudtbxox.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uczzvkjk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jwxuvfnh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3sqemlxbm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ldfprjha.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nsmtxhds.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dxvkxrhs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jpxffpqr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sctrupkx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oevnvzcu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nszxqoat.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlobqkza.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmausqbu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ewxswoae.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnggdcbz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qqhzpiyj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbephtew.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yszvikuh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zlelcygz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zgasduvl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3imwmwjwi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhjfbfi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jfadckqa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3idgbizww.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xmgbrznb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oyjwmxcb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hlgxwrof.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3myizugjd.html


<!-- 参考信息 -->