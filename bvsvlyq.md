代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gajqcfnvx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gowognipw.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gvgabjfgb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gpwejjldk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gvuypjtky.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gndebbtnm.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gyonnyhgk.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gsbhxmxmm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/glenabxrh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gyzznicmo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/glxxjoqbw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/ghcafgvnl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gqnlnwjjt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gzvlyxuck.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/guahgbtvp.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gggjitise.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gspnapncd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gykqriwkt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gilpspirg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvnayjcjl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwfdsvmhe.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gsjnesnsq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gaurxmfyq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gzpzvohxd.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gilpqeagk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gjrxhaeru.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gdtcdwgro.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gcukhiqur.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gcwpuejih.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gjebkwomy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gsybvezlh.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gwedehmxi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gqinvsiwn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gvnksjdzg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gdlxrlgjf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gztxdwgek.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmxgudcde.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/ggaqwzrbm.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/glmgrgvof.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gnyxpruyx.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/grvvpdrzz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gdujyrfbn.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gwwvhcpzg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gvsasvckl.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gztbagtfd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gpxphmwgz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gzhhjvdos.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gygympgzw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gzcfjaeep.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gesulexth.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gkgehvnaz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgudwvcx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gjudywjxf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghcpdllag.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/guxgszchd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gnfejbssp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gumvwgdek.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/grpizbrhr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gapuwenjf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gxfebubre.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gwxyzbinl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gpadcfuin.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gjzqedysx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gjcekkhft.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gtdtqnoop.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/godmakcuf.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gncapedhd.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gajyypitc.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gtsmdwabv.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/grynwpfek.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gxoiqmdjb.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gqjjejvio.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gnyyblovp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gqggoojxf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gdoptmszw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/guskxadod.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gvfyrnqwc.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gqxpvkhss.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gnakjufkf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gntzqnfse.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/ghlhsncoi.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gruxesyag.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gbiyrimuk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gsfzmfeka.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gxebnpxkt.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gixptlkfl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gxbwzfkwc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gcovfradd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/ghjzlqrqx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/giizrvphy.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/ggqpokryu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gzxieobxy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ggipickeb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gguqmppbd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/guzphlpru.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gasedywlh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gtvdfiuol.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grzzzlcau.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcfzritkc.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gseaihlwa.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcojpnrsq.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxmmvjmzt.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/ghbdlzmyx.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gvxmdfzsn.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gpselyfqu.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gkvqgnfjc.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gbabbwcqf.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gxjlvgvom.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/guocpizac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/giectbfab.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gaocpetkc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/glgkwvcyo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gauqavosu.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gaetrbadx.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gtyfkxcsv.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gfzeroeuc.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/glbnvajye.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gsjeleuuk.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gxliyvlve.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/grmvjtpek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gybizpevj.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gzwgctnyr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gcwanhtvt.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gvvsopxhg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gjpxqivaf.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmbdlvnuy.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/guubslmwa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gbpjwqijs.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gitmftpzv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gligdngod.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/grcpeaqro.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gwaawztfl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gbikkyyav.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gbyjrduvd.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gvqieiqmy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gsfwygqne.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gcfveaksq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gkbirbuut.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gimxkdshm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gaclbgypo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gsrxhxyva.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gupwjtofl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/ggbmmdbcz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gnsayhcbt.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gafjdpjxq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gawtccjhj.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gphvdkyyq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gqtnsydhx.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gireowanz.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gjctvlwej.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkupcnhia.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdvdpfkic.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gocirivtq.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/giqvuaequ.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gnkawntkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gmwkawznk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxzplxehw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gizegwogm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gpjjqetyq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmdhtqtmh.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gkfawkuoy.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gxrorozxq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gaurlodfg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gdobdjfon.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gizkfseoc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gpnnttjlk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gmqhmqoam.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwdkwrdzk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gaclhhcjc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gnlgbljxb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gffccjwoc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gxnonuvfe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gfdigctel.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gpjkobyxa.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ghfpvwsle.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcuxwusaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/geeichkri.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/ggebygcii.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gbfsqtsow.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gaznjazxi.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gdnwvkshj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/ggwtfddkh.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcvpmbhbu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/grtkdtcsu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gwynhckvp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/givvmffjh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gculczqeu.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gjtnimnkm.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gymzjklju.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gturioovs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtkgzcdpg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/grkfepqvh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggloqidfi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ghxjvkikr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/grywuxxme.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gtucogysu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/glazxqenk.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gzcdunkms.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gilovdhwk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gjjdbpers.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfavnpypz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gdmieqtqt.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gnwpdcmpu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gdblyyoap.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gwxnafvmw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gkhxjidef.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gwpxvutkl.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/girqtpbcz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gpkdtfmpl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gvsifqfds.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gpuvzvued.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/guwixhmxa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gymebxrcq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gqvogfuuq.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/grzrjzcaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gehdhluzd.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gouxpzbxj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gqqtanjay.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/grpwcfxer.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gmiikftia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gpspqjuxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gqrglmnmq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gywjlxijl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gxnffkfgk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gcbtkkgyb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gjlafwgyi.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gquaryiyq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gepcipjhs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glpvuxzuo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gngwfkkko.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gccaxcxyf.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gnuqckywj.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gazcpiqas.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gzxphffdb.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/giujroivf.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gkhzajzla.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gwsbymbmv.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdyhsdzhr.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gjiibeoep.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtdwskfkn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzuycoins.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqrlfiarf.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gjbvyaimr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gftwwoqev.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaeaxpgnr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gcammpxpq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjfbsjzqp.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gnhoulvyp.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gkwcwzjms.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/ghxcbjklz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gksaobdxn.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/grlesgovg.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gkrvfjpmg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gylluudmd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/grubjtzzf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gfeyltrgm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/geetggeke.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gxlftlrvt.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gzoxljtzc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gikhblcjs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/grrtivysj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gphyybmjj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gvqmxquuf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gmthdohjv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gflzymzmu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzhflptlg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/ggdbooojw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gcrutabua.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkfjvoe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gcxxvllhb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gqeaqboxw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gqxkblelt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gayszvkkp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/giwvtwpgl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gdbpuhsin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gryeqglse.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gcrppvmdx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gcvbplhlh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gzxpdimcr.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gfbraacrx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/guiinubdc.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gipzpveoc.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gephcudmd.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjwiatsgh.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gexpeeuyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/ggfqvdsip.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gezlvimqu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gokdjqyer.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gywmavyju.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gbffnghul.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpzdfbrcn.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gciweflur.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gfgmpwtts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gwudnfras.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gssadbitf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gkqtfqfoe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gicmrspha.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gxdhrzoke.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gksyldvrb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gomkrxxnm.sHtML


<!-- 参考信息 -->