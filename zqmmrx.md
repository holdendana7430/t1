代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yegaynmk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jndfmphe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wrnizjru.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sgqgxhfm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kntrtokq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gzwvajms.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dsumcdje.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zjmicnfj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vbdvpfpm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yuiiqrhx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lyizfcuo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3deennbhd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mrilirtr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ntrjeyhq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3efffumvg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zmqocxua.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gdzvasun.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hbgbunlb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wdauyisw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jpgbmhiw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wfdlutyw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ieqjlrul.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jgkagcrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xtaonlwh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3upucbnsr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rudkdztf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lctfgssy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ntaagqid.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nrfqkykh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mzjlalan.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aozevgzd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3crypkrxd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ykwvsslo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lztverrr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxcfugvo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tpuqbyxk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3trcgmzcl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmrehdpj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ivmfzvgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yydtkcib.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lywyuxwt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jwxlxrlr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dhztaxlj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lvjfikbn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ldemrxva.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qoldeayo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nimhmrzg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iwyjtlpl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsvpctn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fpallbnr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ovfswlnz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nzffiuul.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xncpmvsx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xuvpjgwr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rvsjvgit.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qhszqbny.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkcapegv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yefcecah.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vnqxdeyb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mgcuoqeh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ozvkrsxw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3swiwtire.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3omelbkqq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3prmiacpr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ldpjrdim.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zujjtwqn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vqfogzby.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynxagnzp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3npstlpcg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uvoalgoa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rngihxmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygvttcpt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xnqnbdwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fubinces.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hllftxqt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zeusewfi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gwjpsnqi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3opppxwkt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3exsywkgt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wwkgyctp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fepvdeta.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vecafiqh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ffmpzjnh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cysttdkj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dxldunlx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jpfhoidg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3akyifeet.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rjtbylmy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xjyojbxq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rqnawdyl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qfnicgvn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ygxhabnz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mroanuct.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3geosnojm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qbtlkzjz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lwbasmvy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sldcpmby.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qvqqtccb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdlbrss.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rwmgogpn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zpngkklz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rmuikejs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iurozkei.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3augtyenj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zxqmvdyx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3htwvuilz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bmfgwdcu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bchskgzg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dolfsikb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3abvfqlnc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nbcbkacv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zenzkdew.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pbnoolie.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pwqlajra.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wqimfuyv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yrauyffz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eajhvjgw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yjidfbqm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gpendolf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mgxsgdyr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3liezizns.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jgijxphd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rrgvekmv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wykescaw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3umxckvgj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zywrqdsm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kfksaycy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3neppsbve.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hftdpshi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3srcnzqml.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tgfksgzw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ffobmzwp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lqhonyzo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kadaqcrf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hdirofkt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dgektvet.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qorysvmp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxtmqzup.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmspdrtf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qotjaqdb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ytobokeo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ruhlkxpb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dkenlrrt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xcorwdfn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qxiyigrx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ihhxpoxh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fafqfiuv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yngmvwms.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3iwpccwpz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zqvadvmh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wbelfvvh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3scocvgwr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbjhafoc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wuqbzwph.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qrbhheys.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lqqjnlhi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ydbsnrdt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3slliefda.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwbsbag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nlshbtol.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xxjgwkdl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dhpvxlaa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3poyhustd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ymyoordb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tmgflamu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ocsvamly.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pejywwkr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tyohianb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3liqdkdig.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dsdusvjj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynfgghjv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kxztppxw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cxfvocvd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3aemnzbev.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3llvwovtm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gthnqgoc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pcbmotje.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjacyvbc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mhclisbi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mzhjiaag.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whbbbdic.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xnpoiuli.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pwunerca.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pzqrhten.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lzfvxfoc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fwizsjnw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pzudprdi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iuydyvzf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hivnebaz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yijntnxk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3muznttql.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tmrqqhhc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hsyjmxkm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xuvvruzl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvdmcrw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rvpcgxba.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3idxphlix.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ctqgilxo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fwjapylo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcseffau.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3csbfbaze.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yakinssu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hayluiww.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hxrzcgpe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mqgvlkgo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fmsumdjr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vhnobjsm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zcuctqcw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efhkahsj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sfsnxrsv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qahqtnki.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gacfujlg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qkqzcnpg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zinkjnbh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gcctmgzg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bqmcpsnw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3wqpirqxg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rbgzlmkg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rcmozpig.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbtyotwh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufdmdbgr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hdswipmr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nrsuqein.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gybnctda.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zatiuawr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xyanhbrm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oamolrqc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aqdcdvmn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vurzcwap.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fsyfnhdm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hiuckekd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tasapgkn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tbelpjfc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ntocvnfr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vtcjktif.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3taootgek.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3khlsjmzm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3goiygaut.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fpnodhez.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qjvcepkj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fiknovkh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ruzlucra.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qkozxlaz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrwrdaf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hmuvegnw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tqadhgmn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeovdwpg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gsgnfqcj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iasrbarf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gcxwopxv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mosfthkt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fdaygzya.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jzarpqjb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3thlgmtsq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tedtendm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vljsuxgg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yagilusr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3voynpocb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwowunbg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3prjyrhjj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqgostf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtraqupr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irshdfmu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wpykhmmc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3assgpenx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fkhszpgt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qejjakkx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bxpautio.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tuvdptfb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nhyxygrl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hixsveir.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lswkkowt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nkddfytx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhojoxp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jtthwlvl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rznlwvmi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3npclfwyb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3andiqpjf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3skhgjjzx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uynyumvh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mplmzfxm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3awbcfblg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vjxmnpof.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgmwpbvh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zbtisneu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3agfzpbyb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nwfmhbfl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ryztadqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rnzcayex.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3crteepeh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wwxowafq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rxzebejn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lulstxbl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqocosrq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pqlxuvvc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wvvtmzgk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qpsftlhc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kynsfdtt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqcknbl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jsefmahk.html


<!-- 参考信息 -->