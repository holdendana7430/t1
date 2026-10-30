代发 wailian999

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/grbknpvfo.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/goawnivda.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gkqyaatxd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gxyqenxpz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ghmjrvnuz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvknuoq.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gqoufvqtw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gxeqqocyk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gomfrvbpm.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/goukyzboc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gofamrdef.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gsotjcdnp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/giwfkutsc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gqhehlnmb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/grhfahrfy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gyvmroyrb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/glixybyaj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gthqzhmey.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzbvgqhaz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/goyuggkbh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/grrgfmqzn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gxzuhwmin.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/goxdkkgbg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gkljncsdj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gagppnujc.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gqwszjagm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/ganfxitjr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyxuqitrp.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/ghkesvpws.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gaigeiydd.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gimnzeujb.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gystqufqn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/geokyngfv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gvjkffxgy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/geqgweopt.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gkfebfrnt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gvqmusyqk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/godkusjkm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gprzsefdx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/groheilop.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtzfubaek.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gxdyvqtci.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/givdmszng.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gfcseezoi.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gsnyccsqd.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gyorypdws.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gcqpelmme.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gzihylzxp.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gvrjsjsmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/guphgojoh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gpxzrjkzn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtpvquwdm.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gvgoywbbi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gdwrcgbmp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/goxshtmqi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggmfvlarc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/ghxjgvvqf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gddfbhhim.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gznxbuyqw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gcppkoywe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gbayxeezh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/garnmihcx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gwghsrizs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/glptgbhrg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gevcqtozw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gieqrvzda.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gwxemmqrs.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gikxvomyo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gvyfwkxzk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gffujvfjg.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwmmgmkib.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/glcrtdwkv.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gwwdochev.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gcavtyzkt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gxjvygxwq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gkrkayzkr.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gsgeqrvch.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gdrrqndir.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gwpugeyez.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gmqkpvlcb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/ggzxjtmvs.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmsjllxim.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gxunzmdtc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvefujqwu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnbufnvvr.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/grdepvhji.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/goxtpbbsg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gxhnikbep.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/glkdwqxfm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gygtmqmar.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghdojmluc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gufylgfqh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gfdgohqrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gmduqrujb.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gukdxtpwn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gxnulihdm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdymxydst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ggelntoho.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gcfzuceom.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gjhcjjmgh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glinzkfvj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gwfrcllgy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ggpfbuxvl.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gtuevmkjv.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/glduoezuc.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gqwksoztn.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gsrhosvlt.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gcwaucpga.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gajpqalhr.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtguveits.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gbvdgjajv.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gwxmmqxtd.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/glpiukvao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/grfggthec.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gkkqtvovz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gingoxpgx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gnsuqbozm.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gsedysbwr.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gvmtguzeg.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gkwnnbfbl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gmzoxmfor.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/guptbtawm.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gjozdjccb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gjezzcjrm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/ggoqidvmd.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gzfzgmnag.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gujbzjctv.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gqzulwdtk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gyqucpxmy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gdakhcmrs.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gvunrhqaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gvfywszwc.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gzryjcjua.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gagebkwza.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gjpyfewbe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gebvszmhd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gtzpaafbr.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gnguiluqz.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gzqebekgj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gttmbuozv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/geexmrbfh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gkcmcozly.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ggrmkwcga.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gckkofzfa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gjltxrlth.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gxioujmzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/goxslfnhj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gfwivsrrv.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/ghpwvbqop.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gjaffohos.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggnxlsfyf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gsolyixwe.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gccibtbwt.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gpkotjamf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gneuatowo.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gvhbkuthh.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gzwevanfs.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gnllfwezb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gessopqrv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gofrijrqw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/geubfbcih.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsndtuobk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gjibitzhx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyzwcvbel.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/glwxrxefp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gavemwrkc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gcoorddcr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/govnvywmg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gxikoyaes.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gqfmewuby.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gxqlknzdz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gjcjiigcj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gnbzfnxnn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gvqqpnxbs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdkhmvkle.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/ggtfncnya.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gjslclwmb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gabqirsip.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtmtnjzvb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzugfoutn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gwjoualqj.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gbtoaznek.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/genscikub.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqmxfvrun.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/ggzhbzjth.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gksvnbcqx.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsqbxutxn.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/galgfvirw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gvyqsbwnw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gkjugfjpf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gkjehkkea.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gandsdext.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjbbkidkj.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gfmkuwmzv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gjpigoqag.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gufvqzfcl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gugjvwzmn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmtmbbydk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gvvdkdmzy.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gaxhhmbjb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gjnjxfkve.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/glhzvqatb.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gmerdotgi.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gmhtvexzr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdkyclrri.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gcdumjapg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gplplraxx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gyyqdwofx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gobajoriv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/govejqacp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gthfderro.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/giycyxxoz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gvydcgrdb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gihtpfqte.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gnembpvwj.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gohgtwwll.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gmzkpdrja.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gtgleqqnv.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gisigvtkn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gugkillfl.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/guskddemt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gpssvtfzj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gqqzvbjsj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ggohttgsl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ghrsyvkvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/ggbuocswj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gquiajpop.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gqjdtjtmn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gwqvfuuhu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gvpehjnne.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gcuystnyd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwopjhxce.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gvhvkadhu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gplpcghrn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gefbjtzpw.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/glxixmqtl.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gzuopgoxw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gpsgeuhls.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gvwqweanj.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gxrtinapf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gqdbpuspl.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gmfemkhhl.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gunjqxpbi.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gcrisoiql.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdrwirczj.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gcznhonjx.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gslqryceb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gkvbuvmba.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/guiqlvcpf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/goybtrftp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gidfsrfxa.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gaygdexum.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gpclmlwtb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/ggqnyccww.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/guguoxlre.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gmlcmbnfo.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gnvkrmixd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gfqoyocak.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gyqborbwz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ggxwxjefx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwblmodhf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gsekvazdf.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gnouvvpru.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gfbtnrjzs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxzmzuqb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gdbqjzqys.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gveujinvf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxlpjssaf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gxaukjdsu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyagklvhx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gxiiikijv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/ggpvhcsfh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gkxiuosag.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gthtkqmmp.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gbifyvijc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gobijhoel.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gpcoayric.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/ghhrbeupp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gfqwckbfp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gkcodwsmn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/ghtsyjxxy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gbcwwqxxx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gbhiyfhnt.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/grfghgnib.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbtpvvd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxjvzrjd.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gatzetuji.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gfliphoxb.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gyignfylq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gqtbzxnsa.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gassidyft.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbmwanpvl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guvdfldqy.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gvntwvvsx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gelmaqdan.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gmrraqgkn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/ghupjklbc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/ggillfrka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gbjcaldez.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gzkluvfjn.sHtML


<!-- 参考信息 -->