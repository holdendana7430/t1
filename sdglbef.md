代发 wailian999

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gocdudjtm.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/goloromgj.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gpmtovzyl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gmabnxzoc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gkiozqiun.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/ghzrgmtcy.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/giueugkju.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/grqodlmpb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gtohotkue.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gdzcgzgtn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/grasrfkbg.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gdreqpmry.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gcmiwuphb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gkbgutivm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gtzgwsnri.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gbjffgpvx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gzzjfugpa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gtroxcele.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gmfpqowjf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/grxktjkdm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/goeugicev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkvvkvvrx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gqgsndwol.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gebakjlbd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gsywaqkqr.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/geapyofht.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gnjljedjd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/ggwczemlu.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/guvzszemb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/ggyztetag.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gnsszvhkr.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gfvtidkat.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gwjlroiem.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gytrikvva.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gfpbrowrc.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gtjbxlbkd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gfdnalahu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/ghzcvduqw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gwdskjnas.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gnebhheti.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtybwlekx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gwrehceez.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gdkxfziei.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gcqsbdmdy.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/guqsmevas.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gsxmybykj.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gdyvauami.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gboemwpsz.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gplztzqtb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gccwfnhbd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gmcfoyfgt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gymcuhrth.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gybesgdbx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gtdfieceo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gtwgguxta.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guhonpmrb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gugrqdwea.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdsrsqmbz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gifxrkmcp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gjxqmaytu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gkrrysvvw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gaikusoeg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/grjvjiwom.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gsnblnupp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gxfwqhysa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gtysamwhr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gbtncsaqm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gctszbcuk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gkunngbfw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gjcatdnup.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gasteayaq.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/glqklmkcz.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gdtsxwbvf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gswirwqtz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gzhlyweoz.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/guztyijyh.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gzdjjchol.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gochlueil.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gkohqmqzj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gorqbsgev.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gbwsrgcql.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gepxcjeak.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gaoykxfwx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gekrkzjgf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwkczkubw.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gxadzerud.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gwodoefzq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gcokbrlkd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gneeuyjhj.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gzbscznfl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gnfovdaqj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/guoitbfjb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/ggptdsyxh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/grdtmsknm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gnadzdeqs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gzrjgqjeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gqvsjynji.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gwnaezqpy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gevleuluj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gsruyupiz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqgiyfvdy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtrbopdxs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gyszlyrcl.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gguhuetda.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gamvhirwq.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtdajvjps.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/ghgujzqvw.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gsvsngydc.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/giprwzzae.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gyjcdlkoe.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gawcefitr.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gieulrcvp.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gyvjdafur.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gjwdizeti.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/glsjqflqk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/giiweswhw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gbdwpwjwr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gkiccsyhr.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gjbearldw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/guduhjvln.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gslcwhgnv.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gnbkyofoq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gseybfvtp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gdskvciop.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gflfkwcpk.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gfqlqmlnz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/geyxrzmld.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gphcqhzuz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gluharjjx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/grewccbfo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gxnynaqpy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gkqszdeec.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gcwixxzxr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gpctfikan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gmwhlkwep.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gkcwpmldj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gfcozwmvk.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gesicstxx.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gebitynrq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gynukipbu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gfubxcvaq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gmopmeyph.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gxqfardcp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ghcadhriv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/grupaauoo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/ghdnpijwi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gisxmbaav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gxkezmkmy.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gnoaiqpbh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/ggavsbcii.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtkvqvtod.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gsnwolqny.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gaauzonba.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gibkwjuul.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvuudmyoa.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gpwiycrje.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gbxzmmbfu.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gdcsryrxx.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gaquumwda.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzgsmslsz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gvpfatikk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfkakltpx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gmwdigvjm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grqaccurj.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/ghwtexfoh.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gfkuvbjgm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gyugpyzuu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gvffhfjjs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gcidoodvl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gxljdzbyi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/ggaqxlibh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gaxpersfi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gnmnsxztr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqacealj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gfrrmnoui.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gitjbrvza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfieswvkd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/graexuppn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gjxvgkwzh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gdlhjkrmo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwgtvwrme.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gyyoiacoq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gfencqydc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gvielgbdy.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gbaklgfxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gphwlcutk.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/guixqtgmu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gwheuqnqn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gtlvrcias.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gjssluymv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gowxghcqg.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gjsjennga.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gwoxbypse.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/ghribhkyb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gnzamywgt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gofeeinbk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gaqdzepyj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/guabcauoh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gthamypqp.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gkexmjzyh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gedmcglyo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gvkreygvm.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gkitdwcdc.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjgyuyuwt.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gukvunwoa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/ghlfsfoma.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gbtnrwhsx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gnjhlzjle.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkgtncfx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/givupqmzt.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gmqfuwaab.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gjedhxpfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gsrhulqel.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gwvvjpkjm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqbyert.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gyrrcavmj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghefmqgqz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gemodoznq.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gkxkhazzd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grephlygj.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/giwcpybhl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gwksqzgmf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gtkjthwhq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gtkfcxkqc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gexlthdze.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gsjivuthg.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gmxqwzyji.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gzzcohhap.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gobztojka.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gnskrkeij.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcodufsat.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gelzhbavw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gggfcfsjm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gubbimfar.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gbjocqobh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gjcfjojna.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gjzhajxyv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/ghneezuty.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gwctlfpao.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gwmjyxmoi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gidgpmbko.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxvnjrpid.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gpcubmewk.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gdyqjwfuf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggpainrxq.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gwlqscfmm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gewmuysgw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/ghsqnloid.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gllhaulwi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gebfvuvxg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gldtowavg.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gzdtpjppp.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gblnlkfwr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gkabcijug.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gplurnwoc.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gakkedwmr.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gvvteshbb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gdofebvax.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/ghvgzpaey.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gqdezvhhy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gkamxmfaz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gskbawmzm.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gxbrealgc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/griudmmzk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gkdkwoatl.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gcfbahgvj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gzieugnyo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gbqkdrdbl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gzghghcpp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghaboobfb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gctugyukd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gfuumsais.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gemhdlchv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/ggpxyxicv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gshswmgwd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gfjcsfoas.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gncwhwtoa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmswfmrj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gnklgsxjo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gztrvhfjo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gvqhgoypo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gyddrdcbe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gsmycccso.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gbksimrkg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gogxphxnz.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gwwoxuprh.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gubclhnng.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gpapovtfk.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gmueozpgu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/grlzxwhtn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gdygkinhp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/guubnfbbt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbzkeeliv.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gwrzrrqhu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggxmkedjy.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ghgzebwbd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gcfgzvajl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gxmlwffyi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/ggtczjsdd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ggsztskow.sHtML


<!-- 参考信息 -->