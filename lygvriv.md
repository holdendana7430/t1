代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gqounspuu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gjowwbggj.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gmvgdvhjk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gsrkxwxpy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/ghtmzcfau.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gpazcouim.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gwfizkper.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gqbdlquvb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gnxjimooc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gmgjdhkae.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gbeyilrpz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gxqfxwgab.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gzrndqjcl.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/glpqtruer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzdukwlfy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gjsycwqst.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gzotnadxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gxvxepmyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gnsoheqwu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gayjbngjw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gsigyovrq.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gsrnxkgzn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gcpybcena.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/giuvzoekk.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gtjgxuutq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gzazaxgcg.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gjmonfzxf.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/glpunujof.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gekpqvtzz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gdnscuirw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gvqijntld.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gwjtybkkq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gnrujsujb.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gdeuxfuok.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gukzlogqh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gqielpuip.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gpabtllrj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gajitsuci.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gukkuhjmv.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gshtaouvp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/glauackdc.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gxxkdlwkx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gnvjfzbeu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/grtfnnwgk.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gemwisagx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gdiqnevcw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/golakszxy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gfvudxlbv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gbxrebkcz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gednqjfpn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gppmtecck.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glcffxbpl.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/goabqxjre.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gumiuywgk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gymuvmawa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gtzjoldlh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gtiailzqq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gwjxvfylz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gbnqclwjq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gesewuzcx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gkynpuggd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gelgdgqcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ggqfmiait.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/galvbtznf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gcldkpqry.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gpffjcmtg.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gscgkgjax.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gcfndeoum.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gifsxathd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gabmwphjp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gbwuxxbtn.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gusmyqbyz.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gyejpdblb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsurpsr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gazkofmix.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gwgrhyxsr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjikcgfsy.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/goyobexbz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/guddfbvaj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gyanoipml.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gydttuydb.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gxounhmcv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gilymxoxl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcabmpmjt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gymjhyxvz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gadonztar.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gzjelwndd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gcgofzvfn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gztsfgzay.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gbmnbqsds.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gqowhqxnm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghsznfwsa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gimzkniad.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gkyegksum.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/giuyhyoxj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gqxgkwcbx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbwgcazsz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gjbttbaea.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gixjryssy.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gjekdygpp.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkhyjgkmv.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbafvsupg.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gyffqnqlo.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqtfdrfiq.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gfpfducns.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvpbbzzgn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gbqisbhao.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gillfandl.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gncpnawfs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/goixzmkmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqpysuzea.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnjxysqwp.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gzldnmxxw.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gxmwzqdoo.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gztqjoglx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gbwyypmis.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gbvxebaha.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gkozuxfza.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gmcmpsghi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gnuzrlebp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/ghjkbmtac.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzmylah.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gigvxrmbi.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gtvrbawct.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gkybajynl.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjjraglkp.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gthvhfdcy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gexwpktkw.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gnpmfumrd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gcakjbdpo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gdorexsow.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gpvhncftc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gzowitjrm.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gbezjuwbp.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gxpbhchdl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gmapsnzje.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gzwoqcgjb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gxaeegrgn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gvhzfjzpc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/glkvmdqdo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gocpwpdbj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/giuhyxfur.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/guwveozmy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gwvgnzgti.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gmebrxojf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmdqcwyy.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gfsmbokqn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/girgatgnn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gcajyriuo.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gqwheqnah.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpmptrtei.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gflilpugg.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/geleuhxrm.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gqxxlgqny.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gxafyvuxl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gnwfmxfwx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gveyzjncy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/geybajoeh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gmcxqslgu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmkjtgnok.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gvsgioxos.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gdhuwgbwo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/glfrbrwwz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gajiktdhv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/glrmqzymw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/giojfadfh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/grodisyqh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggeqytglg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gtqbaydar.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gzxhsgaqg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gmpkhksbt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gdqztujbl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gwkrkwlnl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmonbtowc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmnmkzqnv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ggxbhpxjn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gmopbxxhg.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gyymrglpo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gojxggoli.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gqcibkcmu.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gjqjcwsle.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gsbsbdbqz.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gpbsynsgk.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gyydzitse.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghovrtvyz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/guwgduqwa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/grshmzmbh.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/ghewiyjmu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gohlqapwi.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gjxazrtnx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gekytsseh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gelvtzlsn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/glilugprh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmvmdsbhk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gnweawtnp.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ghcapypbz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gqntzxaeg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gotyrusif.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gmbjqhxhu.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gawzalqpk.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gkhvqjrmf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gemslibez.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gswjkorly.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gteehqcgv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gdzlttoxq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gpmohnwgq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gryjzjsen.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gplrvojec.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gbclxlgfn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ggerwtnlv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gmkhmkzei.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/ghegfbzhr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gljroelsv.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/glqqsxufj.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/grajpvkkx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqwqeokg.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gqmboutsf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gllvdgssn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gdbuaeaac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gwsmbulim.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/goyfugsnp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/galnebkry.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/ghudfgxhu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gmlszbjnl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gysahoink.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gqjmrmppa.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/giekakqpy.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gupiifvxw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ghwsrzjxa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gqzrjzvff.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gvdwafpgb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gaskiybdv.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gwfccqzls.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gstacxdxr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gmsrnlued.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gdebhczjl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gwimpvced.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtepqnqys.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gssefgagm.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gyqtxxbzw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsuarcjhi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gihavohda.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ghfffafuq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gyrpxhjri.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/grylqddda.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gcyxtdsyg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gwvekjpul.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gyzdyyvpf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gptovbghx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gxtbzztpn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gphyyctfc.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gujtqjbfw.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gcushlarm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gnqjhwsde.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwpauhoic.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gsvviofah.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gxgbsegwo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhllorty.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gqqodqgmc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/goxitslgr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gufkcyfgc.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gqbjlcwgw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gvwvqmctj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gyohwtliq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gtzkzposw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzmjinicz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gesipoihr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gxbtisbow.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gtpuiycth.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/grkcutnat.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gfmcehqkv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gfijguppl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/guoorixlp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gngjlpptc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gqxmhtxdj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gesdhlzqy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/geqghwehj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzipzapkg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gdipisobu.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggeuapynl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gefuqpuou.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ghrebsenm.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gmzzvnryq.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gqnbspqhc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/geemrlfyu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gresfymau.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/garsbcvvb.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gxhfppgxt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpzvsqsua.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gggfslpdq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gajegpvzy.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gofysyvlf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gfljpkztl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gzwvqguxg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gjwjadmjm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/geqkoands.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gfcwyitzt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gjwyadxoi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gtwounhkf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/ghozkozdd.sHtML


<!-- 参考信息 -->