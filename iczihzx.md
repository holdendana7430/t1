代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gyqvuuiwi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/glanfqcia.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gawwamhut.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gtuzswaku.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gxeemrtpr.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gcfftazmf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/ghpqjbplv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gywndrlyf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gbnxkscwy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gutcxgpyg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gkexmphnh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/glzxckoaf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gyaxrteoj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gllktgdum.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gfftkdrzm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gwrkyojkh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gjpfgwwgo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gthsnteqw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gprlfpjnu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gltjanshe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gwrwdunee.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gmpcpltvg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gjgaulukx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gfuktpyyb.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/ghjfnibub.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/grcqxysba.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gynubdbmv.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/guhupyfhm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/ghblliexa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gvudyhyxp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gweuwthec.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gzilecyph.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gxirmnlak.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gqgwxxghf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/guorqogiv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gstnkfwep.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gvefzbpcn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ggatjiezd.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gzqeydvbs.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gsxhjqahb.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gdqvvbmmi.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gwijnlszj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gboyrrqbv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/glkradyir.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gxjtjjliq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/glnyjfwuj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gzadihrnp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gifqmwrkx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gjxunwpcu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gdgzxbvsz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gswotwgkr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjzeprcgh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gflanznda.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaewowuhq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gwiznceng.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/ggfughncp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gnliakzwz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gxermilqj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gmgvpvvey.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gvydeugbr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/ghdqmjwlt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gqnygveij.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/ggtpvgpom.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gfabjsmkg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gumurwkzl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gvevumqxq.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwfcqqodj.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gxjhpgdun.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gxsjqcixn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gpecdygvk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gmfletpjg.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggemypncb.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/grqmuesgv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/girqfddhp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gjspieaeh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gwvyfezdo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxvxbptcx.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvlbznuyu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gfdeyqoql.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gkdnqgogr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/grpdcgowz.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gzmxvrybw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/goyqqygxq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/giogxzgbl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gswuocjfk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ginpdargd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gayhdtwni.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/ggghpfvwl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gzkulrgns.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gvucbgrso.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gimmojyoo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gooalbrwm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ggbcjeehi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gzxsowcpo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkppmwpn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gphajrenr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/glsswgipn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/guetfwtrf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grbcfjhiq.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtbvmamrp.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gikaxnvfo.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gxkvmgdzm.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/glvizrcdf.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gaqqnspzm.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gfevffgtj.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmrtdixqv.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/goqghgbbj.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gjjkcbkon.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gsuyqlomh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gjwhueqma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gkhtmxehu.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gybvwflmd.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/garbpplzi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gzxhzgfad.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/givsfpvvf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkmhmejff.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjlbvzgga.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/griwddlzq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gwmljcvgt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gkpwcsvxh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/ggrtizlhn.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gexrdhqoq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gskrdvsvw.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gkwkpgkhp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gqqjtxwvu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gihzspdna.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gplxdxwlh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gsyzjqudv.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/geawrhqok.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gylyusvrf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gmrowmtwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gjikxprhp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gixooxdbe.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gdxwabnvs.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gwjlxuvnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gmfwhugww.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gauvxisgq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gxrzfwrhq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gbrzcxndu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gmtizgfex.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gypyyvbwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gdxedlbyn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gowdcybty.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbncuxq.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gtlucbgkj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gpehzfnwb.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gumhjrwev.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gpxwdwrcb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gbzljxpvq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gzlygfchq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdpbbgcon.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/goprzwcrr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gmnkespca.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/grbfprtpw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gcchoxxin.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gbrdbnkfd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/grbxzjkfa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gtydiluvr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gmuvmrbqe.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbvtuzxbm.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gdavfsicp.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gtfjiylfr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gynkhahdo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gjollilsu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gbepqzvoh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gjyogaooz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghxowigei.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gzshsrdfn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gcumjfqci.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gzozmzitn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtqebmppn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gdoxeumoa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gemhgizdx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gugdclhgw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ginvhgcsv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gysmrfwkg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsveoeoou.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gauyftupk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqttahuay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gdkqscusl.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gzqkffuvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/glpauvqvo.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/garrkslyv.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gtrtjjati.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gehsjsrmn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gwteptcku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/ghudlzmch.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/guawjwlyd.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbhvwsmtw.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gsmoyimcs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzbvcbjwz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcuhkheda.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gooifpvhi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyhoxioxq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gidbcxfpd.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gldoqbbzw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/ghspspfrb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gtngubjee.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gyisgcclm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gxyaptibd.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gulbunqgx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/guapdetyg.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/guihcvofu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gjadklsxg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gahqwbjlv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gtybqdnbh.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gioukldxh.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gxicpfcwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gtmkxalnu.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/geddjgbrh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gsztpxccv.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gcgarvjqx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gamfaacuv.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/glhkqtavq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gwsrwafrm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gasltgqgs.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gfdubhwhm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gzoytwjnj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gwwpikhfs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gehuuafuv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gkxnulpnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/ghesefrkq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/guftuwvlp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/giucvcryx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/giinzjekz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gwgxfjpop.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gdouqivjz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gtuckrxic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gnvmgqazt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gaabyjtlr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gpdrbvwhs.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gmtmkdepy.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gphykruzi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/glxshmbbd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gwicpwasb.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gdefrgtdx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/ghlzbbeab.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gcnvbzuns.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gqbsgaxrk.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gcamzyplj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glbstqint.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gsdcdxnhf.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gddnsztmg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gweqmkhwx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gqznvlmdw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gejgibckq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmqltyvzs.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gwhhrafla.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gxrqvqiir.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gwtpyzdvn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gfkeesziu.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/giojhyizk.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/guivnpcih.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gyhbawmwz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/glijsyool.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gykmoqtjv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gcfhhegih.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/glxqrejch.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdaapyszr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gcwuzzreo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gxaaoupji.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gecbtrolw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gsvfeksek.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/giqycxtjn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gleugeyyq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gahygteqf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gqwqircca.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/ginadzfer.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gfkohokaz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gjlmyhpwt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gswdjwdss.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/goqcwwnjm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gdjmfflpl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gvshieenu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gttiojyjj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsiizzozp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gzluocbtf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gtmwhisct.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsdvflldq.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/grsfllhjk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gmfaoxqch.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gvhzkqefv.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/grbhvjznp.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gpmffxugh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gbekxnatv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gvnaxsltd.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/glptfgnnm.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gmsuozanx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibebyzbu.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gkjbdjrsn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goweioxhg.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghifroljs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gqclsfdsi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gsxwqyxbe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqptwlnry.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gqgyuckxi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gztdfpnwo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gnjrwrpeu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gdaeldxmy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/grpnfmhny.sHtML


<!-- 参考信息 -->