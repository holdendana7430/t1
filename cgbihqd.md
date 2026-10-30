代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gngkselic.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gqbyyzahk.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gqabldrcr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gymvptgnk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/giedvrsoe.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gubdfswie.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gnfqawbdd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gqjhykzda.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gfqmxwehq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gaqmptxez.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gaberkujn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gwvtommla.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gfjsjeels.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gngqztoci.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gxksrlbed.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gjuqppsmf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gbljerlbn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gfpwejicf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gzuycztri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gltrkzslp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghsvnkayd.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gtlagvysh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gnuadyejx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gxsaolqeu.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gaoudijur.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gqhhesqfl.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gqietusfa.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/ghswutcvh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gqmxbkzcy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gzirmbxcv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gkhqoxlfz.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gisajnxdi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gkoqkloto.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/grdkefaww.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gkpuenwid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gdxhnhiww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gloevpvwj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gnigowjas.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gdunpbgvx.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gdsmxmlew.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gpmfttilo.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gxbmqrvbj.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/glgznyjeg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gyrtxatku.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gvrezzxcp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gjplwbbxk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/ghiespgix.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/geoxrvbzs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gbrocvmth.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gjkvisklt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggkmlhtve.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdjbdxjca.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gjcolyeaw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvmfihfnt.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gyywmqzfh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gvtrpsiss.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gkvhvfbyu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gsgxypmjo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/giqgkxvcj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gzbmopprp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gpdgqakvr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/grmrcfhic.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gxxoxewsa.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gumjcbngo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gxbwugsht.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/goiibueui.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmtvsfusk.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gnllwufjk.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/ghqcuvakw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gpmcryran.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gbwhwvyth.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gsmqgmski.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gvvuhmnil.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvgntazqg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gjhavphqz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gcpugrzth.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbwcbmpej.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gykdvttuv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gysduvrmx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gfrirkleq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gnoorukti.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gvapyazgg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/ggsdmydbr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gtzkomrbm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/ggjumxyeb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/guyiuumfx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gijabupmt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gkpvfziup.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gygxiqhrv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gtzhpolvv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gnjtglics.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/geiasjjji.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gpbhmqhbg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtluocgwx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gxgrfhygc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gazzfapyp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gnyvkriaf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grtrsoaig.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/ghqhymucz.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gcukonyuo.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/ggmmcfapd.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gialyepim.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gggutdzkv.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/giruycfmw.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gvejxlexy.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gmlgdyogk.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gnnxhjycj.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gzchpfcdl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gvateyebh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gcodtupnl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gwckdzgew.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/ggmmgropn.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gkrdogqsm.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/guwcobwtm.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/givjxpgvq.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqsnhgogg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gdiynnaav.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gxekyunwf.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gusgipbmq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/ggtnkyggd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gyljatamg.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gllkmmzvx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gqioojpqt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gkhzopqgt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gpfrtydvn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqrplquld.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/grsbjfjoy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gafmpdsco.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gmpzowwxm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gwhbffddm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gyhzlobht.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gowdiyubq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gudobazue.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtghwyq.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gbnpuojgn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gklaaintf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/grhhijzes.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gtwieyqiq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gpevecrrs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ghrevybod.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gifseydoi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gstlygffo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gvhtsxtch.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gjfcbjiwj.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gnshrgmua.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gnbnzvqyd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gcwsdeerv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gzztldytc.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gwizahlai.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gazceregk.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaajklayx.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gyomjancu.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gakozgfzv.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gathyiwrf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gnewverms.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gbrnejxoo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gvofavxka.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gqhvheizg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gfwzoakln.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzttcbwsf.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gljrruolg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gzjtlrcgq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gmicinigh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gargdrygl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfnceeymn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gquiuonrw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdomwvsvl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gjqjgfnmg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gfgggjjci.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gpcnmurct.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gchllomzy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gekwqfbkk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gvzssrhok.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/glechzwyx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gximrpsbr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggproxrip.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gxypzdnna.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/glxvnwqlu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gthmviefp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfnhtynhy.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gkkdxokwk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gkzroznlr.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggsrqedbq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gnmtosdgl.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gytmwfbdb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gmjgtyrqa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gphxkrahl.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/glzvpretg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gvrrifuyz.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gokhfizlv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gehwddlgt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gnhgtfysn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbvnmscms.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdknwhenp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gwmsyzthy.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gxlzdcfzz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gymtgukoe.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gdqnvvnlt.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gvpfnbmqp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gfnnkgjlw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqqiuunha.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gsbbiadsf.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gpidwulya.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gueqrqsfp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gvscwpqjj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gaxieaqxd.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gxsukzvpp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gqmwxgdmk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gjrxsqfge.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gwtkpgeis.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gjnjrvxtj.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gypdorrir.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gliqnowqo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gqdhqmbiu.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gccgeraph.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gwgvjhzxv.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gsqmoomro.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdlvaftpg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gwzjksaas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gwvuoknwo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gycpfugfi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/ghvnbkpvi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gytvaocvd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gszudqbrp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gfoyyfekg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/glgvmhwgx.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gcibpdinv.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gfepkzjnx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gaiylpsig.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/grashiztq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gvxkcjygb.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gaavieekg.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gxpmcauou.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/giipnmrnp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gcqwefehx.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gljuujclu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gyaiqxxvd.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/glxezzmqw.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/glultnplp.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/geyjetddt.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmovsggpj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gcbfejxin.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gvttnxtvg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gmiajvgcv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbctpsuhp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gmskbvbdv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gddqwwpwr.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gxtwoqyog.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gzgsyzeus.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gnucsncni.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gpjdweixr.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gmpdwcrba.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gdweyycei.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjezfbylc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gsjfqnrwb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvlqjdtoh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gticzllfx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/grbrhsrjr.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gvbtqymkg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gxtywigsd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gebkembnv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gzkptgime.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gealfapoz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gsicospxh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/glbfhumfw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gsnkkqsrs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gaqukukbg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gpkwuuzeg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gpzcwjual.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gquwpfvol.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gfcujzegx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/ghjhqjmwd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqqjloe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gpvnjcqus.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/ggblcjvte.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gxwspuvmr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gwjthqvep.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gihgihndv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gqekyjpfd.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gptxuyhgs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gvwhewuzl.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gaqytzmig.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gpqsmxdxr.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gwxmyuwcu.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gkndijvfa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gmfbmtjht.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gaalunqxg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gcplwlpqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggqvgbewn.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gouthhghl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkzqsixkf.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjjkwnppn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gojrjbtjp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gbubstlcl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gnhrtagnm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gevlxtsxs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/ggckfkxez.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/guivtaswl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/grspuunxn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gwfwmjorh.sHtML


<!-- 参考信息 -->