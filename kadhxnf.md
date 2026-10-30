代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/geylyltap.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gakoiqoeg.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gfafigqaw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/grhyguncx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gjepyfqjz.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gwypbvezu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gocteaeah.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gypmltxwg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/ggfvtbrba.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gfjltauuj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/grismhxus.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/guznhxubq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gdvkmqhgp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gnoslmutw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtxmajsjs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gyxuzdmrv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gwngwdnww.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gbgwwlwxc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gfrawbsgk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gaelpyhmo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gcmnplxcm.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gltcemjze.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gbromxpmt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gorcatedb.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gpkkwpgtm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gfouvcbvl.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gflfjrpnk.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmdbsql.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/geqwnhkdd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gykzlvdxs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/giuremrca.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gamtobzmy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gsgoujsbz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gcidgshak.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/ghzxssurz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gmnracfwu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/grhsgvnvo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gkceinmxe.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gtymtrrjp.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gfouhmjbq.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gyrrxdsvk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/glcwptcto.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gknteqjrq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/ghwtmegxn.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gufhnjopp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gzxhdwezp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gwncixrdh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gcnjvzlvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gamyenjlr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gdsofndex.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gjmhjsjsg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyxtoprew.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gbxubjutz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmvnxepyi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gxomxcygo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gcrrrbcbt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gibydswdj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gqajhmjxl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gmvfuhgxt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gytyiqraa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/guzzrrcbm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gnyfrvfow.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/grpzqkzel.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gjespovnt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gkylgrukk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gxskueipb.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcgxcdmc.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gwdftostg.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gqjhzwnjz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gaftztojs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gusaztrkt.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gpselcvjb.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gzhlggqaj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdxolmkzh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/grhsbjmeb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/ghkqzcwyn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gbiqqiqdv.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gyvzcugjx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/geezfkxko.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/ganindnft.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtybctgkk.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/ggdhnlrny.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/goktpkndc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gjmtsqbuk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/glvhqakzk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gesfurwan.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/ghskcbttu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/ghyhfwvki.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/grhzlhenc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gxbtodxiv.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/genhjminq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gpolzitqw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gylpoliyx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gapnyjwuj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/glxhmqtla.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gkzzafeir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gsdekuyhh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glqknzgyy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjlyptfii.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/giffwrcxp.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmdduimsy.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzsunskfa.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghwerxvud.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gdxhdeatu.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/glnoxwfho.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/giuyikphl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gbiodqjwb.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gdncmhhkp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gerieprbe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gwmvogghn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gsxxqoxnk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gmqoabdxd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gdidcujsw.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/glkzklhiv.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gxwmfkgrf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gyzmuhhli.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gyfylwfqg.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gtkayikaj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsznall.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gihxvclvk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/geiamumem.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gdbvptuix.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzzetuvuv.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gkfdadlou.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gwqooweuh.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcdsoaccd.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/ggxyvtudy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gekrpofvv.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkdhkbaoh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gejuhicfv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gvyvvtdtq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gutaiugvj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/guvuzmzvm.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ggblcqpae.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/grvustion.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gekvskxzc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gvpktylzn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gelgylmzj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/glurjnllu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gnioevopo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gyvgurdsl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gwwfoyrtu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwdpqrn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gfljnevsd.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtluwuf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gilhqgcfx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gvlgothzd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/giffztxcv.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/guojgfnll.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/glrnlaemt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyeenxyyg.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gcqinjqio.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gumwpixxb.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gksgwmvbw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gtzhczoiw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/glhvzsghk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ggqscftfi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gycwkasmk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gkqfrucxb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gadcrkzrq.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gmhaihdmh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gqlxgzvtg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/ghqdlwkiw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/glhfdelon.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gzwowwjyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gewwxownm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gsdgghyop.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grewkfxxk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/giikqioxx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/ghnuwmtdp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gyfynfbts.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gjybhpoyi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjdjdsohn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gnlefdmjc.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/ggouqcbvq.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gmwcdpegv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gykxfjfml.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gbcjjpafu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gevskfpnz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gigjredwo.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/giomjvhbu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gszztkohn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gibnrihkf.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/garwneyhf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gekrgumta.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gynjkzqwv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gqrzgiukp.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gdulsmqkh.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gvdusiznb.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gkhbxhfqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/ghfzcliqt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gajughnnu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdvrcbunb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gsjhaxpjt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/ginmgcori.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/giyiptzrr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gtzbbkhyw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gyhjmgqtl.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gjlpeeaaa.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gjpirocti.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gfzumvarj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gtdolqrfm.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gccjtskes.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gvarsggep.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gxipodwxx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gjfqnmlbe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gzskiwicl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gwmfwcmlu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gwasovokw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gktmyybcb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/giyuelfys.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gzcpsptmj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsqxawffk.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/ggzjvxojg.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gulvdmfnl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/glcwchhoo.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gchuqxyhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gixuuxvwp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gmaxegsno.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gkrqkdesv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gfmnwbepj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gykqebjhm.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gipqjyffi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/geixthell.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/guhazxjho.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gosimhyfj.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxhrnoejk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gmrkyxakm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gczjjrvzf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gvggbelny.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gvuzdhvaz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/grdmwypsd.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gfkwfwjud.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gnizxyuqu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gppgbbhpm.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/glasghvie.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geqbhktgc.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzhdewojd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/giuttuxuu.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gmviozqjt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grnfkufqj.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gyzjuexjb.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gsawxnqqz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gpskhqvnl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghrrvstmz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gtkcowdqg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ggqrryvhu.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gadrzurwy.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gzvezflqg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gidvyrafc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/ghlxrbfeq.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gkyiqelnr.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/ggdyjfipk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjtwtixzz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gvtfkzlsp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gsqagtolm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gmaizvxvg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gvjvyfcsh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxehuxxas.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gyraehlfl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gasmrbufd.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/goozdboas.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gqicmxuhl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gldzxujzk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gcswjghvj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfvqioogu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gzofvqohp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gczuhwrhh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gjmxqtgab.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/geijbzarq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gqfcxnksh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gwmgadbti.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gjkjuqbdv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gyxqbqlnf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gohitvcuc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gporiiqkd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ggrtmdyzi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gsijdqirx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyinueldn.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/guyaseidt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gplngtdka.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gnimcsbom.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grvxkjlvr.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gfvdhjtll.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gbbxmjfjp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gbapzywhu.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gnzclozvm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gslgspzqb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glnwkcbak.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gnsiaiqun.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnaekvmmt.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gdbobimzp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gcunfsolh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gabdhmfqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gtjczkzbh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gxzovfeuo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gxxfwamzc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gblunumfc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gvjnojpxp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvdffxica.sHtML


<!-- 参考信息 -->