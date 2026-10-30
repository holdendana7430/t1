代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gginehnlf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gwdydzmod.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gpmecdrws.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gjbaegsrv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gbavvjdpl.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gleqovwee.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/grdxtpgxq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gflhhqlux.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gqabiinbp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gjfhwvhbo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gsrifyrsc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gjblyrona.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/ggvypglhz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gtjnwxntl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/giiucvkuc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gipvwjdkn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gnioilaxk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gsbblgmqf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gbqurepvr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gyxbveuhy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvolscjmz.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/grdgsnwja.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gmhstjifl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhkxwbf.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gnqrkrodm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gwbxlycqr.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grrukovgj.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gyoovxdoh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gccbahtvj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gurzczgrb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gkxvronud.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gaiiiypub.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/geaomciio.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gndfjjjxn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gbpdbmbcv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gxcgorhgg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gkdkegmxr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggkkysrpq.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/ggtofomqm.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gmkdyyjwm.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gcjrhgixh.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/goieohwyd.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/girefhpcy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gyliqukzp.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gdndkjjze.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gsmjtiebs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/ggijmyskz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/glsvhjmov.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gpqeeokru.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gjgpxunmc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gvqkmciwe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbovgicuy.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gkclkdano.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gisrofoas.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/goioxzlhz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gskbrnhes.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gggoyiunv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gfjtujhez.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gmfgihihz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gwdnnlhng.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gwxqtpbhs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gswfmthtb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/ghxhfoniv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gyvgvxitt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gfhiqpiwa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/goutliupn.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gzmjlnvei.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gtjcifzma.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gxksmschc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxxnfkizk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gylkcezsy.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gopbgvyjm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gbbupthny.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdgehdnfo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gxpwghjnz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gfwidyejo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gyvyiglyf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnfbmaqqn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/glyotynef.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gcaabxfdk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gsxdfnsqe.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gkgvfwbny.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gxyaawzsy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gmvzeunze.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/giomzkinm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gxuicfggt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjtfnwrex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gwtpceteo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gkforpfvh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gggmenyig.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzniqtpvx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gjpakszgx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnydhnwgf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsmvjsjri.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/giharkvvr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gbtbymzcm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfpplxsgy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gjzdgprhp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvrivfohf.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/griwqrjcv.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gtgulzvzs.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gsalcronr.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gxpqejkid.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gcocvtfxi.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gapliqmvs.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gaqpcvwyj.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gdnnjwhpn.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ggjzqcfjy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/gltnfzcno.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gmnoynsue.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gbmwmdhyq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gyhkqoidv.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gstrndwmn.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gyvjjiyqd.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gfbjjiubx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/glkoinbcb.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfkllttwm.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gbfncxtrl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gbgcbbjuj.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gmuknqxfd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gvranqwhk.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gjipjtpbh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/ggomtyxvf.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gqsequbpy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gdqnkubgl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcjcwojag.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gtxzujksm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gmckvdtki.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/glhlktlly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gxfqgaxik.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gddbkzdcl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gtkcddedv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmjsyccgo.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gxsgkgmfn.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/grjueuecp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gchtkwqqx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/glhlqaprw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/giuondxdv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/goioiwtfu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/ggifklkik.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gdwisadhg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gnlyubptn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gbddztwyy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/grygngglh.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gfongnbye.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gqvizvopk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gfbqnrwqf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gknflleuk.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gskypegxd.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/glfozezky.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gmmdeuxtj.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gwqfobjft.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/ghvlnbggt.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gouwsjneo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/giqwgwpew.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjaboqzt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ggmcgufub.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gbrjvacuj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gwiwjcyga.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gnglxcdmp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gcxxpridj.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/goreobhow.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gpqkyljfm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gsjjjayqe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzkvyhli.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdqmirtqk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gevhrwzru.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grksfnnyv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gtkevlkjm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gxugtobix.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwyclvh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gxuxdownr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/grupknlxl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpusmqlhd.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gsirtfbnq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gxlhvebtt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gwaykxzeg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gltybcgbb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxrvthmhi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gflbqdzrc.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gtrexpuwp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gtjmxqejn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqxadkxay.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gmckxvpdz.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxgkqvjgt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gxktjiyax.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/grbkvfdjb.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gbtdduvvo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gkjuqilnq.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/glfdldhon.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gmdlbyllm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gfezprkvn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsiyuncsq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gglokvssh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gtazzeawo.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gvpzrmyap.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gptoedtss.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gqwxdgazh.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gjbeffxaz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtucadywe.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gptgcpshb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/guvkhgmbb.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgljfedc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/geddlauuo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gfosssxmj.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gfaznhrek.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gnyudfbvq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/grmngwrwx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gclfwfcuq.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/glhwvvchd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvbtqeuog.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gendwjtts.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/grgymtdwx.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/glbpwlmqo.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gwokeqmys.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvmzvolep.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gecbzixpj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpsmnibsz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/ggtioglch.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gouxrmcbk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gjbahwyhn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gpqlgwpbx.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gccirwfzq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gpeaqgbxe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gjzvszudo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gqbconrpn.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gyuiqlmgp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gxlcaixss.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gadvkxomn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqazskfok.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/grcewsicf.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/geaacdivd.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gdefygnwu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gynofekin.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/godshfqwj.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/goxbexypf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gtdoovjii.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghbqjfnnt.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gumlrpttt.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/glfdsyjjb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gthdznufi.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/glxiaksnv.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gohjmzely.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gbneldmij.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gfzedplxk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/girkxjuzz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gnrrybyrq.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gdzbwawmk.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gnplligwd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gkxonwgsk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gcytfbthq.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gohacoznr.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gspymsgbd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/ggbxpdapz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/giyypdsur.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpuruzmso.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gomdtbeti.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gnaaxporp.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gndrhxuuf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/geizjpqqf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/godlcyrxo.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gaiexlwar.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkiaspgn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gfxxkoqvd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/giuifejrj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwriikoze.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gewsehyon.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gdthtunds.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzurnko.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gtwudszlt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/glaeiljkp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/guzmgnpmx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gdjmmhalb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/ghuqajwfy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gyszullgy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gfyozzkdc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gaeeuobmu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/guounkqcu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqsgxtfcl.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gunlkoqbr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/ggnakjhtx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/geseuhsxh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/glvepcoeg.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gqfodbijh.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gcgbcqzne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/ghzsmeyap.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggeeixitd.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/geacvpdog.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggirhnlvz.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ggdgfhmwx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghwkruhoq.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gygsjhevw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gesfenjhl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gyjijuzjk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gmpqqpgbi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gsshmwisg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gvvhzwjwf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gpzkzvsmt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gcxwzjyuz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpqvbkzhz.sHtML


<!-- 参考信息 -->