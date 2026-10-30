代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/giwrieygp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gouodtgmj.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gwjhxgvte.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/groqhtfor.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gqgyufwnm.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/ghufvzjhv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gxxdyndbd.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gsjdqueeh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/guzesirxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/giktaksbw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gejrgmafs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gdczuiptv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gqzdrxupr.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gxuyzbxvx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gehdowhss.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gzsdjibtw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gamcmchkz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gkikxfjdi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gnyzogcym.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfqijriye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grhxbcost.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gakgnaopf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gehrbpdjt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gqfrfkbrw.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gqrkpkofo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gnqebrrnq.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gnxwekcyf.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gwzlbqbxi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/glcjrgjpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gxiisjkdk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gqgxetprc.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gfrkbqsfv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/giczvoyeq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gkvdsxdle.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/glidvhvwr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gdmdxceyi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gykfpyoho.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gthgrkqev.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gcuwepjgc.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gghskhohi.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/glnfozxqr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gtmmvraac.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gpiyrqvjp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gnvwlgosk.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gjnucgfan.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gertvyhut.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gleqjhwzj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gkfqlxdzz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gpxaebpuh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtzkoyhho.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gdtetafby.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpsokwtlx.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gzvnqkdle.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gognerhoc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gkvcrdfwe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gxuatughw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gqpjvqrnb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gmpmkdisj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gcnthqwdl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjupkqz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gtuntzyxj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gvifkskks.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/goioymlsg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gsukryskr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gnucwusgv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gyydoqosx.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/geppnfyec.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gcmukwhsl.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gymcwqqlq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gnzclwhgm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gexqyyxfd.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gbxxofuvk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gxpavhklx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gymxytzhg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkagnrpax.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gttttskhu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gwvodpfku.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtvbicjud.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gqagdlzoa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gxeqweawa.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtcdebunp.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gidwzenmp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/grbluajro.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/glpmjpgky.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/ghgxepbwe.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gqsrlfttu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gijrasghh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/genlptqec.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gsnxxumvm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gmwjjyhms.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gyovyvtqw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqoofootf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/grffewmvx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gyhjvrqwt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gdrfcdise.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gsbtgmcsv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gygyjrtua.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gcfqtkvvq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/goluiwywx.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcpynuwdt.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpyxbbqby.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gioecjtyp.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gtsufzffi.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ggjuoputs.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gdadxjmap.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/govkoezjs.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gdybisess.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gigpiudlq.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/ggoslqksi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ggazljtez.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/geyburcxq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gtprlncmh.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gdxskmasu.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghjqolgru.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/ghhwicwwf.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gpbsjulnj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/glclwnwhl.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/ggvrrnxxh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gtkyzpoyi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gcqratiyq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/ggaifoqdo.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gizaoiyet.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gcyecemha.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gwyriqkel.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gjaprqifh.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gzvvbmoso.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/grlntsnhu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gksqwfkst.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ggkkpelur.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gjbuxkchi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/glyshivqq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gkuyoynsv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gplwtiaqu.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gbffdllcw.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/ghkagzolm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gzwoqnizs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gxnnxnuvk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gzqdupalg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gjlfelfwm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gbejpdibx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/godterriq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gvwijleey.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gogyeshos.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gtwlluwhw.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/getclpavn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdeofmwm.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsckfhvao.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ggvwgvtpg.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/goymvbsqp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gztgwgptp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gzufctmjo.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ghuiryzlq.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gdisjjxwi.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gbqnxpzeb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gbjrdkscl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gcjanhamk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gvqqdouxv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gsbasqpyo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/ghviorhyi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gugdsbdbk.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gasrnxcoj.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/glvmfcape.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gmulerwkd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gklnpvbac.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghsawxfkr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/grbmvhcxa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/glbpabqpg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grrydfbjt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gicevyrbx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gwoyywteg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbyovdayn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/ggqmdwoxg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/grrgjcooz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/grzjcfkap.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwhdfmoby.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gegjsrbkd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gbymnveza.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gmdfzyble.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gdxdlvzyq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gouqocgnw.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gyquhtymn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/glrdbokwn.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gggjficjo.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gcygsdpyn.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/glrdcvebd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gopiceszl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gmoaephyn.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gdjtsbuxy.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gkultazif.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gjpkrtetp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnlieidns.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/geeaycexo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gzhajsglk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gbdkryobt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gymuzuxfg.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gwbwibawd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gyzolyged.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/guzvvdwkt.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gqnapdeww.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gwglonaul.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gywiuosjj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gykccfzrq.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gzvevmxbb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpgdukkgi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gklwtsimp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gskugxlnq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/ggnvwqgyt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gcoudeavg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gfmkwiaeh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gyzitsfsz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gyhhzhmfw.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gwgodmkoi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/ghmxoaqtb.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gvoozbwcy.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gqgvuzajd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gauuyeiui.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/grviavmoe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gxgvhnghl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gqalmmsuc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gqafqgopq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/ggqtqpagk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/grsfjidix.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/geufcnsbu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/garinpdap.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/ganjfpbne.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gbivshxlo.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gacfjgtit.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfdgvwlyj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gqppabhky.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gzqrdtuuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gyorsitvk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/ghbazklcp.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/giuzssmop.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gwmmceopx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/grcmuzoyw.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/glqjivcsy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gaxqyyfad.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gakhtiyge.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gxnsfclsc.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrlxjhsf.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdlzhjgtd.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gubhbxloa.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqmdrblkk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gagetqiqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/giiltzmpy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gdpdjqkzs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gmddrjcnb.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/glqtfsyxq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gainhmzcp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ghonyoosg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gabixsrfk.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gjkidjxof.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gypjdtqah.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggiiohmpv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gihernplc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/goiyhhrmc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gulbxmozh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gqiqzubrg.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gdkhwsimh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gelchnoaf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gkffkxwzs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gogrjntiq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/ghtqtwglu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/golksvqtb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gyzpnlbdg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gskreokuc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gdyhjtmhu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gkoprjmjs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gfxmloecs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gdbaaxnpj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/guzajltre.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gcgosdenj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gagkzbnmf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gecukobji.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gwxlfxhtf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gjoxigtli.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gfxuazkcp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gsvlhzfbz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gyghbevnm.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmojycald.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gufkbbkle.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gprwnjpmf.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gysslvujh.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gajbbkdzs.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gplvhiohl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbgzezg.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/goeomdreg.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gpslgcqnp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gynwncuue.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gmmvqubzd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmupysxoj.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gmjfvtavk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gebjzccep.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/grmowlrti.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghvodssaf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gdvowdjiz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gflpwfzfg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/geoywvdzy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gpnlvoelr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbzhfdgks.sHtML


<!-- 参考信息 -->