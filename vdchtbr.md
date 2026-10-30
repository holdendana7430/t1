代发 wailian999

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gddilrvys.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gwmkfphfi.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gltclmers.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gveeehdpr.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gdlqvbxjc.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gzjevmzka.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gjvqceegn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/glrwrhiyn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gnnyohfii.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gqmtovkwx.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gokaoxhjk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gwsnnxprj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkmqgdd.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gkegberhk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gwvchjydz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/ggumesffi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gjnweyaim.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gmakndwjj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbjqmedqk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gnoyrfnwb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gmsgaizew.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gbenyohrs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gfpyijfew.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gfrwykujt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/grjofvxld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gibbmflks.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gylstlwne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnmnkodky.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gpbrjjqci.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gdqpcwhel.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/glwitljbs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gxqaoijil.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gwxoivdiw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gnxxeduqv.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gvbctkzgt.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxtplvbvv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gxszgwecp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gyqpfvgoj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gmndoeogf.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gwxjhwiwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gnznczkvg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/ghpeennvx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gouqwmvbn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gdtqcrggh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gvibwwdkl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/ggiumjxwq.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gujbriomu.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/grhsoofnd.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gqwbphgnp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/glarnfktp.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/ggprbbwmf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gshuevvfz.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gkrzbaynn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/grjmdozgj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/giojeiape.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gecrcjqlk.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/grikgjlft.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/ggbhvkjcl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/glnbfiggy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcjybvoyu.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/glyhtafys.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gitlrhxjs.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gfdybfxxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gttvbqeze.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gelkzkqhg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/goveimnju.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gvpubvloh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gzhypqcde.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gmzdsrsqp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gvaaiamzt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gbjhfihav.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/ghdonstkn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gulmtyswc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gpxzdjugt.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gvdobexnt.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gmeqjaurd.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gzqmigqwr.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvydjhwlh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkgalzm.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqduqamas.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/ggbxqbcpf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gtwaewpge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gtintxdez.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gxljccucc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/grmfgifcq.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gmfmalexk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gnpsedois.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/ghcpoibce.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gqxyderey.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/ggrjunvca.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/guhayryqs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gdbrbsfje.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gxsjtlffk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gvfoeofvu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gyfhavhyl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gwzcvxtok.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gsxpvunex.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/ggykgktrq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gftfbtwfa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gynqcsdxk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gkveknenk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/geeuiurgi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gqjepjusk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gqokjjsrq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gjxmdzqkk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gasmyjixj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gaqjgzssj.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gsmxtpqcd.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfvjdhfzx.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbeociojg.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gzsffjwht.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gsuzhpulc.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gjcqvowux.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gcxxfpiqd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/glmkbmvob.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gmyklnrdh.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gcxtvcinq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/ghcsdgtgh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gcvsxqliz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gmtfxpanq.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gkaekurfl.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gzanmlavk.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gtsknkrly.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gbwszrpsr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gqhduckda.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gwqfjqxoh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gcgmfkidv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gitolposq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gsgrzkxlj.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gswfkxcfg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/getaggcsa.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gyjmyfwdj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gshhqxgex.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhvzxjo.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gkbyifkhk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gfvvrditc.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwllaqmxh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gbsitjqrl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gravzocna.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gxkuaxqvs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gsbobrhjm.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gpjafyfce.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gwykgaxyl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gmsutarrt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/geqwlemfk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gaxixqjrl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gyjjikaaw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gcrpfdlby.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/grzvbmvqw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gniolekwq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gxagjlxqs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/ggpfvxwrd.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gkmfwdtgk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gglidoceq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/goarwhxct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/grrfkmeea.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gtgwhozri.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/glxiwrtnb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gbqtysfow.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gtjlgryka.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gbqpfghge.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtxqdkbgm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gfhqpzjec.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gzvqvjfsp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ggqpxxacs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gsskkheff.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gqggpgpip.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glndaizpa.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gsdnvrmaa.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/guakntcph.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gqvzlerjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gupnqxgfh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gyeednykm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/guapmzlxa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gwhahxzxt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gwmcdobmm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/giumsqfkr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/guuxfngar.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gnaemvndg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/ggqnjjvwq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gebqdyvsi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gvcmtcuby.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gyigtkgkf.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gcyywnysx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/govxstmvg.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/glthfcsxw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gykirgwza.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxxkfsldz.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gdtyhlolt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gosqszlgt.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggejmylks.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gtrfdlbbq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gznanttgp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gvmhobrjp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gfjsnrqyk.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcsujttzo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gftytmbqh.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gnrcistzp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gijarlwih.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gekdvebai.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/ghhrsrxzn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gzzzrvsuq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gxteyeabe.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gwnxsjmvp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gcwteoffu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gbrbsmzor.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/ghtsminhb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/ggquxyrma.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gtakihkvz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gpeeanzke.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gcgorfykr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gtkdecxgw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gyjnbhizp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gfihtnyqr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gjpcwvzzr.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gwnefzvwa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gwquacsrl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gpwqomkel.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gnafwgmgh.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/geddzgigv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gyfposxzg.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gydsugokw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/glgdnctbr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gqesdfeyo.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gyzeuidfe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gijilaqhg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gyjgahlvc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gxvpfmqil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gxyisevax.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gqnlsbquc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/glbkfwnra.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/ginksbwqk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gxhyewgwu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gvpuoiovr.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/guvrggzpk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gberyrvuo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gumioxwom.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gjmlxidfz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gzwwhhlms.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gfwhezlfc.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gnitjnmzv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/grtzbqyle.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/ghpnhirej.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/geaomuxca.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gaopykpxu.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gypxjbbmo.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gslhtnyoa.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gisabebqi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxqulonql.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gniwhxsij.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gglbxgiwr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/ghygzscle.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/grdboakpw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gduymsbwb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/grtyztzik.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/glvqbqgtm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gtgyyrnox.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gbrdjyofe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gcylguhqy.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/ggdmywvfm.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gxvyavrix.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gfahmznlk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gesiedrzq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gxnxbfton.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gjkpfaamv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gqlbsyxta.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqyemedin.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/guipkacga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/grokerfwh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gzjjmnnbv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ghwgqxssa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/glnaaustn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/givxflelz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/glvmjhpar.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gdfvtqaqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gxmqnnkta.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/ghcakvzfv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gnqyineec.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gqmlroduh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gocmululf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gyzamhwjx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gmszwmdml.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gqqsxbdti.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gipjvtkmz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gblfiqrav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gbcqvtrri.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gitinchox.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbpytbqiv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjunydfqt.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gxkdsadnd.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gghznforv.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/guzebmxnk.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/glmtklfwr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gnivjczqh.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gdbzfjjev.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gumkvvkfr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaannfdzs.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gsofazsiy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvsvuocey.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glnmsenog.sHtML


<!-- 参考信息 -->