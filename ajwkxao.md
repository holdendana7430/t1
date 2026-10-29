代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gtaipjpvc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gqvotxxhk.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gzonnkruz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/grlxsybwi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gfzdetvit.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gkerknznq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gwxqakwtl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gggcjfwsk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gzoqjjkir.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gxvwvhdfn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gjopfakcl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gbaqfkkfu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/ghkfncclx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gjteejdqi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gdaxxxsvu.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gphlcttly.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghbrbcxdy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gibjytcti.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gsbsxboau.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gkcqgjriy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gsdmfucsn.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gfzwryjms.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/grprlqyzr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gweyamblq.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/glalzevhm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/guxholwfc.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxhzmcakg.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ggcojmrtj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/grdmaoszr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/ghctaovhl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/geihiwydg.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gvzmvgxxm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gafyoczwg.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gqhsewovl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gkfzgrfbr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gzuygmuul.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gzenverbx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gbgeocpzq.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gsvzhhkei.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gupfougib.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/grgkmmmoe.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gasbsmwps.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gmzntzqvz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gmaejlpeg.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/ghmjjngie.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gwfeuviok.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gkjfkekse.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gpqbqppdn.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gnraaashu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gieiescxe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/ghrclheys.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gszdiwfjc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gkbbixenz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxurcriq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gfagmozii.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gjuzokbad.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gedapfsmb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/giiofmwks.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gfpertkkk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gjgdxrrlr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/grhjxczfd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gelovwjhb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gthsatkeo.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gsuzazdww.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gllyqekbk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gritvgvcj.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gsemqakci.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ghxduywgd.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gwcaflfik.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/grqarjwoh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gcygaztjq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gorvcoarc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gohfzjwgk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/glyrrqsbj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/ghrcsddrm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gjlmftiuu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gvidbpaqa.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gbykpihqf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gvxzcswsx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/ggeghqhgm.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gjuwtxwld.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gubcquviy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gvyimnbof.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gacibolkr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/glfjsagph.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gagfohrgs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gjclapdkp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gsnkgxooe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/goprjyuqf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gaulfupay.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/ghkartpzt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/guvmarcts.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gpptidovh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjrxwrfaz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/ggdsmirng.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gaikzhadr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gdhwxxich.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gonvwqtxw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gworgejrl.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gzjuodgxq.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggilmdzzj.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gwipybiou.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gazklhdoe.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gshhbxzxw.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gmadnghmr.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnuzxznpw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gezakopjg.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gewdkmvbf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gbtptbvdb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gwcxqrdhr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/ggyewjpze.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghaduxzqa.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjemrtaqc.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/grpukyrim.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/ghrwclzfo.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gtipwcwxo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gondqefmn.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gkactsmbm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsxkmowcp.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gubdlgnvh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gpxzljokv.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gxmaavwvz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gkedkbpxw.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/graknaupj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/ggtupfxor.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gowiihmmx.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gvbyntequ.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghlfczohv.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gzdkukkwh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gvdhbshht.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gswdwdree.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gyvshvvqj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ggkoiqjqd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gjrstzmlv.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gcqgvusst.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gxxmuffqf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gcbkbraav.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvgxquj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gkusuhkgo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/grfoeqpdx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gtydugafp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gvqdisnbh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gjshkbmyp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/golcwrhca.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/glaccvwyt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/ggvwuaifq.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwyxrdao.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/ggjjnxppt.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gprcdetgr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gsnjifkje.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gthhvgrxo.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/ghmztnmat.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gqnxmkcyv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gahsrawzz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gleycnygl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gfuvtxten.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnmroevkg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gdyloxejt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/grbeqedmv.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gkkucnygc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/grgysesun.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gkzzvmdew.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ghhvwwntp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsarvorhh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/ghrvdqsfv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gymnekgts.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ghmqlwwpc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gwpdejhho.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gtpdjaysd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gdwevsnke.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/grvcoidme.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gnykyrpgc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gxbkipqwz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gowwywsqw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gzmapyowm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvcazokoy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gcoigkwje.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gwfwpkctd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/guvidgesw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/ghjclnoju.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gpsabbjio.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ginmvbepm.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsmyeniuj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gvbgkpsfo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzzjcnfdt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/geyaywree.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/ggiyxfyoq.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gylpyyhwi.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gbtrspggf.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gabnfmxyh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbuxckdie.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gqjggexeq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gtprrdire.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gjlysnqvj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/glycilyrv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gnrjkvoxn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/ghmsoenkg.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gnhjzfcij.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gymikvznm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqrdbwtie.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gzucysimp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gbfhprdpw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gegmhnael.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gfycipcwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkxlvwlka.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/grdxgupfx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gxvociyav.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gqkcviifw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/glblasnes.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gvpnzigcj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gtkpejyot.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gaeaakjtc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/ginanizcf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gsrstdsmy.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gkfruduow.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/geofblcbi.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gxerjmhao.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gbbupvpdz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gcbtduijz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/ggaukdyuf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gvmkvoxbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gjaobhhdz.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gvmiarsqx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/grlwnuhnk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gwlzsonld.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/ghuhlgelt.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxvpmdtlx.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/guschgpil.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gfnjgmcex.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gzuhrmngu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gjiagfhfo.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/goohgyoji.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gindryert.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gfkkdshhv.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/girllfrdg.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gkmorcxqr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gwideconz.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gmyxruxiy.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqtrnymya.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxttgytzy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gldzidrdo.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gpjbwmmed.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gtftmyovg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gvjcailzy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gisgodsxm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gzmjdlfom.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gafmxmebv.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gtuwgxuvs.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gehlqyhed.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gedsrymma.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gfitdrtnm.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gtjdhspih.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gmbbntdcf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghkzrijrd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gmtccddbz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gfgazuxnj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gunnjxzub.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gcjrjvczk.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/goxnlaqoy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gvhpzmvdr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gtqnuxxgu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gfiiwjtzv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gkawrzbdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gnqzminru.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gobsxxkcb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gadlxnktq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gzssxhvwc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gzqpmsqis.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gaokqlieo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gqzcqtzao.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gludxtgwz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/ghetnypxk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gualsxuaf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/geccjtkai.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gnoxlmahw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gjjrshnro.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gcfhwdqcm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/giynsuyde.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/glusshdds.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/grpvwsyrl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gzxegdcen.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkhyvgpqm.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gnmivfplr.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gygjytzlv.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gqvgjapod.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gqjbnqttn.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/ggxdnmpml.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrrywhm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbvrxcwxr.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gsztefyyr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdndsqupj.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbetgvgvj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/ghtaysrmt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gfamsymqh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gjfewqqlm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gjabvbprm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtgmtgq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjjncrxte.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gmqbjybhx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyismqjqz.sHtML


<!-- 参考信息 -->