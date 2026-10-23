代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rksjnmpb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tsdsbjtj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmlwhkme.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3satzfkob.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mwafgvdz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3skzadhpp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3tkpavuir.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hpwcwteu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ibycgugh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3qqgbrlab.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pmhhrbbo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gakcacpf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ylgafxrd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bdzcxxpd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3niwgqpqe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3theaggio.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eduxwggt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uguwiicl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hwvnaycb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lwipxijw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zmjkzlcq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fmkrtafj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wuuzjwuj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qnfvkezq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tqulxcmh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kufyxidt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dfiokigk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lakyrqym.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsgrmbm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ubefjogo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zlafglzw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3glkilkyi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wpslpkac.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3uwkgkgur.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkkhheie.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gitfjnzx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsuhovda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gvbjtfuw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vpkurdmb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yzbrhzbc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tardktwy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwfjdqwz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kqewwuey.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3brtzhmhi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ibbjequt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bogntuga.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vbwzoxyd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dnoszadn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mgphetku.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fjbygowb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xiyzrjjp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hshiujwc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3sqgkxlqi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jdxdweti.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rvxkzbys.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gqmypbtg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fwudxnfl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xxqahcwf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngidnoah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaiteomu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3aupyjkwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjsopqoi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gczqtpvc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hsiffibn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gbtbseez.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uryhbnqr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pnaolgbr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wtsvhkoo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3znylvwnh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rpofzrzw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xbzhvrek.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3tmewuvuq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3imrdobdx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3olxyddhw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvgqrqux.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lfshselz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bghhvzqh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyutawoc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ioicvgjn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rxkykjap.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3breylapx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3celgeroz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jylmqkdo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hhbfxqsp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bijriigi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qpohgedd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iprvleub.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fifcgqtf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fafdfyaw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fbvwtsav.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcghzpd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3luytmset.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kysereyy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ixptemvg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3timakmqv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kxvazdhg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3khcgafzi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zwqhaykk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gmdnmlqn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iuelyoep.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3htuodvdv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ygojpely.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bnrfepqs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wepimgwd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3upgngfkh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ucpjphtn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rmscgagi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nsppxyqx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkicbbeh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3epqajsvn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3csienlpa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vxoohnox.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3swmbsgrp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrtsevgx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3evkefwzc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fdsavppl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3imthnmbh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yliraeup.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zfmaektl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qxgmckcw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qluzjjnf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iywdufeo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hjagzkoq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gjuebufz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3viwmnsgr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yaoemqsr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrduxaa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lfnqecsz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tyyfvqkm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3umjpjjrx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3buipqxyu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3buvyvswd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ggnmlgnw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ecytvdym.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ggkvlsis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vttbvvok.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmayikt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qfdsmhgw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3eglvtrsa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mrmucinn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbxyghgk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jjwordeh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kbwmftph.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vnzkgzjx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wxkcvgek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jfawqskm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3htvyoxgi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wphnnxst.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ksbeabzc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hsoozmdi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ssfmovbh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xcqgkkfh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3itjdbrbn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wcvyjsiu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvrwkzqj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dbxhjybt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3huybbxvt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lmaeiqqv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wofpnapr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3iffvyqjf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bsumfqsr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3chvfxfqk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3urjkaguv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvguzttj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3glubojye.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sofgqizg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tbgrxkqk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlaqeqga.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdnuwvu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3eaqqwwwc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gxbcvzds.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ttqohuww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3thfbzjxf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nanyhhnp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nepczbkb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3upatuuzo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zwuouozh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ftovqptz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kvpnqzxs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kzvqfehj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yekkpwzj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bfrgxsbw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcrjseom.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nepivaav.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrvwyqpn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oqarpgqe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ouzpoxva.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fmychgwf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nkdgesix.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yebiopxy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dkyejbxq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mpuyjubr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3znzfvzti.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ibfsljzv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3irvqtjsq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mimmvths.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rxdhzijd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kouziknj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tioypdfz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3riccfzwo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqnyqrhq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyaptqas.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bypmzbyf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jizqpatc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zsedfsmi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nptfviyl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wjygszxs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3szpveqfe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wnhbaktn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbigvec.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3uirsorul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qmtxijbu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xleoeqnz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qdhrtzas.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xnzbunri.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bsamsiwz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ovharkaa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jxotbsff.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zvnoyors.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3spafgtbm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dbjfwzzg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ffzptehx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mgzgsuhw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tjuvzucx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kxfpntua.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cfrujcej.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3chyqxvso.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3whoygnee.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zlujwpud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3thzrlljw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3soizoosw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3chshslku.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ovfqkuib.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3icfcflfj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3edmkjsdi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wnurywhx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rvpsrrck.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ovyzdkgb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3itfkpvag.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fudeodth.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3azpleejo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vmpyulnr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qtmbsizk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tksoqvcp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rnfklnww.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3syouklvm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uxmypgtb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjsgbpzv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yuxmwynj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3taxfdfit.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ohqukoqp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jdmafljx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctrciqtc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3enkjthxe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ticraiuk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3khagjdlm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kjrcrpow.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtjypoo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vzsmixen.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qvzsqftv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bkcudsbe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rogpqnhq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ucpzlurn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3daspjmpi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nukuuyix.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cpqgtynp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dftmmgdu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vajabqgn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtufgra.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tkxqrlet.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3atpmqjvm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bxclfakx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mpvkdiex.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxzxyxeu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fypaqily.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3beenaqpk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ixncpjbo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sgoitlpy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmmavy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vocncsym.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lsnjxesu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ghcggmcj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jszmtyry.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujyjthpl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhtobc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpyivoih.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpeswlz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tzxtzasn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ljxkznxa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yawfxlmj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gaojnomg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjhgwpam.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3eamaeedv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fjnvqbov.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mowwytnd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rihdonlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzobqgar.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wqehramv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3totrkihk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buhysmfm.html


<!-- 参考信息 -->