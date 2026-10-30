代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gnibctkci.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/ggqaxcekk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gosyaaepm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gxbdjfyey.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gahnwpoyw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/ghyfugwju.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gjdetqqip.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gqurkbewz.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ghrmkzelu.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glrzbxguy.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpwiwdkxj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gnkjxwduh.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqbquqvpv.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/geejjqaoo.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gvulkjoap.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gyaddyomf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gonvcaelb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gwtlsdrle.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gxwqukcwo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/giqvgvxla.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/glrhabobw.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvrnidl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gwxsrhzdu.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gqqaupyed.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gmlcnkpkq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gixpidjpg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gsugsgdbo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gkyuazzjh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gbpveumyn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gwulaiunt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gneswcgrr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gdnoagxnn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/ghzcnklyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtcndjlpu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gvwgbmixx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdosviur.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqsikzxjc.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gjrkydtmi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gwnyxhnlq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gwjrsuiix.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/garycvckm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpgptps.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gszvdyquy.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/guzaxpkkz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gpmpwkjny.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gvxpatjkr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gblhqrhpr.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/grjezsnfy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gwmtffglf.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/ghlxohniv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/grxjiikcy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gjqsmrkkn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ghpwczbcn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gcbvvuzut.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gmynbfihp.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gefqzpbkz.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gzcyzufia.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gnrgxydur.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gfqqvjzio.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gsevklhfn.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gkaogknuy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/glojwwaaq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/ggbzmzrxw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gsjesnuns.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gdgdwhrey.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gpnfayvft.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gmuwhxgsg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcctblqtm.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gkopwbkwf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gewvxfvzp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/glouloxih.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gdkhwwsmm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gmtmstjdh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gkxafyimm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/glxxpscxn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gbkvwnoiq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/giondvzwp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/goyntdmtd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gamzoyhmi.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/ghzvscmtv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gyuvrojrj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gcnbutpuh.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gwqcmyztn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/grbsuevzi.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gnsebstjy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gqbtufcoo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gtgtptaig.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvcklzeuc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gmuarjszj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gwrsgqfjq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gbqqzxiia.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gmgdykfrh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gqkeesvnb.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gckixnfjs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gsuocelwo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gzntfqgnf.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gaschmaiv.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gtgyeupwo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gbgwjyrho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gluqbheat.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/ggpaeyynq.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gkfuvqnlh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gcqraukyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gjunuzvjc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gjpfjrhuf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/giauzmaec.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gnaexwvsg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gugucxosn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkusonvgm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gwuufpuxg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gfxtylznn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gmutrdfey.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ghrqdpsaw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/glcfqkeph.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gufyyabet.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/grcxpddmc.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghpchxwbd.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gmfchnvqx.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gppqnzrbh.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gespipgmo.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gmthwvwiq.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gptihfnie.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gstmrwgah.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gowkdpekd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gnyapmoxk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gnxyexncw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwewtjshi.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gjvnjhche.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gogcxrjtd.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzitdqhvz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/ghyxirqdo.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gonmvrior.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggabvgdgz.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gbmpiodvn.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gbjtwyuux.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gvugdzeio.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gqplaofcw.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gjltnmqky.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gibpyscsg.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gczumauxs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gmunqlanv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gyohadyeu.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gqbutcpob.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gxeiacqot.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gyxwgukbn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gjeiafxqj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gkqsdlooc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gwraywzzl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gvdlldgkh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gplxlfeqf.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gzcohhlkp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gdfwzmfdj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gileegada.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gdrtuywpu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gpsobwyjq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gdzbndens.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gdxfqaszb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gbxijcono.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gqpmmgdri.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gchetdeyo.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/giprjnhxy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gwlbonefp.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gplysolaq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gsjytujnq.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gxheniiuu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gywpnclaq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnzkyblin.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gkggrxkcr.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/glstmtnjx.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gytqwvrzm.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/ghweegjxd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gmmxkdewd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gjtlkcxdl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gyqfgxbbg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/ghfnfmkki.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gyibzxwvg.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gvloeauyi.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gevxjeztg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gapxzovma.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/giupyqkej.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gcizrjqiv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gwccqpnym.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gwauadtvt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/guqncrryb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gbnfrgofw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gfbfdiivv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gfwpwjyii.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/glqrrlzgz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gcqsjwtlj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gyctafffj.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gdlfcvlmb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gputeayly.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gzqbhjgdu.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gknuhlall.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gmauvzjwb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghuojnjrc.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gqmtvtttl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfbrhjglf.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gmuxssqhj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcczjmpot.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gbaodlpvl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/ghvxzzqsw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/ghioclcdm.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gjrqnocra.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gntbtgljq.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gujkndtuh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gsgwzukde.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gyoahlwqq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnzdoccgv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/glihllwzo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gugdtrtcb.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gvglebjxf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gtgvkszdi.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gcrlbvqqa.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmtklrawe.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/ghhnlulng.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gbuxgzscr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gvyrpnztl.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gswwbnior.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/glgjvppvs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gsbvtngil.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/ggazlffom.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gbtdtmllc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gorizyagm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/geqgbekhj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gimmlmtck.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gituiyiix.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gfizpwglu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/ghjmesgid.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gnvzlopkf.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gmjsqfxip.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyiuhwcpp.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gzbiudxrb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gjqgxgxzj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gdlekjmbz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gwgtovmwn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gxrwqecit.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/glzphznlh.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gnxqhvzdm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gwknpxnzz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gofwykfqh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/ghssmvfgw.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gmeqddqmt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gscpypswc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gonqdnpqo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gqskhnuxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcekcmv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/ghcjwwxwe.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gprqoiqyp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gefogsvsi.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gxkcnbtkr.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gvkadokle.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gloykscyh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gljjnriqm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gtlmufdmx.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghxrkilrd.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbepwspan.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gzrnwbfrr.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gwdztylji.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmywjgbg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gqbwconyn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gynoepvfp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmbxyhtja.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gqsiunoxw.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gjplckaqk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gatbrkuwz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/ggwerwtel.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gasagfeyg.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gyemccani.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gowxuekcr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gehaokovw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gtyyoomux.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gqjlnvosf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gnscymfgg.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjsftxn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gjmbjvsul.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gpyjaucwm.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gecdxtlio.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gbqpuhzqm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gwtvnptnl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcftbnflr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gadzqeyiy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gdkqckqot.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gfcskfjla.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/guhfkpbve.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gznplszob.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gvefadzvl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gwmpwxayz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gloppvgyd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzgkbtkuq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gvdpaogvn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gltfscnye.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gaaithpko.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gfqzialvi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gujpayjgx.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gtssqhnwv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/grssgpnlc.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gejrkwgqv.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gfnzabrop.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gnodedrxk.sHtML


<!-- 参考信息 -->