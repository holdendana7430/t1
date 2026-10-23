代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tcgdvrtl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3znwjrxah.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3csgmucxk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3oyavzfgo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3cdxqmgpa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3guurvmke.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qpdzwtbj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tqeuvfvt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gbjyxazp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkhdhjp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3flbyexbt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nxoeeoeu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tzkbmyuz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zqswmhmu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3twjbkfir.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3etjtouxh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3stydaedq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebdiyyvj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cjodzcbo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pkejrnbv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kfbyizet.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tqkozxil.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ucslkfio.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ckmyjrfw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oupqecai.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3baettwjy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jzjgjldk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mrdswsmw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zeyxlttj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nbojjqaq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lkzukpms.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fdimqwad.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xotgecdb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mrqelosg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3abqstavk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mpcutono.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xogqfyua.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3tgxrjjpe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3iruycjlz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nakhpswg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tgzdsbhq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gbdkshag.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3glcvvwia.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3irauncof.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3erznyafr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ozevoggg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xelegfoi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3iamvgahw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kjaoqvps.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jycawiof.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngmkbfgz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3itydylju.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mropbaui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqfarbez.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lrndleky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifoyevzn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pkvufluy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oiothpqb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3befmyyet.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kcomilos.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yewufwio.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xixlxbgl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ckccuktk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ozmyyzqm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynditwrp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3arfyxjfx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yfgygrvp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gdewrypv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ntfpxufg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mltdwqjs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3itulddda.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nnkqqcku.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlskcczw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usbdizuf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hvwhchzb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cetlzjth.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nxtzmxtx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fvnuvyrx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ijzeyjqt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lnywioty.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3afqqzbsf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ywsbvrkv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vjzngbzs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3worssoml.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jukexscf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3upcessjq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kjgajeil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpydlozo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3taowfhxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlllwdym.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3exbwokaa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mcdmhsoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zbgzqfmj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ykmspdeu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wggencwo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3crfcqenb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yqysayya.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3blzbqnsu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mlcafrxd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mvlwxilp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ddecsqjb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kajqkymn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bsdmuhgh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tcrzvoxq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3eaomhjtf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ufmtzuuf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fgkaikwb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vqovteua.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zvyevsot.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qnofzlyr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yavspdyr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bdvwqhnz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hkiubabn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lslxlqnn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3erfrqfsb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmktfsu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cdzrfssx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3iztegyly.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pntzlzya.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtyezhsz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kevyozja.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hmbqgnua.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3agbhmcxz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xvbhhgtl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hmflogyq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tzloxwjt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3seqivmxw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zqytbrit.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fcxmljbx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3suismndl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3eziqezae.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fyimppgy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yocjgfqq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hrmiknhd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cfzksuii.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hwpxjsyd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amwziloz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ouqywbum.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mmozqssa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qrywtjyh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vszbjshi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtzksbsk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dctesdyc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kkaldkjh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dclpxuvr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3njmiacxf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hxrtjufp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3acibwoxb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vnysrrfl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywzgnzdh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gljxyuel.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lgesmeaw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qkjwcfgw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ptdylgor.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vztozyfp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cqgyszrz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ajrggbiv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iywckozb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uotbsdem.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmmjidq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cfwyylej.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bbfmehud.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jrnodqre.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uhckbouv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihsmrqcq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3walmtmhv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3faapzefs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zfzzkssa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iymumjpg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aiwscivu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hkuclmbt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fqzjjpmw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jemvizsd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3roxbbffb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yysftgwe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvzjnup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3utoykxzx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kgotszbv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gwqlcsty.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kurkmrzi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hkjltotj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fvgrelii.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ckhtvfle.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pbxrsgvc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3byazzmnx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wlibejry.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojrfgkad.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dkamkwhf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ikuamroh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qvnqxszu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mdhrnieb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccjiotqh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dskhsxqp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xxdreudw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3majwvyze.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3flmvldtl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyclqoak.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ssipvsjk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kbsjwwbk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgdjagnq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdchrmdi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xukxgqmx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3efqlwzva.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zygmdjtj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zodnaopw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpirsiud.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbsuzszy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ireeiohz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bibvakxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ruvtikri.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rumczhev.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3azbraclt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xjsvpgnn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mirvvkwx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pjmwtkxv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnzvoxjz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rasrbdwd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zxhljchn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lduilosh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cjrovnya.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vdodoxpd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lwmlsviq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3izvvyafx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3suxhgptr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tgcwwbiv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bfsaqgjj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfbjvlhk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pcicbwef.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxrmazk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iarvonfz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mhnejnch.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3elianrnq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pvoxizhj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gwrlwrfs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3grqubusw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3unrssddt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpkbsayj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dekhurcw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ccmujxsv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wdezefqv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zuxywdyx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qlizivhk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3duvmpieb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xylbvkxn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kcfmssfz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vvpotnvj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lydurvow.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qcelrgae.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3adafehbw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rvdaxyyz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qjxqygzf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3stjftfdo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jhtokqkv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rppmnbkm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ekshswsa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3blwzepux.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mqejbuwn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xjbmcpnp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ugiaijgj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xsyjbghl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xwixkahs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ximsjtpx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcvdmbv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gwvgksdt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iacqxqzs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tahpmdax.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3stzrwwbu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fyesywva.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fmiemxhn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3panilulu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wggokzsl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3alcggydi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mzqhnzxv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cgnahmpk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ytefahfb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kkefwqjl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xmdpuxai.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvagpql.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcksjvdk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xwehfisg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjitoxnz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gaoehnse.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3feaqvehj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zykeacta.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3prgfmhkl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rmouwqcn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3yttbeilb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3twieqitw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mujqspeu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jvmviucr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bzrufrbd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bylewtxo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3szymctyt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hazlyrab.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3obinktpf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oqtvofzn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmtxlzrm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kfqydabu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3uccasxdq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mbfubsqt.html


<!-- 参考信息 -->