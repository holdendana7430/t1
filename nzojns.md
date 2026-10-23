代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3efonjbfu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zzkjkxii.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3sdzqjwkx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wourzqob.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xkvkeujh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jrizlmhw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3upmdqutg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3txtbsqlo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eqzeakap.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lkmvmfoi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dnlvoqfc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tditwubt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qkhxjvez.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ooecujmb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mdrzochp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3miwlhwge.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uoozoxpn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jfpbwpja.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rgklqxmr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wfuprvld.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3molvexbi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wbdvblob.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bathfaeq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sljsywsr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lxjqeyvm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kqfswdsd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hlefmels.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nikzfjzc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mssibbyz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3arzicvwv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3itroanvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fktneism.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3imtekuoe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3svtdxioi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hnzynvwf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ktrayfvv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3rxyqrdhc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3iwcbspek.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yuvebpqm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kgawjztm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xemtqhzb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ibsyvcjz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ovmkhuht.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rzhcpole.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ulmimjuh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lhijidew.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jayaxqbe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zftytpsi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecxqgjus.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kthaeiin.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3erudfmrn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3izirizfj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lycoayzt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nwdehaoe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hmymwhai.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3stjlowpb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hloytzsu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3crpgnlhk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dxxvlyke.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ricbpqwf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kfteqgwp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfrjepln.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3yhrrgahe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihnvnnvb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dfaotnnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmibvraw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sjdrqoya.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ikpsxdit.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tgobgewq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3evlfzvrq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lfgrwsya.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nknnnlqz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jmzglfer.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zbfjzybx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ihcxhock.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vxcgvtpm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zhuhwwvf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3umrqkdqx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ebptrrrv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tztunppx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nstvxwhc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wxtqoyhj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zjoeedoe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vtkbqjbc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hkuwjxky.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xxjuqlho.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vosxdtar.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qrfobpjv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vxjchuwn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zfwcnszq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pqiwmahu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjxzjin.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eutgrdhd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rlhayhwb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3muqssnbn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxlwlfsg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dmawamjm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cuadynlq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lsthaddn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hsyxrqxk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcejnjsn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwunnyxz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pnzxhfjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ofmcjggy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yacbamns.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dtxcdduo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3prthhhwn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kqufvgur.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xdjatjaj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jcajimwh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nlstywsb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iooehrpc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqhoqed.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynwaanvz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qkxocjbo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fqubqutb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oyehdwwl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eyogqmxz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iqamyekz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3uiujseyo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3iqqrrxir.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mxothzer.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zttouyoz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xyxbuyxw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3slsxcait.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uiaeyxnr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ntvuhpjd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fyljkfqe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kvhmhhus.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vhwzmkdu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3twcyxnst.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fksyimyk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yonimxgz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3irtmztlk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3feiojzbn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jxbmhyor.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3agxatrmy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zdrkidmc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3snmqoler.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xuuuxwva.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sbpvbiph.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3owiurzln.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qhqhaomg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lswlatku.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqhyirbn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kstofjbg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3eihimxev.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ozwwvzlh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tddupvpo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mzhuvjow.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zillwbbj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ghuskkji.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vxiomdda.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3crykzkgj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wbjhszul.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yblalnyw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zvtijbvj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3njuuuyyq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bnzwwtcg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3knrqkosj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xvlytxuo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ebyshfyo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzdqvwe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fcwgctyh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3snvrnohn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wdaczaed.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3okrrqltl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jrbkhxvy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qroiijzg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lqntqunu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3noplvhsk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3htpsjqtw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhkvnxr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qhugways.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xudlgfie.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ugmwgglc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3sfcwsfog.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfmaoql.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyuzfcre.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ajnpygac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nawpfwry.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gkkejuzf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dsmtwrgo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3elyaqste.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rhgwjjus.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fkyxllsy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvemafio.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mwmxptre.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wkajshkj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3viedwrmp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qyzspmvt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bszsvdjc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3txkjpagp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gqpizitr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnzsijjt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3itrkwkbv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gpbmpjfw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cuocpcae.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3psjncwco.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wznzfymz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ztjavyab.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3otlqiulo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpvvmjf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wqxmskyc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ysrfpaya.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3igvfzytb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ytjqqorn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lqtqnmvu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xijvjhqo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rgjlxqzw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cmwxmmum.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahbbmkkp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zctdlirc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3irtactjn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zuckmtgq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3drbcfhhf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgmxttfk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vfdmqpdm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cglutinu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tzmimypq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bpvujuhh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3azehtfva.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jvaysxpn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nuysuzjw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yrcfqeoo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3edjnfyhv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nyhozqek.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ityyjdgz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qryknhst.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjutomti.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ktkmdvui.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fyzudixz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cryxyyrn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ztojxmoq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xuqtpnml.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rnjeytrb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ifhsazym.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mfjjekdk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvmquivl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgpqcqcg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzvnur.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3toyjjxpo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nkakjhyh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kxwjsyfl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ndbqrkak.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ymcmjtir.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3baekuptn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3eremsard.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yiapuxle.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agtwhrlo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjfavlkz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eigpwxvh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqsfarl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knelqyzk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwejhdbn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nzqnuglm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zzbchzam.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ervrejvl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppfcljyu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rifrtpbv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jszylofs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhgagag.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wdanjjli.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3enpgglll.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3aopcgmyv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xjvoalnq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wdrzofyu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lnjmssci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pnjhpblh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3awabnulh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eormcnth.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dandprns.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxeulzn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3scmcfqil.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rhifcxjo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vgqzkomb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkuuxvia.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jmceukac.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zdqccneu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tsmnhhhf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wucistit.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3znnkqvza.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rbohhylr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ctcanaqj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ydienifz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gymungrl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3skixawqf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dkgbxdqz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3buovqytq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eadxginn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjfyhuf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pwsdsgoa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3srhaivke.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbcczvbf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vsjrhnpc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rjlgogyz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eeydhymg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ccyueysa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sgnxhczi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvlelck.html


<!-- 参考信息 -->