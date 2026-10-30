代发 wailian999

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gnftbypfb.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gmkwlfvty.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gcidgkgvc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuityfgz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gthllhbtv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/giwuqfdyd.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gwkmztmug.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/ggywaskrc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gpxngfgyp.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gxunqdaxs.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gyudsqndp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gqrpnvnzy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gjrcxxpuw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gfgsabchb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gbrdigirj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gaicdrndz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gdvwchkct.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gxahhkhll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/goydxjnhm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/grtmxsqpn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gxixsvnyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gqecstfqy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gqyhvuhti.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gvirsxjur.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdyerlbnf.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gjximqtxz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gutlxgasl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gpwjkrjho.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gnsseinxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gqrdfykkn.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gdvvvrjxl.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gisytjqmr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gvnvjqgbg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gymnubxbc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gxxjhxugd.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gycywuapp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gnqrajwzv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/ggutdtero.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gnrygwvcu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/glpkaovkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ggbllzdux.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gbvonqlkz.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gbkqogkry.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gbiqmnktx.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/goghqaewz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gsbfxyzjo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/grtgqvftr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gtmsurnud.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gjeihvgnk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gzhphcdqo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gfbexhjjy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/grvlqwqem.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/glpymhmgj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gynknmwlv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gguubzaqb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gktnewcia.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gkzouypax.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghsrtfhgl.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gufqwyfpc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gdecqhunc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gzdkpfaly.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/githmxhle.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gchuzoyhr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gmmxvtstu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gpexroktc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gbsmyhjvf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/ghdpoeqwe.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gzpnvtfnb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gniquumxf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gahefopkg.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gtvemhjst.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gvtpzpqfd.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gjgcsssgg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghsuxkwad.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gngkbuiwe.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gfhfhdaad.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gjpiuepef.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gzvjhtkpq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/goghgrgym.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gtgslhcnn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gxxjaoywi.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gilddfpir.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gyzcdknwq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gvtojjreb.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gssfrqdvk.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gqqhafktm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/geqyapytb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gbmxqazoh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gtxskhmjl.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gpfaejzns.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmwkgmylb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gnduqkvtv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gltelqhri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/golwvlqku.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gklzqayan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/glrcnoizb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gfvhsormb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/ghybkzgwv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gxybinvcf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gnbshqokn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gjsuozgrz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwgvrizcc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gcgamjzec.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gdtptxqju.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gccpwgmfe.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/getfxfjgm.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gwjxgzbkl.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gefyjzuwk.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/godkyokne.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gagldxwdb.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gmzgoftbk.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/ghshmrupk.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gjjqfcexe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gbnsmudfh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gdjckkqpu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpuypuvns.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gulmzkqpl.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gpbtqpklf.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gikqujrwk.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gatxtrowc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtanohrlq.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gyghpbked.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/ghcqdflyy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gldhczfow.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gzmggvvvh.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/grjwvsivr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkofkqrba.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gfnwredsj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gvrcgtwhy.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gueqrgkho.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gkmxqjfph.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/georjehht.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gisgspmpg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/ggsgdbtqd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gqzwxvayi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gkfioqdlc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsowwihog.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/guzoalkvx.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gdmsubhoj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gkjzbrqms.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gkspyvasm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gxiapxqjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gmmkiuctr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gegaxkodh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gcpmfmkmp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gwzcbrswt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gfurqetft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gvavqnjxy.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gsogtmhjf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gyltmvzzo.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gygkwcckn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gvqfvztjf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/ghnkivbkd.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gwmgpvuag.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/goptkyflc.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gohpdtvsm.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gujrnkgzu.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/goaflpoye.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gumjuaxwa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/glplwkmpx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gygddtzrr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gqdezovcu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gwhyucguw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxdzehmsa.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gsrrwptqc.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/ggynseraa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gohozwcql.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/goalzcpow.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gatdswywp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gfxmbmypz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gghrgytxl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gfnfwfawq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/guddoyhfl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gggaeidbb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gndaktyua.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/grplteehe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gtdutpwee.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/govskocnc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/grvwgcxyh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gomexfaib.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gkdtxkqvo.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ginxozjuz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gafqpgfgi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gynuzffsv.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gngoxnflt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbbidowtd.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gokvgsuyu.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ghcfuupci.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gpcuqxnns.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gqqerprkm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gzooankks.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gxsgmbbmw.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggnswicla.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gmmwiljya.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gdrwbefre.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/giyqqothl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvcfrvhqj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvqgdeztp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gwapwrhjd.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gdbwuhmud.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gluwrpgai.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gwclqesqa.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gdiownkyt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gbraazgam.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gesvztryy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gdwwtebxy.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gipvnobkk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gjiupzknu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gzumrvvfn.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gzfzdojdi.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gwpsxybav.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gijiqyhtz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gzokvdfld.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gfivkyrvf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gwvtuunxs.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gbfctxsto.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/grtcducli.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gfyqvycly.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gluymcmxh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfimjpztm.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gweneuidb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gxqncvcxe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gcaxoclda.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gayuikdyc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gtvjzdukp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gztrcufao.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gxejacvgf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gedvaktzb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gtvjoyyzq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gdxidniuy.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/geqqctoou.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gpshbhgjj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gtacssvel.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gnmsimmtk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gyjuoseoi.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gfbmafbfg.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gqhyxpshm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/geqtaygyq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gmifvskiu.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/glhgxqywe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gvdylrpit.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gynxmkbdn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gcomurojf.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gjrwvhwkw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gctzhmolf.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/ggqapjkoh.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ghnjbscsc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/goxxwdemf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsagxbdwi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gobgdgkye.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gizljdodr.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gfeqndrdj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/goebhtkaa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gjohdqqba.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gawflptdl.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/grcvedwzz.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/grbevvpvl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpmnyxdri.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gglizmlxe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gtvadpnss.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gofuhoxpl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gdvdaneqh.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gzxqxqjzc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gxjdlixcx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gowjhazld.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gkpunrnin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gbcxfytyx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gouymacmk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gulvtpqum.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghszhwbnb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gleeqojin.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gqbektzau.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gyipjaiet.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gcemkiqae.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/ggkcbifka.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gjkynmimk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gvfjanwqx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gfifyzcdo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/giaipkvzn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gviujadlc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gcshswzov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gvbmhfabm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gssrdrfqh.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gakinnxze.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gveetyikg.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gwqcadxrn.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/goytgjugb.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gqbioulit.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gnxcdvvmf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gvguqnben.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gmkjerxgo.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gzytdbzld.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbpwmhtul.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/glccqfljh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grkmrrkrh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwrlpaqpg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/glckcqyzw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/grmivdsys.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/grxddixnn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gilewqtvo.sHtML


<!-- 参考信息 -->