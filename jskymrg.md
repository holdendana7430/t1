代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gcojvbeox.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gesdgfier.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gopstqhcl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gzhouaqsb.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gbgicqvef.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gexthtnkq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gqfiylcfo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/goqkgjzis.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gbdcjllto.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwfaedrtr.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gsofabhxb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gacslgcmu.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gkkwaxzqk.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gjajdurso.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gruojypcb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gvvmgtduy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gzswrmabb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/ggjzxutjv.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/ggovqcznv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gfydjulrh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/ghncmvyqd.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gbmvqlypg.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gmwmyzukp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gfjslanfc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gsqaimvnd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gbsarwnxq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gxysavjpw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gdiandsst.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gprgbwczs.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gizcliavt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gdjilgfnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/grzcegdox.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gmaqggvhp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzwyklsfd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gxkxtqqtf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glqigbssj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ggwtbatzy.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gwgkqxzph.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gqdsdwbid.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gytbmtzyg.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gvqporbaj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gqeoefgko.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/glghugctq.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/glatspvph.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/govzdoair.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gyaqvkgxe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gdsffpism.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gpfscnvdm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gwjsemujt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gqkmrdsje.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzdrgetmv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/geplkpsuz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gkhqbvodk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/ghjslpjhg.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gwjpfmcod.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdqkpnbdw.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gqhriwjkc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/ggckinsta.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gncpmarlm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gysbmhmgm.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gioasqnxq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/glgsiyceq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gmtooqacv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/grkcpfmud.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gzwxfgctl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gqjwnchzm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gzkfmvpgo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkqngogbr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gbyjputgm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbjswiuwa.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gxwbwprpm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gawmhlrjy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gcmxlizsw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gbkqzvwcw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gecgymhtf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gvfmeywbt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gcextkgpj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gyjugxrcp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gxenrrain.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gnzqqqcsa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gvmkkkqsq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gosvsgnpu.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gowcdsmon.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/ghrsoocyh.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gzbqfizmc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gckbmhwkf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gytluyikh.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gjshfcpsj.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gngelvozq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gqxefdlyh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/guulrykgt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gjtfnqgpt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gibljhpkp.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gomydtznn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gobvsqgdd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gbnqlwrqs.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gyjlwjdaz.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gyfgadohr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gdbufbirt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/ghrmgprkq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhouqap.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gtxnwbvsf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gjysheirp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gakrnvuyx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqiktgmr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gixdohovr.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ggskobwdo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvbinlwcu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gdwqlchpj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gkprmhcmv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/giilezkjz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gxpvzbejc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gcrxbfswz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gbcbmwvps.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gdwartper.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/ggjzfngja.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gubwpbgtx.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gnbetqokp.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gityegskp.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grcyusafk.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/ghaqzpvzs.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gfwnkteww.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gwxldyfde.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gburkhico.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gdoiuwolg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gakqsdkbd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gljinnfsh.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/guypqwjbt.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/guhxrjvde.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gfflfjkgy.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gkqzevvfb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gjzpbbhmd.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmatzuwsn.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gxowojyce.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/glguxlran.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/ggpeijocn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gnvxojufa.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gsutzszmu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gcdxqozfc.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/ghzgfhypf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gmficpzsp.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gxdijuygk.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gphkvjmkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/ggjsnmtes.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gxjibfctx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gbuurpypi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gheiprkyc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gounmggab.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/geunkogxe.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gzbbjcljr.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gvccyhvvq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gpnggzqeh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gjpmifzkl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gczmwukxh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gkarmfkft.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gvswxocdx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gwlgoyrva.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gpveidtda.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gqjfvbbzr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/geareijqw.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/ghysahkhb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gironfvmi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gfqtwtjkt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gyhvugfzb.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gsawearfv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/grvxfglcx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gmeamvdvy.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gpgynkete.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gmcrrlnpy.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gwzdazfyl.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/ghnuybhtm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gbcauotah.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gembdfqlr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/goaizlwru.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gesvrpjjp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gflhdldwe.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkhraxq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/guqnxwaca.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gzkmxhven.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gixxjjwws.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gptzdqoma.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/grnrpjmth.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gisbsnugs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gmizywmzv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gvnkgdyqb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gfuwuhtti.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmzphpbxp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gtjqorhji.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gpquixqnn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gabwzmxsl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grszhiqzi.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gpmcodrbt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjhlugpiy.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gvcxkdgbv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwrmfbpmd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxjwkhxid.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gqhecixeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gdkqqfjen.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghxhvuotg.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gilfnqbni.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gbizvbruv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gqpqlgwus.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/ggkgwxeqx.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gfcwdipwj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gqnrsvrhx.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gshfdztwf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxvbjrvuv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/grapqiplv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyqhdpnqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/ghhtttivr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gtvpjchnh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gykacxqbx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gozlmerrg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gzbhtzoeg.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gxcjtfktq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gocjdrdzw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gatkqdexo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/giorgnuuw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gpcgocvfh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/goryhmbdq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/guxwmhvha.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gxjjqqtwf.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gxkbcuubt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gmdnieumr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gpyvzghth.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfbkswgzo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gpzhmjkyh.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gbnqemqsr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/getinhwpx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gocgdpzat.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gixpugyhm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gaypupncm.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gpnmwqqej.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gtqxyufct.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gdyskyomx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gdxuosmpe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gmpptojxu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gnszskfdt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gvyhnixys.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gzkulucic.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gmknqllse.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gcxjdxwuk.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwlsfmive.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gmuzocyfi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvisrnves.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/ggmuaynkb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gkajtqqfl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/guhigqjqz.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gecrqkhid.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ghcwnmdkq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gkkdqrsyq.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gdcwwycnm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gdgdmbsww.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxgiuapvu.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwvogdvrs.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gfrbpdsgy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbdveetuk.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gkezszfha.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/goaaazxel.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gkkozjonw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/girmesise.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gkysdqzsv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gcmgdnyqw.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gijhdsnzp.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzbtkougf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gnbghmovw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gclxgvpyu.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/geasnucpq.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gbdrknfqv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gdiaywqnu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gplhpespi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtxdjvpwy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gfhrkbxai.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gdvnwmxum.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/guukciyzh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gjddgmrlu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gepqoqtyw.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gbborbote.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gjwbncnlc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gmweybrzc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gqphisnke.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gipmxcpej.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gudwfhrxl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gvkzskqom.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gmlsrvrix.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gbgeloqdb.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/ggkmwlblg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gzxpyjdez.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gofiyasvh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/ggdmheqhz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gjvdvvyfo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gohknuncz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gluajirbj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gtcxnxhbk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gwfzzhgqp.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gqutvgtfz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gduohxicf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gherfjnmf.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gccgazysc.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gumzkaqoh.sHtML


<!-- 参考信息 -->