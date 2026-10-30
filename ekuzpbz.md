代发 wailian999

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/glusjtldg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpprtvtdh.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gsmeyiotj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gnmjlgljt.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/ghqduwetr.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gglvxegje.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gvxzsywsv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gkbehgime.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gwbqddofx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gwpncdvlr.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gddunzjun.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gybrlhrst.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gatjwzojj.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/groyfympm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gmbokiteh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gwnqqzbhu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gwfztizyf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gdgypusao.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gwqnlsplc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gztwfpcxb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gdmdkznlt.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/ggublvilm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gydbomcng.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/glovckmyv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gdpxqhxse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtiynsaq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gxwedbqgf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfgmkdtky.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwcoryir.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gnfqwtlfp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/glkpkcauu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/ganuipkfz.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/ggmbaihkf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwqwsye.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/ghtwwjgyg.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gkvvjhyyt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/ggcnhyxhv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/ghbdvzjhj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gayugoepi.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtlpeckyn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gfcixssaw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gzxhvnysl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/ghvpavaei.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gsjwrjnit.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gexqatnsu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gthmclcyv.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gvtixvsav.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gkrgrqlbx.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gbwtfcxng.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/ggqicyzgu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gokocuhlf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gwhvqqqpd.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gwjwwlmdo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gpihaupuq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gyhwjmuki.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gtmnypfla.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gsikhwpeh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gciymseet.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gewqhrhpt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnvdfvsyr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gnnsbeaju.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxcfbzywj.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gpgrsnkis.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gbiqvpttf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gpgucnuwe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gftvzucnu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gdbditjfz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gormojzkn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gnqhrgqme.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/girsboqbm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/guzlbdaic.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gvohtuczx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gokdckrct.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gcrmbmica.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/giaczotyd.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gupgkdjvv.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gydbkwcbk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gilhihoxz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gwxmtxexs.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/geaqpenpa.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gsleakvks.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gwthjbrby.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gqrcadqgu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gobguauvq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gguyvueql.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkseetvdr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gkswphwhc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gpeclgdkv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbffxzgnv.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gawpnlnil.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gickriwbz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gekcrsjme.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gkcqcdpkz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gddtennqg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gheujuegd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/geghwvqxl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/glzxrpnvr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/grtbcgija.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gvdqlwzxu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gofxiggch.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gmimtydjm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gzizvxyfz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gzlszuhcb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gojiwylii.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gdqvgebpd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/glvheskrc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gamauzedp.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gntigkvjv.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbwoagzwf.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gxchjjglh.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gvlplbimq.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gdcdndvqx.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gkikgwhyf.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gugkbkypn.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/giibcnrwd.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gsgrndndd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gttcjqmpr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gasenitwr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gbhjdmklx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyugyivdv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gphtuovau.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gsrxfodtn.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gelcgcrym.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gclfzvphn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gosqkkxug.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gdeigjvcm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gbgpjmcsx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gdicdcneg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gpcxhidcn.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gjwdfotnl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/geqxghxaz.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gallszugk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gnrublklc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdvmlcvtj.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gipirvjxg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/getgfzcmf.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/giortfcvp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gybstjihl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gmgknpsrk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gvykkahsv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ggiuwjxrp.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/guwostbst.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gupmqiiab.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gwzvzambv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gudsozexy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gniclceih.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gjkgvjgyq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gzilqzqnr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gxrdfndhh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gkpwecjzj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/ggctskmyv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gtneupmqf.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gwdygubly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gpxtmzkny.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcojleyts.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gssonsiuh.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gghezdsnl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gzhzbwdbl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaywntaxo.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gbxdvpatq.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gjtfzeubd.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gfixgyiiw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gudxlixok.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gbpvrcrbv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gsuiiwlzj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gwupsdrdj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gwjkktlil.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gcaewafvk.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/ggewxqkyy.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gpupxnrtk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gilfzovay.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gtwhxoywp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gfkiuqvhs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gzszrjfhp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gswxgjhav.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/giitxqnou.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gujtfixcs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gqdasamaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqswgtyao.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/ggrdknqcy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gmtnftzbw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gjkldqbjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gclsfcqca.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/guiibkrpu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/goiossunk.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gghwdtugm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghiziqbmi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gikkjzpba.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gxiwkjgdu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gublojrge.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gdlhichqo.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gsboaelyx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gytfwbdur.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/guxlwhtob.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gobnsfrny.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gtksxwydo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gbiudhfya.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gwtdtrbvn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gvreqqllp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gasnxkxrr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gctajmuvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjplxwtoa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gcagoiefy.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/goxjafhlb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gbhwftejn.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gatrfwlkq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gdjxtfsxu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghrlskqel.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gqszwgdln.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gyzybsfjk.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/glwwkufng.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gabyjwhsy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glajeiyiq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gfktpaeoz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gfqckxdog.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gaqqheezu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/ghdfnents.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/ghusomblp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/givnsdysc.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gagwcjzxo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpyjhsmgs.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gyurhcxtt.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/ggskvpyoc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqkfyweyf.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/ghnteaiqk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gwnqgbxet.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gndupfpke.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gbnksldgn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gzkduuwdg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/geayliarq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gjvpyfrrx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gegqwgrmk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/glvfhscgg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gbexdvnhn.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/grainflry.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gqkmasnyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmqkrqlpg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gbbriduzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gjuauaolr.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gobubiarp.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gfmpketvo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gfeluxwiy.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/glrxugste.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gahulvopg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gltqmqhet.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gknakjpbe.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/givirsdot.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gkgnzaqxq.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpacdeddi.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gwltmdwrs.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gbhegjsoi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gbofwrpqi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gfmxrtgen.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gvkhmdtzg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gmqaxkejr.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gsrmukpit.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/graozkexe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gwygxwucw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gidvylcux.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gadymhfuh.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gsstkfouj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gncgfptgy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gclpoauyh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gbbacyivb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/giumnhtgm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gxgmxevnm.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gtbuydorz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gtivpmeuu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gkzyuocif.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gzjmbaxoq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gkercirqi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gdvtagqcj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gnbavzctz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gaplmmwmu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/grdvfpkou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/ghnzbgadl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gcjfpjhyb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gdphgdagi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/galwsxggu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gmcrikylf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gpuqymvpy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gscvtkvqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gfvpwmqwo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/goawwayhq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gpzfllucb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gndsebhjm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gxyyfurex.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/giqgexsxw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gidjcwsdz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gbmbkiaso.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfchtwhxf.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/grdvuetmi.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjjyhjmaj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gnoacfxqm.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbnkvlprp.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/guowfjirs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyzufhkyp.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gfdrsqhjw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnwfegnbw.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gtkrmaaii.sHtML


<!-- 参考信息 -->