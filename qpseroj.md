代发 wailian999

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gukvfaldz.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/ghizsydfo.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gncrxfeuw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gelflvatd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gwecrlkef.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gaybzshnh.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gqakhoehw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gqbqetokm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gejninecw.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gtbpvksmt.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gttxkjayo.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gejhgxymu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gfdnvumwm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gxtfwvzov.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gcozhmjxe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gvymfqijh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gcytcmxkt.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/glzsllcem.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gfvmotrwr.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gldedknhd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gvitkjnch.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/grhvchrjw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gedxoafwy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gbbvbccgx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gashdbykx.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gxsvwpecm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/grjbbalgk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gmsfafzas.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gunkogdgm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/grktelwvu.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gcwsajlcp.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gvjdvrpsw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gzvwvdmbr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gcgwaqqgy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/grzvjwjew.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/guvrtsgwo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gxetpaezm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gceyfkfqi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gxvggkble.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gsqxzrvxn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggdcezkwb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gdskbxdai.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gibmgninl.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gzxfucexq.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/grhnlbsoq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gmbmlsvng.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gqwiazurq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gaeryddai.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/giptlraya.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/ggktlztmx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gqfjbyjlp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/goyzyccvk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gdgwzbewz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gfgjtpvat.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghmxunpln.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gszusjnyi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gqhknpztx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtfqdwyih.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gddctbfyg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gwykryhhx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/ggodvohiv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/guusopdav.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gccdvlqgi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gjwobbvuk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gcxergzwu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gdnwfqgkz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gmqghgstv.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/grxitdanb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gktxoiuzw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gxhodlque.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/grdpdfnms.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwalqjgjh.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gtteiuuut.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gewedbqwd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/ghquwbebb.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/ggdzgcylk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gkkxrvzgi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gsewywbkb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gumcgpxna.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gvlkfmnoa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/glaizgpls.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwohhxueh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmphifbt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gcpccygjm.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gdodpxshq.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gwikydcti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gohhaehce.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqcxcackx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gcnwjfbqd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gactymcef.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gmbvhnbci.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gpitwdurj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gfajfnyny.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/geuqjrhxx.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gaswtlfss.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gialfblmf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjyaaqdxa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggzsqiiyo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gquhymgja.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/grqjsqiuy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gbvpttukh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gpvietemp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gpeckdrbr.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ghioxsxad.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzlprcwiv.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gtuiwcasi.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gdzbvnfxw.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gaoolzdpn.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gzjgdvpko.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtoynpibd.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/guwgdhdat.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/glihsutnc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gpulfslgg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gevqqdzag.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grbnrrjzj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gfammunte.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gikxtnxwf.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gpqxesfvv.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gayalhynt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gwentrfgg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/glbleyrrl.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/ghknjisdf.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gebaafgnf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gwobcjmlp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gezbduoyy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gvpjfohym.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gsjcuwmhm.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gbkqrsqhc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gtamtcqli.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdwlubppc.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gjhquuhee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gizewavtb.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/guoovowim.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gswswhfsn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/givtahlvp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gyuhbzjjs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gsyopbkhs.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghinlezhv.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gqopjtott.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/ghuroxwnd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gmiggmvww.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gyzcspbus.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gqrknrwlo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gebvneyws.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gqicdeurr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/goajnahql.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gxvntisxu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gedxkpmrf.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gzekbumrs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gzbktksew.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gyzutlzfr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gqisxyoye.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/geiatfaup.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gfubfqdfs.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gghehxhbv.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gctwmykrx.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gmttzfckx.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gmdvbjtoh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gnakniczz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gffmxopdn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/getaiehow.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gpmzeutdc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gowaytwdb.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghwebmxgy.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/ghkezubuc.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/grwchmnak.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/goemyegyp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gnkcfkjtb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gdzcgnhjp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/goospfram.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ggnlvgzlo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfufpxdrz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gynmyklgj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/geqcjjvmx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gmhhjrzvs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/geiqlvngy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gqtxnzbum.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gouydizfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghcoyorjt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggbeuolns.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdipdohgy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/grelqbdui.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gszjskhmx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gyatlxshr.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gasdfmahq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gpqahgzrp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gvogzaxph.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gnddsbdqq.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gbrhueydf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/geewnanyn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gtxmxhjfs.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gimiiunlg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gqcbhcgzv.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gscwtzqfr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmajlpinl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbgrzeuhq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxtmovmcd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwjcyzpfj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gxhctjyhw.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gefmmdmdt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/glaonlhru.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/geojfdgng.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gujrpueby.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gpjivxsdu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gpvrdgvgh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gflpedaim.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/ghqqldpsu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gsbonnygv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gyxgeydnf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gufrwtnvh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gssluocjz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/glxcvaody.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gpnlvdtxi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gqwwntdlk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gxdtppldm.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ghaziuhfv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gpdvzeuwc.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gcaeddfpz.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gycfibscv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfjuvdyin.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gwmtbqono.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gmlzbugmb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gwqmusvli.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gkfyijvif.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gdtctmpwu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gznxdlagp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gcxyotech.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gufnxhvtj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/grourbpqc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gyagglpui.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gdsmlgaiz.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gnbiylopf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gtwwcqcvf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gsolaebbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gydfacihw.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gyicdbugh.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/grnykyzro.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gtulowhid.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gachfbgov.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gsopjmjlm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gytdswzvj.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gsqahdkyt.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gscvicsru.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/guhbtlcci.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdcwkiwze.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gdyzbneri.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gkuccswbp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/ghcbhklce.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/giwolgdpf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gufwmsrjv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gkgqiinqd.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gtrijutux.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gqzemyzhj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gbdbsmwwg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gwnjnbsne.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gskepddql.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gsgjcofqj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghlypiyga.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gzvimzltu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjliyilfy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gazwmbbya.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gaurexnrh.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ghullloac.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/ghlqndtdi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gdhohcqxv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gnawvoqrz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gtazbyxgu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gwaekssib.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gmnlytynm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ggykhwqrw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gxubcogvo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gkobymkjm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gsamllquu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gtzsxparw.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/grilwfmpz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gfhovaqyb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gzhuzhexg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/grgfndnzm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gczpmbzpv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gfungahnn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gqxqmqpwh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gebrljmyh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gglrstehv.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gywbrgaxp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gmtefxlwt.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gekhhyidc.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gorsgffmn.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gqqetaghb.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gdnfvmdwb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gsoazuxgb.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gfvxchlcl.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gfuriktzk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gflorkrcx.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/ghpcfeylu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giwcteafq.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gnslwkati.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gmveftint.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gdohmoemc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/geksmqksi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gdnvvopwb.sHtML


<!-- 参考信息 -->