代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zljcqzny.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tkvudkbc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qzahuazj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3svybkgqc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uobpoxhn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kurancny.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yrfcpwub.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3inzlvjgp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ivdowvgf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3sexxcqcs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ddswssyd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qyjhhdgr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cdtrnwjr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qwnnkyuf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3irtfjxzg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zlrrvbxg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3faofepwr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ofwrvdbs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sraoskwv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3klbtoldx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3oxwhtvot.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xjiikjdp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3prkgwazp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pssckevw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ubwocqcs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yurlvyae.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kindfomq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pfdbliis.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3szssvejn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cxcizixu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ulbvrtbm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zizgofyu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3whwuyujj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ugzdakpg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kiminmim.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pvjyrnxl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hqduqztm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3badhxegp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3krkclpsz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3frwbgfmd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qfzaapck.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3crcfmxjx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3smjkuccc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bzbvufdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3muxtygck.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrxjerrr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rbzoxqfe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lzkeuneh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pazrgmde.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xtefpwsa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qtpxttqn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hvfrvlmh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ddxfxnqd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3onnjpgtx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nqzoccqq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elduxlwm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tylkfwqe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mndmqchh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3baxltvhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjyzoloh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xquysexf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tenlexiw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pleqkliw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mplxqapk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3milnqivz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wygzqvyj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wwyrffxy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iztjmqpk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3poxvkslm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3olbjkrzi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3thsluhqj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vzdsrykz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wmwxweac.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pxmqnfij.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fxwanxho.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnyigjgn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xikwvdcj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3giyaresh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3txucmonk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ciztjsso.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pbhvbahk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kjypbdoq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfxlagun.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xjmdllgo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iscyhwrk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3thxuomqh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dnqvxucy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wttaarqm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dbbruxxb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fjgcgtvj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhzwdbd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjebyapz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zqzakuhl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sgpzluxa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vzprwlwy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rbemcgdw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3svrsbyly.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lwmmlhmz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ejymjrtk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ksbwbkcj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yrovddlo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rcbpvubj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pzzbihcf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hklffsjq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dxvnyvpx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qyttomkz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pwsyxwix.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lloztptv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zgaigvvb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3flgcudby.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qdcbysdk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tynsmhcj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mgrbrzcv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yalztqbx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rtvrsgyu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nnfswjpp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qszfezce.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wtmwcfke.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3balzzogv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tqzdrsne.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lqnnvuvd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3megbilbn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3aymdgibr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jughktwr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3whlzusau.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fcezvroa.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3afhnkkos.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3drxptukx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xalybgwu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kdtnhrds.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3adixyfar.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pljofids.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dzbzkghh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pgatnprc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dlvprddn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fvcwupyz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcstjdrb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mwvlxjhg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3quswdwax.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3lhombxpf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tnoeyuea.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kssstprs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pbuenezi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bovaortb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gjodgyiy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwijkyvj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ivfpedtp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xcilxfou.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hohzpept.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qecpvcfd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kgijzpgg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lvcqtsna.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3anudonkv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hrrqxbcq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slbrdtpg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ckwfwkcs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3phubsqlu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xrbevpdd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vbtwskzs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ibdwxecw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ihmbfxuy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3oikvudba.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3oetwndai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vubnyrlo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fhwxyvqj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3htbgdlms.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pptslaxm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zidudoeq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpqpylhz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zsnvqppv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wymxbtyu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3osxmlxwr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yzcmxzvx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwdpktt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxkebvo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lioztexe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ueqltcaf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3cqxvxkcd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmnjfhes.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ifbweuhg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hjiafuqu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfjskkpy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rjuupjpz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wlarqkmt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxgrwpkn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3comfzklc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3huznxgaa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pennlewc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cyfjuaef.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uqdjzqhl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hixhqujm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fwtmxkmk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xyxtzadv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3raduezep.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xclimtqj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xcflgdaf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3untlrqhu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dcamntoe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oppvwldz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edstgzyp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wyjgemji.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3udubfkex.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3boslplpw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wqdbcych.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3obennilh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3obzwafmg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3riaxjlqo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdowbwzo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkekgxcn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmkjgch.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsaftzmv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hhesbmgd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwmjfcwc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kzgbtpad.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oxgitvhd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lciwrxqb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3aivdjrnr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ttjwmson.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ggcksouh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qfqkkzyx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gifrzcnm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ugtbzfst.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bfnkeqdg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kpicrbwt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hudrbcyk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3oopojqso.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cpywhjpd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vfmcwzrl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fpuluugp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dtwiyrek.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hcitwjnb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jjainvdz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cspzbmlt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jgmsksbl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mchcwykx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gnkgimdt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qwpywlwk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rruyrakm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aqqrexvt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wlguwlpm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cbuzkwdk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pmpfximy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wpmdhygt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3chdfknim.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nsmvxaas.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylnmjlhc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3trhnwhxw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3stgzxinv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3licnxepg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxosvdh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gssmnzvi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dfgddrdc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvzezjkx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dhbhyzyn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ymjvqpfe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ezcsihgv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3mruwnybv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mttrvgow.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3toccqcxk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qdddkizt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hyhdmgcr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlkbycl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3urujvdci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hukepmza.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cpoamvkz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ckjotbru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lqmgoupc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dlmtzydl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jijstomd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3edlnuzsz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mlzvnyjm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nokguxtz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhjlduw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3egpuiawz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lqbgurug.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3esmivyzk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zscafxfj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kvingbqm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3chyididt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jtpfcgwv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tmtyezeh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgapits.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hmdckvmf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjtppnk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tmoylcpp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cxumhakf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnsqqds.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3drgkgvkv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qbmmsqcb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njbucxwv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mevypbqz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gmgytwce.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3whfqulgk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ywoxggtw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3obqcatym.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnqpveg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynjuvziv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bvxqrnmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwdymabi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upmpqsam.html


<!-- 参考信息 -->