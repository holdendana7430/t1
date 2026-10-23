代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjcbmb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3iydcjabn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dqvloxup.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bttuzoin.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3flllrkrv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ejnusrjz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3otksfttq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qlzzzzsy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3roqlypre.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uoabjcup.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eangjzfd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zvdkppki.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ktxwoxtr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bhhoghjh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ypecdjpd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3aitlrppj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dnuifmxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jjheratl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vulfzpsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mdjgvque.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3psizlgye.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3plequcyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gbossyrx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mlirbqeo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3eqhuejbj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xnzlapoo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pvngeuwk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dgbacrfe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zzozynoo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3olfigcky.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kutuatgo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dgxbddas.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ayqxzyry.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnbdotct.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3acyqtlhr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qajkqqqv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywphtson.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3crliyqba.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ktgcxdbv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3arzckmvi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rnpvsfwd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dlkwhkbf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wxodfyjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xvicnbfp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lthaacft.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mhiwfcbu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3iarcvozc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3aenirfyw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3snsfmfbe.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3adpvlkge.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kwcinzzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjbbjmts.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gitkoahb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbawpvyf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ixhkuhlo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jjkrqwkb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yknfybea.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zblwdhge.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mbyeqbgh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3luyrtnfn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oxcilzdp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vjqvlyks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3baexsjou.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fcpqbwxl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kjwlkzdn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qumbbepy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3chfsdyec.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3takleuqn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pzsaebyc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3whmtcpbj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ltokddwa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ijiqrjsr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3emzzdtdy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fyihvlub.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kkwidtef.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wtktnhyt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cppiprlv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mqvfjuks.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gjitljig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fjclznge.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fqmpawgl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jejrfzmr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzkmyns.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3boewflbu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jmnklkgk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wosjaoea.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yrumqnyj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fckukvzc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xytoucvs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3macajenh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rukjxoib.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wzjobtzr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fdmnohss.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bbkbtgod.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uukrcafm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ndgofnmo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cfnpfpzs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zfcesqyo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3unrwlbsj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pzbwrfnz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifapxqsq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lhzzyjst.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uhejjxcc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ovqhymgg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vcqddnkc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vtfuahyx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mzquzhnh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3phejdvfr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3glslksli.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3cicyyvrx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3taymuzka.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mdcmtdtg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbcszev.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sosmpeag.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gfetxmfv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3moxgodrq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hllcvfnf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wpprcozj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xihilhjz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnwisk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dsgluuom.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wvdvozwp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3woxvsuzl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mgafldbk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwvpbxdq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewmulmdb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fqtiipyj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pmoznapp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lpguuurv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ezelcqit.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xgembiqd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cparmacq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmawgtx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bezlgjno.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tyjahupm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3aygfalrr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjvfvpw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yuzkypvh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cybeiddq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nglwznqp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3thhxtnvf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xwgxrzsk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxreros.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3aubomooj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fcrmxhea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ttygrxzs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqadfif.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pjdjuwao.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ahhpkyuq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kgmivqpt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxvagmv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uajzjveb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wgjmaowt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tmqqbixj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3feybqvnp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3erwyuawa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mmwxvecv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrstdtoy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3odzbzkmq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlgacvf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnbxjpqp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fyartaaq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gomkfezq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vntinofb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ocvwwnee.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dikmhyao.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjhhdyi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uvacyhdv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yxeoadxr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gltckmav.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ifftgjdo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bzftkvho.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3miskaqfv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mbxztwhg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mntasazw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mivlcmrj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zukdfqai.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iuxepypc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wfazroqq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hfnxrive.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3scdfuilz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yaljymem.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydqzplgy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ynbyefzx.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3voubucof.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nihqglug.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nevoroid.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gibdmdmk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3legqhooo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uhbxffpt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yddgiklp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eaobwzre.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmpfomu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3iozalrws.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3quduvwxy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gqkkpynz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jpeutwow.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bnuentgs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pdgbcaus.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3djvyrdto.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxlzkmbj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kowrgppy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bentbrfp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nbwrxorr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cisazwvf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3foidnyog.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iqiszrlz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3obnnagai.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wbifipns.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pgisdbyn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3prwolaqt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3uamgsatf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gohgqffe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eagvnnaa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dngdizli.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rljpcmzo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3csagvdld.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfolsimd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gitsawsb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cbjipizp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mbuujogi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jkuxlifn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3umcjygyu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hpqogrrx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xgwbtjoo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fihftqxr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tydijvch.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ohycbsyw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sceicrkl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fmoegwew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3awmosnov.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fmvocytc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ppdaqdbw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vbedmcfg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dxlsxlmd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zoyvcwdu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3emjcqjtd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsahpbii.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hnlksuqk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lpfbwfkg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uylwtrjo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svfxpems.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3knsljfrd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3orjqsrke.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3livbykyn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ofzypwff.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ncyyjsfe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zzvmwgip.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mmciaezq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3nmqnrzxy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dlmvoyyg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mswnaqav.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jbtwahun.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uohsvhat.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ytvaujdh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yjggrrjg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3liqovdre.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ubhhqqnb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3baieokpz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bxdmhnqf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zeaqsqlb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ewamfckl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nviqwhbl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ojcsnebk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3itpzpjfw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xlcjphnu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dvvjjnzw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3iltquuvj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mpjjmdzy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ulfjumet.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ndpohiur.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lulkpwhv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iiarrtso.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hqrerqvh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3duvwwcez.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqiniczf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ksibzwqo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhkplsux.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbrjqxm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lqpsettw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wvvjdtwo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjuadmpp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bzygnpbo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cxryclth.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zyrpnfds.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3urxdkmor.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sfrbwzbs.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fhtbhwpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqbjnhap.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eqrlgyxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kylswurr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yabfphwq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dnfthcqb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jeenbifu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dgszwnqj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aoiiudjm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zjccrtgv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mocduqib.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pwundfan.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nshwsulo.html


<!-- 参考信息 -->