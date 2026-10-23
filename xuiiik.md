代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tlgexqad.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hrmydaji.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pheehvov.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdhpuco.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrvkppio.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sboigxpe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3avhvwesq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cggtsyxv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3aymwdxzo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xprhnazj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3neleqfiv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zisnndyd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tchskvmc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cqstlktl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qxexszvn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pzihgzmm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3uajyntvv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ifjgmxlc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rnyznmni.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3czrteymo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3njnjjwew.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cdljynsl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xzeaeotf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hjkawlcm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jyubwgjg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nnrsrjqe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zxyjrurr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gbvhdtzb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ittpftvr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vnrqhhpu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ojturtux.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldsxaulu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jevyhwkv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ngupaevh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hbtbgcll.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3eiwdcwfw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3icinvbmr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ptasyhph.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cbcjgwtv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3gbcbaeeo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygcspxsb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwzedvea.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvitjnie.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kbayokal.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dewdusrs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rncujypf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rbliyvod.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3txoedmhs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gsggosig.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3grykxwav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qfsodmgq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3orcfnbne.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3illhzwau.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ikhkfkit.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3npgtaxmc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xuceodzr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sipgvwjt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3euhsrcpg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nuxsrkld.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rortbcgx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wxnllqvq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vogudmzd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vwmahekv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3awxasxbc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jxkzwfqr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3smxcoeuj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pysmqlaw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yqmwyvow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lqqhzseu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xtytdtqb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3apaylgmt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ljtldite.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vyvooqdd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cikritcg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lubcdwdd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ghuichli.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fwhuskgf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3oiizdsyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3omnnvjeo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rmgzboww.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3syuozopk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eogbmrrt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmjqedcw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rvjkgqqo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3osbqqcdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kgqlmdsj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3oczqvpby.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjupdfod.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hlnybomb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ufgdykus.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3iknzdsyw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3inrxxbfq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qjryjeoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qwrmculy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3noaxviag.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ihqztsza.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tgzamzov.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qemfdhtl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uezrihdu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wcraigle.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yjpglgvd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jwthfnns.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3coduxmxz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tyuyrjcf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bksfrzsx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3weealrri.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ebmduwej.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lhrazjtw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cfathszq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ezpiruul.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cyrhfplo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ouepnygd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fwnpztcw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tjcthwhj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wetktwgd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzbxlntc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lrushvyd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqiccxzt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovjlmnas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dczypfvy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ycjfyxtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdrupzmn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3goufuxdc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3suklhrmn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nfgjzdqu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ejbgorki.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zkkpvvrp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uokgifkq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yscxxywb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3mxslnuxq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hiaipehu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ppygmqxc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uuzpvaje.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3chuexxdz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxdgoivn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3izajlzjo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzassjcr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zkvxoweo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iegjkuks.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxqgczm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3nugknujl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ngphthav.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ofnyydir.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gadhqjsh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3crsotmuu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3apjiaenl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zuvsbctl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ettqrwik.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3diwdblif.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ygavlhha.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvdzgsh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vxqfuqdw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wkotvibb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wktvhjsm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3drxisqxi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3puxmfksn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tcfudmnf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3esmuixhf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lqzuaqtl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vwrzklub.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dgmeyyrq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bbepbxqh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lxosbjyi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mwtspsyi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lixndfsb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3prpvkyib.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dohxmofh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nqtebpla.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3flarxmwu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3weylwrdv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yorcygpv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xanepkhq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3degsufcs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yximbtoj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gjjqapcy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3oqfzlvsp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ruxronmk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tjdsycol.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vlwpirub.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xircrcdj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3syiipmxo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fmolejst.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zrkreenf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xflidlgq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nqxblddo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xhfxmuxr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3udicgyad.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sivxzkgj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3amdohwlq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wcizimnc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ubofmszk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3izjevalm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oaegqciz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vpyhlogu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gdemfytr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fjfidzwl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ipxytwwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tixofiii.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gqwafdac.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cbktwmua.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bvizmhsi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vswzdfrz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3acaakjhc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uiyyvgru.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mltnwtuy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3frmzvkvs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ovcykbef.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dqkbpyjq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xxjfgyqd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rpjfkovc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pocgrsmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nouwwwit.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3umadmvah.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cxnklkem.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lgvlukcv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ogvjtxkt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kwuthsgg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jinxzaik.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybdqrntu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3drlkjmnd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zzjzepvc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lokyzwal.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dsvkamuo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3negkwfai.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ptdxzpoa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ffzsccuo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xyefpsqu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lrlpcywt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3beotfpwc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iybvwiep.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3uueojjjk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lssceeli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xjccikfk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvgrbcnm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmejzhxt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ntbneter.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dyzgxhdo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3hskcclcm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rnzwylmy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3htoqlbrc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tbjlnwyi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kyxfdhyr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkshhce.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcispidl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3urymztxc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gbghmuru.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fdltkgnr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oalebsrn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3geqpmeky.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3svbmtrio.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gzoyqsoe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yrlztagd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jgvbkdsz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3agfcoovk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3szdxulcj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ebntcnnp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yculvfan.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lmszfvjo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3usresqbs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cunlzbcr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rwmtjolw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frgnpkvy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bgobsvdx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kxgoabtj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3njxazhoj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kblcllme.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ivfotzzy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwrfwtfw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wnvbpqpi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pikmnbvc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cglzsshm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3aztahaty.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kbftpedo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fejxjgzd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3brmvsdqv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zsbxvtcg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bnmissgo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pcuohjmd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kkktyrkn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jpybyuvz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3sgwbukqf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vduzifey.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nhugnlcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yrpuhobe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ozikbefo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xyehklzt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xxhizsul.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xmgsgafd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ahykghmm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pzmlbxng.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3werzbwkx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pmkdxgva.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3indlqnwd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fjzunlcg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckkjtowo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3buwanekc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ysbzjult.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3paezbhof.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yadqzjkl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qbnjxcdr.html


<!-- 参考信息 -->