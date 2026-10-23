代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpcezjc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3echnoybh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lvqgrngx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jplgzyvx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wxhkxbjt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sehuqzcm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3njewegvj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wyiovrar.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bnlnjlbj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lhdauylb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwmnqly.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3borwgxay.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwqdudq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wonwgyww.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbtkaceo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hydgmsjh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhelump.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iegktvlx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cwblfrve.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3snclgjdk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ckhvwwuu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdpjbyh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbiypwvv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ijwjhvjo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wrrmnwmu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ygrtlazn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3iprrpltm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xydqlyvw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tvmlmlob.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sjwgdhux.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ozyjcwjx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3epujdynh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3orblwzns.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wjrkhwti.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3alxnokrv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mqqniaig.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gdqgjqej.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ndgsnduw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hyiryllp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gfrcvfqi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rkgawlue.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qhkdqbaq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oqnsvbbz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ndatjceq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3czngeonn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iecgzjej.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aphqwhkt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fbcspelq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3iigvinor.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vwoinped.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lpxadobp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wpfivpwy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3juwnepnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aydgqglq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ldzywgtq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3llqanwij.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rtyxllrk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lubhsoyn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dnluofhv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hsxhkpyc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jsjlexbn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3htowuroq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lfwewunh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cprmrwvo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3myehvwmr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bvugzqpx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xgpnlcwh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lcfqdbuz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hgtamvhr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ycvuamad.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yghlhvge.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xlsqyfma.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxxwgwkk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwwyxdxz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rtvvqwzy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eposbtto.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3akzdbxqp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nrjsoigh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yfjbzril.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ppvfecwx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pcdphojh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fopjqerz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gofurzxv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgupsxql.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qbilhyjd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xgcjyiph.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fwhvyilu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddvskhrq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3krdswzof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drylopec.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3guyxixoj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yqdpypzr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ebobkmwb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gblavvgd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ggtzcymf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dwcaqpth.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3htuutobs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ridrbelj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lsvvttfe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3luxcxhbm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wgkzdkfe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jqpusrlv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jikosmij.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lpqubpyy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cecjhrkf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qpuoiltu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lsclesap.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bngkwekl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qihsiswp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xxldvvmb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3laxrxeyx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jesqxsbo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qqkdhjsn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3grglzwnn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vvztopkp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3izlpbksl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lbudwuhh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3smaeuorb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sikbxvnr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pulypnnz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ibpxusva.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gidjoubz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nvfctory.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3flcwuhom.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dieuiiap.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mstdfdna.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lxnjwbsj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3csqlvhoo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nxwrmmak.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nvmpvhfk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jlxhpgnv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iriablzs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aanlprui.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kiypbrtq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cbvbirsv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zfacvtnq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khrhahif.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cbcjldol.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yhnvzbpf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xwpvafqq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3voakhkqg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijeegjiz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cwhstpxa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3eiinjncj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xebarmyo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jtvyfece.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sgybtyxa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mleovtln.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nyqaqbuh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oaagbosj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mmdrvtct.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zruthlzt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxqbhae.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3doncshfo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wodebkok.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sqooxmtd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zlddvfku.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rgdbtdnc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oiuagoqz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wkgstvco.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmtgkgw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zhyebuoy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3glbzjiql.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iivbhrut.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rpclqbqd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qkqeabrq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vkbpnlrl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3palcatqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzaopdnx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qdfmztwl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3cbcyqwwf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rhlwczdm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qfubcxlx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rphsklzr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xztwdsee.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhjalmj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wmykkjnx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rqeyktmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pejbfvlr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hzdckjgy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ruueewrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3atccyjjm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nuyqxbwp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pgcdskaq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mycsozsn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yicpurvd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wodciitg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lfekoofn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3npqwbltr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zejergoh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3crgypphh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pppcalxe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avoyvxss.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ecfcnfvj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3cgccwyce.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jjqwjati.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xruzenvt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rrpkufrc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ffhkwasf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rxagvlrt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wyfizydk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kmokeqpx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yejtsdsu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpcwcdft.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gjjdtygs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zpfxzbzk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wjemweqc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3idvcmbmj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cabpofob.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kodxwnqn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olmwlxcy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fvpkcczd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lidcguyx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ezvlipfc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppthinee.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qiablvmd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xsaiinws.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3slghqjmr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxviwwuh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qbrnfrbu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3whfkruil.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rqctszvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mykmcgiu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ibydlsao.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vhbxknld.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hgzlcqxg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uakpoxkb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itheiath.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3acsfmbik.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3conaitna.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ehesaozm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3axzpmpez.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uqbrbslb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vjulucop.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3eeosdmua.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpixdsa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtqscxyi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxevadx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rkrjekuf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dcghoctb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxukttfp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bwxdmvus.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pvzngnfi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ellvphow.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gywpzrbu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kizrcklm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yjofihns.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gwybyyah.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dwomjapc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tkkwzmuc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3invytvls.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bvinyaxh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3scmhyhgf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3osbfkoqv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kisgmzvi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3yzvihuth.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jrefzpfz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tpwcemlx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3okhidvzt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3feceqiib.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3mpvjrsnp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rpxzuvco.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkwsgmhg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttyjhxsq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rzgluopv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ieabrrgz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3tsndkppv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zmzgiafp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wmxqqvfo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rtahixeu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3oadymxse.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bnghqlri.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ywkogiek.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rghppcjb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctxgtpjo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfhdekhd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ltnojpwo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jiezmnjg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzzkacyf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kqnybhcz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qizypoka.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dkagqgws.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ctbspimk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rivlttum.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bcpbpfpl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3twirnuer.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmloqg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qoewuxno.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ogwsungn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkvhnul.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ebvrggej.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tpquaphr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hakrzwob.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3yvlxhyff.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipuocrwf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pgpozkax.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dfdgnnxs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3navsbufd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3keujwuiw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3uqyjvkvr.html


<!-- 参考信息 -->