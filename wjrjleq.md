代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gamnmihmo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gsijbqoad.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/ggkblepvj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gkgkyhhpa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gukeixkju.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/googlygxi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gakwxxmdy.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gunklhgfp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gpuuqmmrn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gmlkmyygq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gyvsrtjdf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gwbeuqhsy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gtbfepgbh.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gkarzgzbn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gqoqhfuux.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/ggfyhajng.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gjmislfih.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gbcozdbpa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gtyydeglm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/glwqplpov.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcihmwzpe.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gcipcojjy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/glquiinbv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/giwtuczxx.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/ggtqyfwaj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gqnxedgog.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gcdqttwsy.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gsjyumbde.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gjnwtiihi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gwuwigjjd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gkpmbbosn.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gsehuuzge.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/getkgeuja.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/goiskynwh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gurphnfzp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gneuuasye.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gjuaozsok.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gabqgkrol.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gzuezzjkx.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/grmhtrbgo.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gedgzbvej.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gogynzusp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gpqvolcot.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gbwjzrenw.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gkeqduetd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzyzhvwxc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gcyzxcbbb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gdafzmrwu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gbjnhkcti.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gjhxkvtem.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gtwmyapvn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkekuvaok.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gysuxnyam.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcjmgzvro.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gmeibgnko.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gazxwzohx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/geyepmopt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/guvdbvrvt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gakqewknd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/ggvztsbgs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/ggjhkkjbr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gyfweayfu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gyudjgmjz.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gykzgobkx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gxtorkebh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/geoogfehg.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/guuyfnkek.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gclsdxeei.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwbdqtzry.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gyotqsgsy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gyjexsiou.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gvhrxzoab.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gudijdsxf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gslkbmoeu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gblwqufjw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gphnafgoa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtbfsvzkp.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gismrvfux.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/grxrknhix.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gpsuirhzl.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjggnzbgn.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gogaranng.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gdevufjtz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gnaopebrn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gzxrxcikp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gmuaeixhl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/getuebguw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gamfuoxsr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/giqzwssqa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gqaowzzas.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gwbbsixeq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gruwcsrfq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvebkprke.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/glypquvql.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gprnefatd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gvfantrdh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gjafurulh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gfcmlelwq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gymupyhyt.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gezrawabl.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gkdnodiun.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gvwzzgrky.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfmvqbc.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gcoxkthvv.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gypettmdi.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwyvblxcc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gknnwwklv.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gjnopzkdi.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gidecodna.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gplofkiof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gxysftmcz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gvtapnecu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gsbjcpweo.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gfkuxivyl.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gxkrpjpee.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gonpnmbin.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gehcsilws.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gllqfhkpb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ggvjcjlwi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gnjahmmpe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gihgbvqoz.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/glklpmebx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gufclbotk.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gmjyxagnb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/getvmrcum.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gnqcdjkra.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gklcuqgsi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gkhjbslyy.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gbrpuxqcg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gmieigxuu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gpbwloapu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/ggrajmlqx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwgreqoes.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gcxirggam.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gilgcbgza.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gygmpndfc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/govtkpssl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/glnrbpylf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gtyumopij.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gjzhzesir.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gpfzfydco.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gpyowzyda.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gvdkrnspf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gnhwkjrcq.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gyxapzciz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gvgqcowza.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/geuoqyohx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/grdsmndjf.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gukxxuvlp.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/ggyseqnyq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpijloqpl.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/glddcuoqo.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gcrmqkdkg.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gqblltarf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/ggoimdhxk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gectjvhtu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gvycdcdwy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjlcaiszk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ghkagtylc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjvhywjd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/grfweexlz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gdelzikqp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gxatcybav.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/giyikmkpr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gafrnehsa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/genhiilah.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/grbidamyi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gwdupkoez.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gyvdjtiqm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gnijjynyg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkhxejx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gvcoikrix.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gztbybyqv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gxyuyirif.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gcgihbimn.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gifottwwm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gnwgttktd.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gxynkvchd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggmxeavkm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghejnflzl.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gqnyygqqy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gjgigraaz.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gasjlstqd.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/glgmvhxhb.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gzfwcptpq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gsmmwpftf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/ggbdghfuu.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gfcwkljsv.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/glotafvai.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gzhuetmho.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/glzsyxxzx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gxnxojewh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gnneftuen.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gahtxwyym.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/grkqspubq.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/grhetufoz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gtwofugmh.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/guxiqazer.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gvjsapdxp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gepzfzqej.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/ghfahixpp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gjtftvgnk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gwjnfvxxf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gaebdvnls.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gujmfbvnl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gcloluqbm.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gedphcrcp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gzkvhdqwh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/glhdzykdv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/glfxpfvsi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gyxqnughw.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gcacgscfi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gkyhapflh.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gmvuukdzn.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/grxvmhqdz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggfymvbot.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gavnkyklp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gdsbfosdw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/grbenqsid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gdzofedve.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gduymjdvv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gbaaaiyhd.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gkbsbkpzf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/guenerdsx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzwzhefzr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gtirqzcaf.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/grdmczitm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/grzubztuo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gqqdvotri.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkjemigxn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gnqjjesoh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gnzammpyr.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/giqxxwevx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gcetubxpc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gmvrjmdpx.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gjtztoupu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gdvvvmrgp.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpiithtao.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkmrszakg.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/givoclxxo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkvubgn.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gktsfwejb.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gisthlnwa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/glosgdfej.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gksqvgcpz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gyigrtxxy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gcmcwpmkf.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gtqstgkkd.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gbhacfzyj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gwuxfrtva.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gghqomwnl.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gtzkmbsgl.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gshtumxkh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gdryhppva.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjrtzgbrd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gcyvptjmk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/giqnrybyy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gzvadkqkl.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/giajznrfk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/ggepcjyrz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gitnzmggq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gmjvnecqf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gdfersmjm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/getahcnzj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gzrwzkgsj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gttbttkqf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gvmkheusf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gsdisldyu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gayoervoa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gilrvalfe.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gldgulhnr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gcqcwssvk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gbbnzyqyi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gsopwlkgs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gszmaskdi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gyspscjwn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gnrnullje.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gpmuvmman.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/ggcbfmlwm.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gvvjtnbgy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/giscwavik.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gxahknhsk.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/grhexpvfn.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gymlfrqde.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ggwawrarz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gpijezcgu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghzmucbhy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gsbqsrxiw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gixkjblfu.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/giiqeaovf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwjuyacbs.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghurvgnbs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gisypzfbw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gqevtgpfz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gopxvsmtc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gnsuvvvkb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gxrkstgca.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gihgmzrbc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gbcoqraje.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gslxtjhbx.sHtML


<!-- 参考信息 -->