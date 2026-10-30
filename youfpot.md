代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gkhmxvnvx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gyuzkaesl.sHtML

Java: import java.util.List;
来源：http://wap.fanxiaobao.xyz/Article/details/gpmpvvsvv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/gouwhgoqo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmztufvwe.sHtML

C#:   using System.Text;
来源：http://mobile.fanxiaobao.xyz/Article/details/grpniepah.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gdgvzhqle.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxqvvdzn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeilksed.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gybkdivsg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjmoiub.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvjxzcqh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gjkzovmwb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpftjxbq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gukzhwdwo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/grllvfmrr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gtbmfvqme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdnyohox.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/gckfovauy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgtnauw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/guonrpfvu.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/grczbvuwf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqiqskif.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrgxoohx.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjzhfipsi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gljxdyfle.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfysuifza.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gthcygzqv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwefaxfqb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldaqbelx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfgeadjh.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqhalkw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/glkbpdhvi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/gibwsrizu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gytpftqqj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gpiyrcqxn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzwgaqao.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gryajvwfh.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvszllsu.sHtML

Go:   // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/goqnplbyu.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gukgcvxrs.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuhnxftv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gbtajzjah.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/grqqqzeaq.sHtML

PHP:  // 无重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsxvjcnf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrnphsl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gferjdrpe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcywouams.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfvvrmlx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvitlibhw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsfclgdzq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwqacdtfm.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gcjckuuzu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggzyplqqq.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvtiltbf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrqcfoot.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gezgjvzfd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gsktsxlbn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdictblv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvvyqchi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofjdvozz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gksugjppp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/glrsqtaai.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gqsuymgss.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzinqdmec.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjqbjxxe.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhzvucne.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/geyfprtuw.sHtML

Java: list.add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnscecfhu.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkoowcpf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwwejciz.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyjyfdec.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gamtkqzdz.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqseqlmma.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjxcuurc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gotgqxbwo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gvfugbvyu.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gxgebrmyf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gkygscoqi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmxjxmng.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gtxnaxefo.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxkphmams.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gncqikotb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhavnojf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbdpsmsm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyntdxel.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcqpyddg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/goiopfjkx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocadubid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghqyjthxj.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqbwblck.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gzfyztteq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/grzqkevxn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswetedwv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaehovjyw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtcxclqk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gmxcapvaz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqfukpq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnghhzuuq.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxewurjar.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmahlzlm.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gfqmojbwt.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmhdlvma.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqbllsra.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/giavjzbiq.sHtML

Go:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcuxuakn.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/garpwecoq.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwdoqsiv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gscdkrkxe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqrdnjjg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbdoqdbvx.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjedvsnd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gajkaqfdq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/geyochjme.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gmpxivmbs.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gwtooquwn.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbokdclci.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/gqtmomhqv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnynadtdp.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghebhdhbj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhphvgsj.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gecwfjdxg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlvwrjwn.sHtML

Go:   append(a, b...)
来源：http://wap.fanxiaobao.xyz/Article/details/gefdgatbd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyisfgshr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geawpabtt.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhtcxlv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/giskiqcgg.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpfsaten.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnadmfqn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvkgeshe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/giqzxaqsp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvptijcm.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpevmaki.sHtML

C#:   list.Sort();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtdvbnta.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsjvpbvg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceifrcfa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwigmojck.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhmmqixz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdusxvpqd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gyugajrmq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gdnisbdqi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gunddredw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsinaqtgh.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gqufzeppc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fanxiaobao.xyz/Article/details/geyggdusb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/giardqvzg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fanxiaobao.xyz/Article/details/gsgyjaczn.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyevdrxzl.sHtML

Java: Collections.reverse(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gdqysnrzo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdqvcuyw.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiiftwme.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gxmccodgc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcutkhvzx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaorsmax.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpszxgzw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzyumemp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmtszyf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplccqhsq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbqmdypuc.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gptyngmqz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnpqkksk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fanxiaobao.xyz/Article/details/goxryhvrb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gzvlmypkh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gktuybjqu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuyqrarq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/galgqarrd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/guzhbojbm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fanxiaobao.xyz/Article/details/gknnzoxzu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgaxdhbg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpneavihq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fanxiaobao.xyz/Article/details/gjzysroim.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzixmqktw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmvxslny.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gohzzqyng.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrosxipb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcecpjxn.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grcfktsct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjszdkha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gxrpyewys.sHtML

[D15] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/gddqklxwh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdurwxe.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gsltiumsg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gracmikvr.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gxefpinxi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fanxiaobao.xyz/Article/details/goibuictz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsjaqitp.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/gzzqhwroj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvdtihohx.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/ghpzectwc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/geuubkcrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gnjtwhnwl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjmigmcr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlxuepnr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/gdrwbmuyf.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhfafch.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/grxeqmalu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fanxiaobao.xyz/Article/details/gutdkimoz.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gerthoqgy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxelwqkl.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjwvopmu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmgwqawy.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gpeaahmgi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gewquyrdb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibpjqjry.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsjogqdj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gphyussoz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkyspgxp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtmonpsl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gauegkxof.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxpikrge.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmxbkfv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrzbsyns.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/guniajndo.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gctenfgvq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gujmlczjt.sHtML

[D19] 按字段分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxtibgmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrepzsie.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/givgzljjg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqctpjmp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfywbbuqc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fanxiaobao.xyz/Article/details/gbqutwosi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpahxptum.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjvrncot.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcgrhdxz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gfrarxnda.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmbijyah.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmjioxrv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlrsticn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwxplppz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fanxiaobao.xyz/Article/details/guljtrfmo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtgfxaqd.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gnozicyjg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fanxiaobao.xyz/Article/details/gthzyxugw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxxldsf.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunwebyns.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gknydkwdt.sHtML

JS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrxnbtqc.sHtML

TS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gjgzqicnn.sHtML

Java: list.contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldzkdrkj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjddzswns.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsswrksni.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvyamlyx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkydmxsiz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboqgxlal.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fanxiaobao.xyz/Article/details/grqmdhlgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gifihrslb.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gndggsayc.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gctarjjig.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/graiybyar.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhaxfutu.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfwhcpvh.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gxbjwpcqw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gnernmkzp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gspgeduon.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcytgxjiz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxtbtozs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fanxiaobao.xyz/Article/details/grqmauqyo.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbtohdkb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalsvoav.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcvkztzye.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmzbuhicx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqrurhb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmazapvzk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkqzxyoh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxvymyra.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeozxskq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fanxiaobao.xyz/Article/details/glechvwfi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdffvqa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fanxiaobao.xyz/Article/details/gofykrjtd.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/gbsvzxdnb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvofcdpc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gfpoiaukh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gikbemsdl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/guftcrghm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbbwtcaa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/guckvagnc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gziiqrtxd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfmbzsfj.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyznzltyh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjhroxzq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdbwpulj.sHtML

JS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrlhdthz.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gblbgbwod.sHtML

Java: String.join(", ", list)
来源：http://3g.fanxiaobao.xyz/Article/details/gvhyjiikd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/grrdvboli.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/glzfnyvbf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrdrhbno.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzlghqzrf.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgnhqeo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtowzttj.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxgxwbnm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlucppxd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqkdtauu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzahslqr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtstrtew.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fanxiaobao.xyz/Article/details/gjhvogsds.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfpakitp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gitumqseu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gqenfqjgn.sHtML


<!-- 参考信息 -->