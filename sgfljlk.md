代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzvezoajy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gywawvzuf.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gtuyajqmx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/ghrpapaje.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gcynjjbeg.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gepzwgwkn.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gonzsxarl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gqnncjytr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/ggkzpblay.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/geopmsncw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gtvaqsxgw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/geinqmgci.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gpesgnlhr.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gaytaxfth.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gfpsrksxk.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gpinraeoz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gfelfrvkr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/guuruiqri.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gmqqxzbzm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmvmwsjyj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/grhbwwbeu.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gfjjyxfbo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gekzkfbva.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gnybiqthe.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gpwbmgtbp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gutwwumsg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ggqavckzt.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gasclcbyf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gcxlbdllw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/giklnzyrc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gvpaszjsj.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gapifhyrz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gsaxqxwdn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gugcrbbiy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/ggykcmopg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gawgxpsuk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gbwhqgcmf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/givdkpjbg.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gqoyikwsq.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gyhzdtybc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gcxsnirrv.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gvmwbfopx.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gqbewwzzq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gbijbbhak.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gloknpvrx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gejsptlnh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gwgzgiwes.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gpevxnvzy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/grsjhdxzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gasnrzkjn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/goujwndbp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggihxxkrm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gbxcovqsq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqhxevleo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gpxrgukfb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gwhrtofmr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gpzpefyog.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gomskwpnt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gdvboevwf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gwsxjnkyc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gudjksdnv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gsczsammr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gawgcpyrl.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gtjgubbux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/glzqhabxc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gqktoxjgi.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gpgsvjrem.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/griykqfks.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gabccdzlt.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/grxuzldmx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/giaamafxa.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/godbuyvwz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/giovctdpo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gfalaqskd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gjefunijj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/greokkdif.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gyiqvglnt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqlrurmua.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/ggklzissx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gqlxlpyel.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gtrcywidc.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gzgxfwdhn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gjqyotwhh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/glqhczlye.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/grperuezc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gmaxuxgub.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/grbodqgdr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gnaxvirnc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gdqqmyphl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gsmhxgimx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gnagsmtfz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gtflpucul.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grmabavzz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtmkonqnm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gggydbfbe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gtfzwmqax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbafxbgre.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gwkypmpki.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/geporwmsr.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gjxngtmjd.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gslcnygat.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgdtsuyo.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gjvnxrptw.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gadmsspan.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gzwblwxkx.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gpfrqxtjg.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gosphllgo.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gtybpvubv.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gkotqotod.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gvlbgzjow.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gjurgjmdw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gifydlptj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gejuwcsch.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/glbwmuppg.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gxemhtnpg.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gabegzxez.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyiboahee.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/godbfelrk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdylfbklj.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/ghihvduao.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gunzazpzg.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gupikovcl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/giovagkwk.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gefngaomp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/glsresxva.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbmpouywx.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gftjnjpqr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gvnjfkhoh.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/ghofeowvv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gzcmdhsjl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gbvoavmbv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gpwwuuiha.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gexdriiov.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gwmcollws.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gleleztft.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gqqattgao.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gejgycmsq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gbfwhhksi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gvmzadhzr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzcxxpliv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gfzektctk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gcqmnpyri.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gzkpcoeoi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gvhdcpzql.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gdjntqggr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/ghtgfrjse.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gzvexzjmi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/girmcmcjk.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gwydelrau.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/guvnquhdz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqnjjlzsz.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gsfmvkbic.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gntkbeays.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gzbsnwovh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gdzidqdgu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwwtcnexc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gaiexjojh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gzdkwapif.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmsaheclb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmvgbrtdg.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gvzpphjhj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gasihlusz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gjcvosszm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gcnhjcygu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvsiqfvcr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/grdndvqxl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gnnfgakrm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/glctvdupt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gatjtmltv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gqvfiuexc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/grjygixbp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gssntxket.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gqxtahkrp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjtxzbtds.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gndyoszeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gouifwfgm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gbryysutc.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/glqdjtpki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gzbxvckzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gwwcdzgkn.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gduuuebht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gkynxodrb.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtptkirmf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfnpkafyp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkykhwlba.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gzbmczhxv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gmttcynsk.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gnkgjnmck.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gecsncwjq.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/ghtqhvwzf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gqoolkzhg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gemwanzgz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gluisgscz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gwztlxuzg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gvjupmizn.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gglyrtfto.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gmnvvjkti.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/giclujcmk.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gddkbojnd.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtziksgbz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gxwzsisoz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gnuhvizyb.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gtkaoqghl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gglqwaknh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/geuyrtgsn.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gzhqnwoki.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gxdoaskjq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/grjwyhjat.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gzplyqmvt.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gxvxquspx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gmwpamwsk.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gkjsjbqax.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gqwigfxtg.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gpsjxtych.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ggmjknoxy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gmzjanoic.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/glzcmnguh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gmzpigrlq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gjqkifcvl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/grgehcoqs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gcmqsyola.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/guuqqedjn.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gknrarmsk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gssfrnszp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gptjwyrfw.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gxoisnbaj.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxsarkpyq.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbcagvcfm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ggnweviwh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gzqihllut.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gqkvpoabr.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gslyikkgb.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gnqqdknch.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/giotlylps.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/glwobxuzc.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/guawsmeog.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/glwoykoew.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gjelwsjic.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gkovsvpei.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/getyqppac.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsbifhrsh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gjsjepheh.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/giuemulic.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/geioezctl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggggqqirc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gdfxxlwdu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gcsnwaxtn.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gpuuwnwed.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gmhfqdsde.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gdbwiyjeo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/ggrxvwjct.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/ggtszbucx.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gxsjroama.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gjuymspqn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gymphvhkw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gibwtalee.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gzbnozrqh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gfnwpvoxl.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gkgerrguu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gatwlpmfb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gwcoesnep.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gcvyesrzm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gwznxmmtl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gbrbmycou.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gpxuxcbub.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gixvazuvt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gaaxvrnix.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gjegcsyml.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gypfmneua.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gijeghwmt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gurcsbcoz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gluyzgwaf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gxcytkgfh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gmsoorrxk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/glbubjlxu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/groigodfy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gucklemuv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gwmmhfopr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gtwpxavxt.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gvwbxputb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gxfwqiwqm.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/ghsghtdfn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmldslfre.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gfvpexqpm.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gbupqfcrn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gqwgrzsfl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnftmwcep.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gyrcbuidz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdfqujiku.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gjyavvykv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxdiredid.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfzmuzqeu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/ghziwqqik.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gcqbzopmk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gsqnosdnr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gozzdhhrf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gqukwswnb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gnvqbpihl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gqwbirvhn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjrgkrgzd.sHtML


<!-- 参考信息 -->