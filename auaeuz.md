代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kuarfcnc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ogvfyjgp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rsfxnvwe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kfhpscps.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sfawrsfn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hqgnfuje.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sttinawy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ijatphja.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jfzjurqp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dqubshgk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wjgfictr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mjlmiaav.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zmhywecz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nvtpiudx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qenogwny.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qlqoqkug.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bwbqprtt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgqfwfl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lgmsnnqr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ktwkapau.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mdkjfwnp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ttxscfhe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mhwtujhn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ucjkxwhb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2prdympxf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yngzcoos.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yqiendta.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qqszribh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xyndkqir.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gtrvugcm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dfbzjpoz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2svoqwtsk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ecesyxdw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2uahfifhf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cnltvghy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lltncnkz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ycafutlx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awlqgcgh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2guiqzpip.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wknkdknt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mbbouaxq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qeyzmbka.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mxjnuwpz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bybfiunf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pjuunrhz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wytipzkb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jmorsbtu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tyyyqowv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2sfbcvnsw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzsqqpnu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cphqduwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpgetdod.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ksfdnkug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddruqueq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2habplsoq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yujioaew.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zdrqazuc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ljegvhtb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ioxidghc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ntzyuorv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gvdkrrfp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qusgvfze.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lqdpyeui.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vqhlpjpx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dobwvirj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2baqzajmc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vubtmmdy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anxhotwm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zmtcdhix.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2euwmledn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dqvmxkyu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2heqfsbyk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2caityjzg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhdgdhi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2myxvsmgx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mkucmmde.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iugpsvbc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2loolexll.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jznthizd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kggzkfub.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lecwriyw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzsymolm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jezroskd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrpshlyn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2eryhkwfp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kjyqtdfp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ntswyngh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rctygoxs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rftieoei.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cdneqsiz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qfajrlry.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qsgklydu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nkugfhrd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lqznxfmt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zuveepso.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lxjkniii.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ccwldadl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mrvwgxll.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zzlkoyhl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2imsdwjdj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tqamgkdr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nebzxgbu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ppcurwwp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wjxnazjw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xszxgyjm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2byxngbxn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hqyxaynk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bsjftexk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nurcnbez.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jqahzmom.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpgrflgm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2stvshqew.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2erybjjpr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fhjudgvy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jsjsuyzr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vomumyxs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zggrenxo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zkkwxkcn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jggpdqfj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2volskrsk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gnrzmcod.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2wjzxhnfi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ovtyljrc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hmgxawsb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nfmfwujd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hqbswkxb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uepvroya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ykfowdam.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mtnniigb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2uhabugcb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uilggkay.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2blbnzdln.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2teqeonjc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rguoridm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qrkypcvc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2eoofhgvi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pcecfjse.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oolzjbou.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdrpumj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ahabqzvl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2grcphycd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xcnjatvy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdslcqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2btgrmvot.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tvhvbsac.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kdnkxmei.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2erfbcbbm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xpvtovzs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2eftsimgx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gywkupka.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbsdwfif.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gmjoynsv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2drkzekuo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vfspzfgo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oekhmzvf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2flmotvhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hneourpe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pecvvjla.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fscvcgmy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmokivsx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2opdyqyoo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xmbfpyop.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gvvzypfh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lfehwzaj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gmqgxpuc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qcbevssi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfuvfbo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrrtmnne.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2unbisshp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkebzid.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ymlvznwf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2unwjnhwq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wmfnyemc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juswndml.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kipjxhtg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtdyuitt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hfcijitr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mwsrtjng.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iwyqcasc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdhvvpmb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2irjorjpb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mowclksn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2okhqzccr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2evzaefbp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2royijlrx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fxzrvuxu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qqwofnty.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pwujkllm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2drkzwaao.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rznnextn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtdxfadk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hiejarwm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2phagprft.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zazkmfyg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqmydjt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2rokkcnuo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zmotsaff.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2jqwbwlnb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2syvqxazy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wrxexfme.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnzafcyg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2szkupgjh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcvgjtds.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ylprxcpx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpetaysy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kejjkuim.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vtlqgjdr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xpqppjov.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2evansowm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ldrrfqud.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cgowuzad.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2phchcblr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jxsjaume.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vzfotkbk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2feukdidz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwkokiab.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vcrgasut.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cubsapif.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xaegpqay.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2oqurymfh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fgakhzhh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ikwsudpe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zokusopc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2uzzdxzup.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fftujrti.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yhjjabsk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2numhzyzd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbeenif.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fysunsvn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rspzpqai.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dupzrbaz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nikgbneo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fzgcuess.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2syaiaigk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nfodximl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bxwowavx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gzhkxevc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgwsktpw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tjqwlmfe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfvjrxa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gtihppbx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mllpuwnt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hschugrx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2exhjsftn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqxsmbzv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qhuyveaz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynizpsxi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hzlnoeqh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2faacqcbu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qhescilw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2osrfjnll.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nfmeqyjq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2avsbpsql.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aycbjlvt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dqcvvumj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hauechkh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wplixfns.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hkpqgmfn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdsvgdjz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2laxdyyzj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdgunoxd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vawipreb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qemydwuv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hpadfuci.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2izpmktoa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pueevbfx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sadlijke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2paogtsys.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ygkgesrc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bohkxrqc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2znleqwhn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xhiknrsk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2crqfujfz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dopemcpr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rqajyuuc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lxgnvjzu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2oexlecpj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2smoakcqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zkwsvalr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xiodvmne.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2itwhuawn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rgexdqov.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uanerckj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xyxtgwcb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yyqujaho.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dtcwnmzf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xnqsrpcy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2olwnjlnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tybwbyvn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2lmfzkjuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouhmhcme.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjthftwo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2prkjhkbf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fpvvbbsk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wpsmwncq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vzuhmrtj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikyklohq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2annfevcr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xbsorfrh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mgdivpgj.html


<!-- 参考信息 -->