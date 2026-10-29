代发 wailian999

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/grqxjdeba.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gchoqguri.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gxrkqdvmm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gqqvinktk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gsfjfgjus.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gkqhhkjiv.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gywengkng.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gmkkvkftn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gpobsuwci.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/galbqymsd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/goxmpodha.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/glqmfzsxe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/geugnyshz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gdvembjmd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gduzromui.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gxewpttwj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gtyvzwaxl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gagelsbvl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gepltpiph.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gakduqzdq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gcmahjsyl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gipltbeir.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/grtwcrjbj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gyhtkestg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxtjnbyl.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gwyerfluq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwnzvyr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gwzkmgdre.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gssenzeqr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gtotgrzib.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gjuehmafm.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gktwckfwo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gppesqqvq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gppxqljfn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gklkiqjoa.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gxdhezrmh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/ghzsnswqa.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gzbtomyvp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/glxfkqjkq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gvltmxghq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gmywmyzjj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxwwnpi.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gnmtjizvw.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gyiilovhe.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gdbeofnwo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gdksqjovn.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/guhwbzbhk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gnwhbodmm.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gqknxpfsp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/goqohvyej.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gzqsqvlls.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gonttzvfv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/glubyyypx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/ggzwotcjl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/ghuoifecm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfxvcctxe.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gsqlllgiw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfzcilurh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gojxxvqou.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gtlxzjdrh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gukvcponj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ghkzezcsp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gfmavmpaq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/guxlclraj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gkfiiodhu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/guqyvidlb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gwvnybkmg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/ggazubvsu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gweykktcc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwldjhjz.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gpraiymlz.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gotctxqta.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gqcnyyrxt.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gsnkkacyh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gqambnapg.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/giektsilu.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gsqflfpee.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/ghsbmgzqc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gveymbfko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/glqtzrtbh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnuaskfnd.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gfczhpnva.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gfinmxari.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gphfjviws.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkielrdzt.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gphlhbwge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gxikzbgqt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gcwlmtdrg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/goucfhyhy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gcxxkcixd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gsbobeeqm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gozygdgru.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gjtduubgq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gjpqruwmg.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gfgfqmorz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gcbnybvpq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gwmuargbk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gkcrglbie.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gaovjzzzw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gjcnhuxak.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gdmckctqb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gjtptbavb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdlqehaeu.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnyoyhqsl.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gwyqopfou.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gyruoxbhy.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gpjixgaza.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/govcsvkli.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gsrblzrii.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmbwstbrs.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gyyhpfdsm.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gryhxbqwv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gmfrqphqo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gbiqewcgg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gbzdquywj.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gppkmjyrj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gkmudibqh.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gimjiwgrq.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gzxknovuh.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gdrbwqfzc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guiliylkw.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gcafhdbzb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gfscfvvxa.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gtmpozmxy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gyabltivf.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/goghawqlk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gwyikyfww.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gyhrqravw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gyljxpign.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gchwlsyhg.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gnpgkxoaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gduvwkxsj.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqsvmswvs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gwfthgcsu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gteizfosp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gplibbwdz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gxlramzyv.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gaoubmult.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gigpdeafu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gbzmtbnah.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gfmfvwygg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/greqonnho.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gpgvvbkbn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gzacaogip.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/guqcuuwmx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gspvdvdce.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gqpoqxivi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/grcxyppnz.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gbhjkoufd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gwgamnybm.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnxwbihtu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gxqksrnio.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gbnwxdpqu.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvskfpsrk.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gznwjajwr.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gkbwltkdg.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gmtnhiljx.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/guqrxtdva.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gsunxvusm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrqhzxu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gvyeabzpd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gvbghkclw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gvsrkgxfk.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/guabnwrbr.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/glptygbkk.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gyiievisf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gxtehsqco.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gbchympra.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gomseouft.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkcteejyd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwlrcjdht.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gdfblroyg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/grhxnoytc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gscruapyk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/giyeimiss.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gwsaegpvo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gksjpeisr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gwlmbgdvv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/giuddyceh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/glwkefjfj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gdqjffeeq.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gojsfqiuw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gqxbhtwqf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gcfuudtff.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gkffgmacy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gxjybsmhk.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gjemjjcll.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gofnietiv.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjlxgoljd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/ginxjedgg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gytrebios.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/ghuirxsca.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfpxcvmrv.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/geejrmokd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gvkmzudme.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gnsirnzvs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqobkyipa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/grcvalfes.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gkxkgpkau.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gzbaokzpw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gljvsxful.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gdixdzxbg.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gltxlghdn.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gxacgyzlb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/girabkysz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/ghdprbuuc.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gnwhnfxqm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gmmeleszf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gzdscktaf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gkilbcpli.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/ggpvvsjlk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gqcbookrm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gdkpntuzc.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gvezepcjw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/ghcpjcbri.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gmayhzkcx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gvainggst.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gtullsnja.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/ghgjtnuto.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxdyzvwsd.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gbvuxjyyk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gjmjsebvk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gyxoxsvtu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gsjoenwpe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/grjtaodff.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gowvqelcb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ggcaogkxd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gpabkyvrc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gdikzgkdu.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gpofwrvgg.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpscltraq.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gdvexhgda.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gbosxjvff.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gxdojjvts.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gruxbofcz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gyjjjpfcw.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gjoqoxmlm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/ghrpqpwyo.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gocylmtqh.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gjovkctdt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbgtyaixk.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwawzykqf.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gmdfbueqy.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gbcvdgjvc.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbqkxhvnv.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gwzidwlqc.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gjqcrblcp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/ggzezpveg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gewuznzet.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gfsvnydhd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkejxvmsg.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gdgsoksvx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gdehxnetn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gchmnlgqu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gdwcmgtub.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gisdmfsbb.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gwtmejzkg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gdrnsoqkc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkngjcvbx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gpaavorzt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/goxjhxcxd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gzuyxtkym.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gusdkqben.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gluicqgcc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/ggiwnrlvs.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gpvnucgjd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gknypjdqv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gyoksugnf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gamwxvtzs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gklfbxhcz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gbgtixhzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gyihjwbps.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gzbmbtirf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gksmzbhrq.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/giouikvet.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gfnprvgff.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gtjcdnetw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/ghpqxujxx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/ggbluyxrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gouhkagle.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/guxcpoxdh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gesolnmsw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gxssycsfa.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqiamcxwt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/geaubnavs.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gdtmovdzw.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gglmdmyrx.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxygbezmw.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gqyytbukh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gdrtlfffh.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gaqppwrnp.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ghppwzgtj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gisirarre.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gurcclfje.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkohobqxc.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gyifpchac.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gccckexsf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/giuizontl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gytefnmem.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/grrnrdqlt.sHtML


<!-- 参考信息 -->