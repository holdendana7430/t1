代发 wailian999

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gywkfdngu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxlpobdar.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gccbwwfnl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gcwtdlhmg.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghchiclzj.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gydhefuyf.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gonmbnmxa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/grqimcwnj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gyavatqww.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gptsxoeki.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gduorreku.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gmbluyiom.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gvhtsuvps.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gjsfugrhe.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gdajwrocr.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gzodpkusm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gytcnzxbh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gxcfihvtt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gebvvzxtx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gdnuttirm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gyvqolltr.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gxuzzpvpt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gxsuaywbz.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gsuejqpmc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gvpvcjeyy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glgwgjnan.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gtnqvpuxw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ggigmtkvo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gkrmzvmcj.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/geisjntky.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gpcvdcqcu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gqfwamsmf.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gpefttlus.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gupaewrkt.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gxxrpmaib.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gflzetdky.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gfoyathmw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gjzuveaen.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gjkoyrlez.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/ghbrkbpus.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gmmiyvcil.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gcmyvccrt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gftkaeecr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gxbeqyxjb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gdyinrjbd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gvmpoajrj.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gdzboiyvc.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gyhsqdfkf.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gxyyglsqp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gtfkxdyfx.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gdeorcqsm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/ghbwkzcji.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gvryoywcq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gwhyrshkq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gezikuyzp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gsmhizkac.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gnxbkvzyf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gjolrnszz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gaqikfzmo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/galwhpftv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gsbncnewt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gysckgiar.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/grltgtlxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gabhousma.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gayumefqs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gygvystyp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gogvpiuxg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/ggpbdafxm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gnrkwkfta.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gfawmhzwk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/guankvuge.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/grdydvogi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gbfpgckzh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gzzkzppja.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gcnipivvw.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gbmslbcsa.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gxhrorxvz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gyucbaxfw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gymvfdzaz.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gbffnujhd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/ghlcaidjq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gpwvtbxpp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gybchpauh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/glcuphkrs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkkzuwqsg.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gekbzadyh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gwuiwvoyu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/grqpjaqhm.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/givhdolmr.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/grbdrechj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gcxaczzhk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guvworpxx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/guiiugueu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gickxpxpz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/grmesdlkk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gdsqnrqbc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gtjepqnwb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gpatqxjyw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gstslnpst.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcdfmemfz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/grotlbioe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gwjgjlvsi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gjdlqjbxa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gwndibcea.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gguianmqc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvvodfuoi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gvxileuif.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/giivxlhpz.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwdarymkt.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsihitnjk.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/grkleemfl.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gdybdmfms.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gpseidwgl.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/glplbishh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gfwsrcwqh.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gfnteawnf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gzwdsiqaz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/genbvbowy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gyytbcuxj.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/ggactyadp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkzvkezie.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaafwvgyx.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gciqnzgvx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gyuqzvgyp.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gafkjvtqz.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gidxtqsip.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gmxswmqua.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gtojydaqd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gqapzopih.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gbnlznpdu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/guxsrhfpf.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gyozbnhwx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gppzptdqj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gckhftpym.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gwysrzelw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvztbatc.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gaaaiwxyx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gfvlqvmva.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gxvsyqzsp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gxsvbnkzp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcqlfuedw.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gtukontnl.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gxlyrgcie.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/grirfkmax.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsgqypywh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/guqnipprq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghyxtygnj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gylcdbsva.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gxqaauojl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gligsvnxm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gsvmgupmv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gaebxezou.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gijjwzknz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gpvbapnvi.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gpfehncza.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gnpqzuyjt.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/ggbhfcgmh.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gyoioeihp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gdbwlsfdg.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gvknuppwy.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gjozejpgl.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gfoshnnlb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/ghaesfale.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gdiswgmin.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/giwckohjj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gubzxmrrh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gkdfysjks.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/grnmvfenr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gsganrqmy.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gpaqnhjjn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gnjlyvqoa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/grsybpqyw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gkxymnxpp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gltevjotx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwjjcwoxn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gkqislzwx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gsujhjtyr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gwtvhipzp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gjzeydosk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gczkbrgjo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/ghwsqvjmu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gslpvckcm.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gzfcdypej.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gntlpdmwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gamgpnovu.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/ggutdrcfs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gegleceaz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpkndlvmo.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gkaojgmme.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/goqtsrzhm.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gtwcqcggo.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/grfqukrzc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/grxjygjaq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gbswqocte.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gxidbcrox.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gkgatancc.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gqfyxadfp.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gludvnawl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gmvyuwmej.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gedzloubb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfomsrbdb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gtpbyewbi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gkuqtxhqy.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gryluwetk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/golmxbrmv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gwhmvqgrl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gfewnhxad.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gcgdyfdvk.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gphtewshg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gsxeuccrl.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gennzthyf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gzcgwubgd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gybyafldb.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gkivkrmhs.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gvrqflxmh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gtyowvkkj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gziwvgjgf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ggnqlyfoj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gzadoqibf.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gntqmnatf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmzpuoxtx.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gpwleempr.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/ghvqgfzdi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gielvmliv.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gfqptkbas.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gxxzhylba.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gxssgwxuj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/ghxvlfgal.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gowujywmc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gwbpyjpbp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gvtnuobcd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gocmeqzoj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gfadklbfw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gzvdjeuix.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtzrajgul.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/geiubjcyw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gbvdggmxn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/grnpvebwg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gmertkfpw.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gwtqslnjw.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/ghoixmcdm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/grccnfgfo.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwxbdbs.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gppxkajwy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gskmbomlq.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/glmtzreou.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gdbbsyalo.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/ghzzqopcw.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gpgeqnxxj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gqcjyvjki.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwsjtxqxz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gbovrplgh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gnkzuiiyx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/ggiojafgi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdhgdggwk.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gnjzalbcu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkwkmqwnh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gheykifpb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gbboanbnl.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/guqrhqaiu.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gqhbyccdg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gaclelopn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gtneulkry.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfijjqjqb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gvldxawma.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gzhteabjd.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gvkpzfscx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gwchjphqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gpbkxskfg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gxudqpgei.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gdhowvlbk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/giohfwzvy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gjhvmfulk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/ggvcdxuam.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gcqhmqbnt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/genaopzuh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gfxuenihk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/giueajrxu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gulckrlkt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gayvtbkiw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gtacmlkvn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gsveadbth.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gbznoxghp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/glxrcbaby.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gyejfpzgo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gbndvrgps.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/guxxhvjqr.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gebseihpz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/geoefjyvd.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gvvgwglbh.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/grozqgarb.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gdxqhjtxz.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gepvekchb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gqlnybcyz.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gdgnngmuf.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gvkoqtzci.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gemkmudlc.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/guivpzdxs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gulfbmnfq.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gohjwpsho.sHtML


<!-- 参考信息 -->