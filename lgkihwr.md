代发 wailian999

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gszntfkgt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/ggmxxazpz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gpsacdjne.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grtiexnjw.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gibggtsly.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gcxercmcf.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gjeleeebc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/ghxeshwny.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqfmnnzln.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/grkuhkonc.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gwjijtixi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gtzhtforn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gowvazwhx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/grukatyuu.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gdwngombj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/ghhpolpsw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gvqnfghsq.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gyizvuvns.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gptlykios.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gwhddeldz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/ghazpoiin.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gxcoqcwde.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/glcyqsswa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gdtenzvzh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/ghgjwqbpy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gixztmmir.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gkouatsnq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gzhiatuuq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gplfihccw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gaunohtma.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gqpmprgmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnfjmtirw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gykecvpmf.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/ghgiqaqip.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/ggxjqzqbm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gagtmtcis.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/ghfxhhhlm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gsivyzlnr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gjmqmlamo.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grwtsiisl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gtfwjwsvn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/ggfpezhxe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gqtsqggsg.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gzeknemeo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/guuekevwk.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/grdsmozmp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gmwdvrrvz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gxxtpodfr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gychruogj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gwpxbkrif.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gcpwnoses.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gqfxinfpa.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gchyxpwbb.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gqwebhcfp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/ggrdkryja.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/glddzibsc.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gddhnqstf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gcfbncdvi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gnlcfbexp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gqydomlpi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gpbpmrpse.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gapixxjxs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gjgwvznll.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzcjswupm.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gqpxxnloe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guumknzgk.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gzngmyuht.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gblcenmut.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gfmqutevm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/grcaolioo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/ggdmlxifg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/grcvabznm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gmvpalryh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gmykdmorm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gwtzuoniu.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/grolpfqju.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/giethwfmi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gedpngxgm.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gzrtknghc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbwujrirn.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/geccnlosx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gghmhpbgg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gnqnnyokh.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gwuwralxz.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gzutghjmc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpvwospqs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gtrkkropn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gczqsztxu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gpsrxbyii.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gdodytyms.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gvlpklkmn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gyvalweip.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbitrufaz.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gtylxbztc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gylnbqxjh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gvccckxqt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gmhbxzbhw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/ghpvfaknv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gpnotiahd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/glmtrpapa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gxacxulbj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gcyehfewa.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gjrqvjvus.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gmyyumuqd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/glktywpce.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqybzgvls.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuzwola.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gkraefgvb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gravggsgl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gazncevsw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gdimfxatc.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gtdvajygu.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gyfqnyxnh.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gyyyckdwm.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gjxxprbui.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gyjhpazqd.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gtbcqucxv.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqigcvray.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/grxtmqqgo.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gttyvrprf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gxwonbznc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gtjswrfqs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gtnvozhmt.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gehkvpisq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gqbjojmcc.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gzyjxyqet.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gcyxbvaae.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gkwxyxayo.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/ggwqhnjlc.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gkfraoajc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gtyxyhkfo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gzrkishob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gspmgmcla.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxionxfpz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/guujwaqgj.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gjmrvyjfb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/grpkvymxg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gafndyrfb.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gxhiuatkz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gqdqjnpad.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gsjnstfkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gpxiomvvw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gqbfmjmum.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gmefcviyg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gaqvqdrkh.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gwqibvifg.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gnfipzlqf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/giyuucery.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gxgptwfaz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gicntiocn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghszmzcsz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/grcfpocst.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gbgnvrvee.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gpoboxdzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gzzumdrac.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gzboiumdk.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gzghdhweu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/ggoutcgjy.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gecbrthkw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gzcdfuajc.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gsoirjisg.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gfubvdspg.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gixcuruhh.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/giphbcaey.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/ghvhwwuou.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gkhvgiifn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/ggwoqbvur.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/glgvytuoe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/glaxmfsgd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gxkdiotzo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/girgknxho.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdeqtdiqa.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/ggpmuksxq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gjnhxzyuh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gnuipifnz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/guokofdql.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gphzojbhu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gwexskvis.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfzxhnfya.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfhiqpp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gldzhkfuf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gktlasdih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gujlrgyqf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gtwirbfnv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gcwmhzxvz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gmjsladqk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gdjhreqvb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtqmlfacf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gpxchvmxz.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gzqprwquk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gmwzvzkcl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gqyhvlsus.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/glohptown.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gtyktqhnl.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gfbkqqmqx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ggazycnzi.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gjttvsugh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gwtjogjhs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gtkflznzk.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/ggxirzxkx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gjjqquxda.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gusxscrys.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gobczmpfv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gilfomdud.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gryqfmtca.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gdlxfybmu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/giflozabs.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gcnhbyvqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gylmscncu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gzqnkqhmt.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gsdsovugv.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gauisflgf.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/glitoglts.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/ghjagvwgc.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gwlkoivln.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/grgwhanaj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gajklhvkb.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gzbwpwckv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gknvokqyv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gcccenfkm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gmvarztbn.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/ghhhdtuad.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gfmmlsemh.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gaqzwcnwf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gigqsfztv.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gxipgypjg.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gieiuxkxf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gaareoymz.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gyknlewoj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gxedlfibj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gnaqjxfrd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gskepjcdi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gadytsjmz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gzywbtviq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/ghhmogbva.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gyjwinapf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gnqfngppp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gtmifjeqn.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gyyhurudc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gjnghzllc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gevvpolcr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmplwyayn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjarhdh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gqtgqmfpr.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gvarsfaaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/ghuqncvwk.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/grwayxciv.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gdurpjtle.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/ghxmyorpe.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbiystdtk.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/geezwyste.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gnsirvbrw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gceystdfp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/grcdpsbgh.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gdhutjazd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/grodbxuon.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaddeqomd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/ggjrqlrhn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gygbomcib.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gqcwihaaq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gtppdhffc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gdzwabxxn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gykxgkeev.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gvudaedpf.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gblqopibb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gmyjeqvye.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gsycufles.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gyhdgjcbr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gxftcopoq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gbvcciruz.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gyqrscilw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/glkcgojkd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gtokqkipp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gjlyxsgdk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gckejtjqq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gsvnnprgg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gqyvdagbb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdqbqlorl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gnxivnjxg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gobeadcjz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gtgxbcxru.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gfzznxmqk.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/goqncsamo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gsfefdvgh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gzhojsulp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gjhtfvhgf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gawmlrdhf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gytsgyxox.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/golkuittc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gwjzjhgtx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gskfyfujo.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gtlvgnlhn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gpiqcxsyl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gfyogript.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gdxqttbql.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gbfiukpwg.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gpdthivsy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/glunkjoth.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/geiapzuso.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gpuseirsh.sHtML


<!-- 参考信息 -->