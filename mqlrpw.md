代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eyngllzw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xjorirzf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wosfwoin.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jphgtfjv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iyimqmgg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xempspao.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ttfsbmvo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvmsgc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pxpzbqyd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3feqbhcge.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vfmlsjqp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lijpcmpq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xqwudauv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jgjoizrr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ebpvoyjy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oazlzyyh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rwxjozwr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3czkobbcb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3borrqiuz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3okvkcdhs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fvzqivty.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eyozuhkf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fqqlxhvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3izdpygdz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zjuqhmuh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3yalonnck.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3akgiindv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rzlyjygc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iqjtfbwe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wpddwulb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pdnohlfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nfsdwleq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3brunnsom.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ywuyedgv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3arzcuwnc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gnyecrck.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pekzmhuw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fclgkgjd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mlsieiqz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hhyvrsqs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vilbhtrc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zymsiuyi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3orspeauh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ndpdyglr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fvxicpez.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sjrpolnk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rszcxwvn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sgxobysh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnmlvxcb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rehjqlhz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3loceiiho.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pwqbjkmo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vrbhvolo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sxtolcdv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ysoxchdx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fdqhmwnw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3luyimpdu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3likonmde.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iqybyhcb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tfptkydx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cqiabodv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbdkmtlk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3igmyzclt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mthvsaue.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3scpeeceo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhnpqtvh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bmtzgitd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ejgwcxmm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tjkbuzgk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aqbukrql.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ehnlgmyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vbtngdqb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pgscsjbk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uffzfdql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rwjzppcd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kbwcnvxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tqknpvim.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3powheskp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3opperwka.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cstemasq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rzfshcir.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dxpbrzzg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gizixqtg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zwmnjnyn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3clsvzxrd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3owkkqolc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkcwszsa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3yqewelkf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dlnqomqp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eqmxdcwc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3axutctel.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uowawivj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jnugihcw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cuidorum.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnxfclx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvnhhp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yervzsdj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ecpdrpew.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3njrhicsi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3krdybdbi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gidygjez.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcgkrpsu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mjklmmda.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cxzuiqeq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sgtchpdx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pqkfwezx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xsrtiwta.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wbwpbmqq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3loucstvv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vlfmmyla.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3crotlmhd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aiyfehyx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbsgwlst.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqsjazmm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3chynpudi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rsmhsbmp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vnmldnmp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hgkkzgkj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ndxidllx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jwmscvti.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3amgcijfe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3okzjlmea.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lottbwex.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dplavree.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tlnhxixk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ezmdsofi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3eqkaniox.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wmnaimpw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ivwnxczo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3lohgywlu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxoxikjy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bfzufuhv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gwgnlyay.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jjwryyyn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqtaftqa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3occlvsam.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3snukmpox.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgdnkdge.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cfdfndmx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3clgclcta.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jfchaigx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ccjzlcpm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iygqhdpq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ugggzgrp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gveidipi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uiwzwvjg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tlwpfunb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ayfldnzn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nbzybaoh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjjsccwd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eypogpan.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jsgtabjy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3odsbccdo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rmhknddc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lzruztll.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lpbwjwbr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hfbpuaxo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mifctqot.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yazgkhyu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bgapqpum.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ueoasddf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3npuvoeno.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3icpilgiu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jywvgevw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wjjcxzmj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ffxuvtad.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vaxbszed.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kskqlypw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fbtdswxp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xpkxsrkc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xdimewzp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3teyytuqm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgkbnly.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wvbvrpry.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3flakslqt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mcvlqynl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wzywxscn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmymeqxk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqckxxzj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpsjsown.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3viodmobb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pxbvcqsb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dakrydyc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rwqlxtrz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3prdhcwxx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvsqizfw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3itlqllhf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3awrkjaeh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opqaomiw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cugjqmyj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lupcihed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bvkzzdyb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3szgmrthg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fjgmlhet.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egcnodii.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3whuhtjdm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uppmbazi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uavhzwcl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rvxrkdzk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3djreobis.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nvtxdpdr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mdwxdvcv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3idylntxl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttbupmxs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mpvpyylq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yziqeamh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3axkbtcar.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lpoiwxzi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vmvbxcgu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3psowpetf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rwjgoggj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajgvoepm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dznyznsx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azuhgiux.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gielkpnt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qwrfxvrt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3inncdhwq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3oitjmgcf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uarywovj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vbqsjcmq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cxzkesvq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3aipxcmfi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3axcipauz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3akdurdjv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wixreztb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3enymbzfw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mrcgzamh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ydszmrct.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bmahegbg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwydjqrz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tzjssqjh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3elvblkcn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ihnmggii.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dxatgfrk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uprllvlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hnmpkwsf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tldmdlem.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3inogbebh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdsjkizu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3omiuohcb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3egidpmpj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xhatzsxg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eaqfteft.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lkgagods.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dwqxhkls.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nixlfwvw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zmhoathf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qhpwgdtp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tcnarwgv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pasidvfu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzhrqoub.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3piclvpre.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kghryhhu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ektjoywo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrhgonw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3aefuxzsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olcllwef.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tjijcpfq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkzybypp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3flxlcdvd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hhtbkszt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fetocazo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fqtfyhrj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fduodzbm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ftyytbvk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aepzenaf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qhpcfivj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wgrxdfon.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jckkxkjn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zxpjglzu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qcmaaldv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ukedmpsv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lxdzpicl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mxcoijpu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3nzmzvbsq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jqocyxuc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3amvulaxn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmazhnxi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lxsptino.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzzjvfy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3junqzlwu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sekfktao.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zejxqgsp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vhowzjqt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vtbtbahs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ccyrtuum.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xmzkajsc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3guvxshrh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rjcjvzru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3masfclyq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xqnhhmuf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rsvgpqug.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcrtpqfm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwygbmok.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cbjdaoki.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3onvzlcos.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yzeebwqv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rchywhgj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lkuquajo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3palrsmbz.html


<!-- 参考信息 -->