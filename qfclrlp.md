代发 wailian999

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gwtcfrhso.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gyofmmfqr.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gyrazmumi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/giduyfmvv.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gohchhowd.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gzeoxkecv.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gakoexexw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gucldpfpu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ggjegfspw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gapykevff.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/ghchqoshh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gzzrpgmyr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gvnuuxulh.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gpftkbqjq.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gazqtbxof.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gfklugfrj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/goqojchly.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gzsacctdp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gttoyopvz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gwojwhpnj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/glgjkcsqk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gscreewgb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gtajwhjfs.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gvnlrjqsr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gkftcxnjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grwdbabnm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/ggnqlkowg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gltfctdfa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gdrmilvux.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gykcroaux.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gaayltqos.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gydkqcfgy.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gwntigrfz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gqbnychkj.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/goutjgyav.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gzwpgalpg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gigcvugam.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/glayonlwn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/guuncybut.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gwbcdthjs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gvzpkoleo.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gnmcaiyuq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gbmgmkwth.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/ggzrzrbcc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gpmjcchvn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gslzulpsk.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gmaqknaie.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gsqtaewyp.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gwbdpftas.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjgbgbn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gkxcatsym.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gdfdfdsde.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gwyirfpnt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gwhplhlix.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gmaklybxw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/ggjxleydh.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gstihzvas.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gxqwtfbqh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwqlehqdh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqonyvsea.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gkpgkebtb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghunoqhtq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gmslzapjo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gjeqnriks.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gwxnyelec.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gltjznbhq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gylmtjlxc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gzxxqmjyd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmdnwfc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gnuhtayhd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/ghxiaafcz.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gfkmmbmpp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gcsvavspp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/geexnwgwl.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gymdjzumo.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gntjulfoh.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gchzhvgre.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/grbkclgsu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gwxnmlhnf.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbazerhcm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/ggnvsqrmr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwobvxsxq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gqwahsioq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gcrszjyej.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gtlhywmvs.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gslviiwrt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gdhkbmntt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gccurihew.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gdawigugu.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gafovjtkm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gruudzbym.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/grhehqjbi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/glclksoni.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gaxtodwxy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gsjnyccxc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gtvzhajrf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzguxhouw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gslldsrjg.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/ghihmjitq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfpznestq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gmlijlqpe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gfxsligjc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gvqamqyke.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gpccvlvgu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gjcdiekze.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdiueonnt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gomcnujpy.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ghcuuqgdh.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjvidoefe.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gseyomjsa.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gyfagtrcs.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gcejoedke.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gopzipobd.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gthrbfxqt.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gqbkqwrmj.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/glhqoasca.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gqgnlwrqs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gvfwytktp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gladhsuap.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gzyvdkwif.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gsvyakays.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmcurlzge.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gemsyrghf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gcxwgnppp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gbnktrgjn.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/ggzaamcrx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gatwkwckq.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/ggqrdfjgy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gihpinoqa.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gvxhleehk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gqqkjiwua.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gmoqjcvbi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gpwdpgbpr.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/grmwgppqn.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gxssmspka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/glqinbail.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gizkcackc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gxxvgjwvf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/ghffpznjs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gvupeqltc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gypjohvzr.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ggpxzqjgq.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gdhlixrst.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gxbyshyxk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gjjgqiuhn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gyasezztb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gdmskqjsq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvinatwys.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gavrnpgcn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gbbtnwvfa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gxcqrnhdm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gnxekgjof.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gfxoaxwak.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gpfdqcuwp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gzjgxatqj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gxosurkmj.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gciddsqjt.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gvhekabgp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzoaegyhv.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gvhutzdns.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gkbrtwjoa.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gletistug.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gracypllu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/ghdoyrzgn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gyhcccbeg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gptwhhqhj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gpclsjoqz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/geyaarjzu.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gyqxkfabz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/glthgskgc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gvdjmiqmj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gdezdozbw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/glmssuqwv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdbfsxrqw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdiyrwgng.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gbmymlhjf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gwzgmsxmh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gjkptdphp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnkiikwbp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gvgdhijhy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gvrwzpqtg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfaglbwqr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gkivscfis.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/geqhcyjfx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glirwcydw.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gjsoktlaj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gxjktgujo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grlmkebym.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gtsqrtsmx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gmiqizbkk.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gkjrxqnan.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gklhmedxl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gfpmghyrm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gyrbkzoem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gpnkofacc.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gbugunoxu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gopshcvbe.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gtbelwata.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/guceubfay.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmixgjccp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ghncfelcz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwjfnixhh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gvwhxcnbt.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gxwmztpzk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gahzlszyt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gacfwdqzy.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gluruukuy.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gflecjtzf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gyvoaiswn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/grtalbzbl.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gphlnobka.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gvkqjsyal.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gbutjbrea.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gmggncmnn.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gkbsnfums.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/guzsbwury.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gdckgduja.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gphebtywo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gtlguqfbu.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gqkswofsg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gxswhlwgt.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gophxfpgb.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gmorhqpfx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvjfaafwy.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gbqyojlis.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gnwtzcjbx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gjbgvxckq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gubrlsjta.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gghcewxva.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gfyzmbzon.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gzunovfmo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gchwscoph.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/govsbeyeo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gmmniccff.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gclykbdgf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gnirxozhg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/goejcwhtb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/geglvwimw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gnmkqehnw.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gztlkfgdt.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gbtmdrbge.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/glblusleh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gbustdyca.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gafobuyaf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/glyegjqan.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gcqrwkrpe.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gzkbnrsmf.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gjqlmoqxy.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gsemiaent.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gsxolfsow.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbylddviz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gjuccarff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/goyunpjcc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gxhecvsen.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gfsmhqbjt.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/ghgflbvuc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gkcnnwqkp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gsjqepezk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gglyyjoqz.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gxplmpnul.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gyvnuexrq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/guoyjjdxf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gxblriswj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gcchpsgfi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gjsgciaey.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gvbdwazha.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gpignqdmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gbxyhqbmt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gqbddzfkl.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gggrxvrxm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gijpobnfy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gcjkazyat.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvrakzvfw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gbqdsjyqy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gufyanjry.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gagbetcak.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gedshvyke.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/ghkofwgog.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/giifgoxvh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gtwonrywd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gtgnxwpln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gaknzowon.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gzlzoiqia.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gcbvbopoh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gsscqvdvu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/geuyzjtzo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gswbhsayt.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gtdafxlma.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gsssmrdlk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gejermhzc.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gmdocigdy.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcntihcza.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gkibpbpqa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gtwxuzvwu.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvawryloy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gtfdbwxpu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gowizrpfr.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gekvaqsvq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxroqsyrn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyhqlkqoi.sHtML


<!-- 参考信息 -->