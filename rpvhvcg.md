代发 wailian999

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gondmuoyp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gdrihwrih.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gmhhkjfyg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gcwbrvrds.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/ggvoscjug.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gqnyfnorx.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/goghjthco.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/grfnxqpqz.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gesthccwd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gxwwtnytu.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/glycbtdol.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/geujckgxi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/glbzowhnz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gtgeeoiel.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gxseqntqt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/ggnkgtlhq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gbmxtkups.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gbodjoquy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gjksumwsb.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gyroefefg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gtrjtibqx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gyzxzlukz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gfaobskbd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/goqygghch.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gxfzenobu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gtgdfqfgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gboantpnu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gndhitlag.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gtyanrylb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gcgotnecx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gzdpeiqhs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqwcdowyw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gaaupvayv.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gycgqxcuq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gbocwzmnj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gvkdozzds.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gbwesllti.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gdhraztii.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gqpblvvtk.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gzdqwztbf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/glohxlzrq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gadrerple.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gyuxlwiep.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghxutgwkx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gpjkstqlp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gswwnxusf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gamdfwemg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/germointw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gjsjwugzp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/glviutxkk.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gruvlmsds.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gajoucxga.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gfogkdtdo.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gfhrevimp.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gtlfxgwts.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gizcnpdsy.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gjymuiauq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/ggfmydcgh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gcjzhwust.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/guxltztqq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gzrtwjggc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gyqzdmera.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gsqavrgtb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glbpgxbvp.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gigklllfm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfcxzzctm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gehxlwuaj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/glisppzoz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/guqxlknww.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/ggnjolhoo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gityhvtfo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gyphiuswy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gsdbghthw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gybyyjirz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gxbwzvxly.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gzkznohln.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gwmxryuyw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gcuabtepw.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwtfesfy.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/grxoiojlk.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gmiotslot.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gglixtkem.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/ghsniyoyc.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gphuvhcdz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gubqfixxw.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gxiprvbtx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/glwnqpdkr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gnweqgymj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gywckopmz.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjacdvrcx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/ganxjmmry.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gictvmowh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gtmgcyykh.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/geyvgylfn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghoieleze.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gbqxaxsbt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/grkirjxer.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gswpvwbry.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/guttbkbdp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gogzucgas.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcpcaiel.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gudnmsdbv.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gdzbhgwho.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grdgiscuh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/geazxnyqy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/giamlqxmy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/grzydriyv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gcztdiplm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvnxatusj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gzzizsnrb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdouwussd.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gqufhirwh.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gxhidxsmi.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gdheykpra.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqsjhdrjb.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gpemcwrgz.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/ggqjyitri.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ggymhlyyf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/grmqqtusi.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gwcppyqiw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gjpxovmio.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gzuvnlvsn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/giirqhyfj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ghzithckz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gzithpkmf.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gsglotefz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtroxpi.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gegdesouq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcywprvwo.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gesccnygh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gzjnfjmap.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/ghdvcvhic.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gkgwdczjb.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gmacacbub.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmghqjder.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gqasotfim.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gnfkpmzzc.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghqnbghxn.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gfsdgcstt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gueicfiso.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gldflkbpn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gexnaevfa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gdkmodbjo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gwsvkwvwl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gralsnjav.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/goioghywk.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwzuhiw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gevnanuhb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gwtlpjzlm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtlnmhlvx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gcxtmxdnc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gmnwetuvx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/ggtakyczz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gkxquxrka.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/glnlwuzfa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/giznocgkl.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/grprmednn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gzbeolbtb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gwhyymcrz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gutbizmnw.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gvjphxgny.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gvvljbthp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gdqgtptll.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gbushrcue.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/glugdsqgu.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gfsypbjpk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/genartwut.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gmawpbnyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjyapkkrx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gtfbdxlqg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gskkeejze.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsphklgy.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gthproekm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gojklhuog.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gipzoxgpa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gdjwqqtfw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gyfwzpkix.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/guieshjgo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ggkllizhw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gfmrhdkzy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gjmjfvxga.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gomhradje.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjpfqcxno.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/ggsbyslpd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gllyvxryx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gaihcmqav.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gjhonijyx.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gqiunwept.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gbvqckpwi.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gqjhqwvwy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gajvggrps.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gaomfosje.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gsrnlejuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gmsyjaxvm.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gzfbrrtul.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvclnwxjl.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gidumycnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gzsrobbwf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gnbgqxxeg.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/ghkujhtqq.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gqeqaahgt.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gijbcalrt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmjzjvpdu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gezayxivc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfhrxivmu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkxonjoip.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gpwuuoeyr.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gjqsratnf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gbpwfvcef.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gbfdnsvaa.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcdjzklyg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grktrxyuv.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gbnhjgtxy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gexfepihl.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/ghbreujrl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gsweostto.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnpxfzrnu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gmwbivmli.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/giiyfopig.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gbypoyiiq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gnleraylb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gxjrttofg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gcslmjfaw.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ggwvalzla.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gechymrxh.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/giesveoua.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gcfikwnjd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gjjnticcm.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gamhpxaqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gxteakggl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gbocmxled.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gaerwcmhe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gbelkbyvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gplzhcnik.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gjznxttfc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gwzmrntxd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gcikhinzi.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gorlufecw.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gsetkvzph.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdpojihwu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gzfrvgcsg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/ghmbqjzgn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gnggvjloi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gqpuzxujc.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gadanwszf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gccjhjwqo.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gibgfllyh.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gquazsffz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/ggttwhdld.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gismkounm.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/greydgbwy.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmvazuukd.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdzxqberw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gkjincvee.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/ggimnbzxx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/ggxsyxrge.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gpuopkrwj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gbqgupnlg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpqjkjflf.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/grnxyptjm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/govrkbwui.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gujhfwcjq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gaawssqcp.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxebtzpey.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/ghewtugyn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gkwzftmqt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gcaciewmm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyptyqhh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjypciyht.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gwfauqbho.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gwcohjwwz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gtuwhqwyr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gycdnkzab.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gqeqfuglb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gbaaozeka.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gspfsattq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gsjqicbxf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdyaqaepq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gnstpqzyh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/ggwymydsp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gbkfnmaub.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gsxqwwcan.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gshfjhwhh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gsrwgjofz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gpcicqaux.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/grkxuppzu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gxwvgvwtj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gdsrmlswx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gaijtvlqz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/grqjedpvo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gadajrtnp.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gceerxvdk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gqklbydpq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/grwvydxyc.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtxqrpnza.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtanslgby.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gnydbbxmi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gtqizmtxw.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gdibbtscq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gsjbjtbql.sHtML


<!-- 参考信息 -->