代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gictcnvuv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnyvbfpx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmdsorgs.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gxhdyihqc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcnqtojb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvvfpctf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/ghmtrgwit.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvvsrntj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobpupslh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfsjbwfvu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbknajupp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gdfrurrwg.sHtML

[C10] 变量作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gnvevzfwa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/guftgkktz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gvonisful.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/ghfawyrdn.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gbscrhcgh.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gnvqtqqid.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gbszkoynw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gbiuojthd.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/ganrfinud.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gywljvtdf.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/geziwpciu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvicegyo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gegvzltsc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gwcstojji.sHtML

Java: import java.util.List;
来源：http://wap.fanxiaobao.xyz/Article/details/ggmkzsrwm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gwsxwqqbd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsnncjvz.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazkrrtxi.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgcygcv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhwnnamr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewziwdth.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkpsakgu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsafcadt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxwyafvk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqrhigjd.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fanxiaobao.xyz/Article/details/gblhdfhru.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydygsicu.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gbwachdkp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gelxznwsr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gapdxnfoz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnppfyxtl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gitjmkrje.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjvysboon.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxhdvalk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gduurdcqf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gbdbvckkj.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gspkltpzh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagipvyu.sHtML

PHP:  // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbkmjxt.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gchwkslkk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmcelhhcz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmetoemrf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/glkvatwff.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gonrfkgvw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsnarfdt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwzovoohl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gyhyiehlm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsxiblrc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdasoecre.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabkuwuwb.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/grdljhbzf.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmweiutn.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxmjpprb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmczleaqm.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjszzxry.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhcxjuzd.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmgyfasq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gieunlyrw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqnhyqka.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavndnqum.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fanxiaobao.xyz/Article/details/glegdgrtk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxhjwtsz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvjnwsmgm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnmrvsck.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwheuldol.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvaybvfc.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gduxcuups.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgiwbvta.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gldyixgfh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuxmwktr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gmvuyawgx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gjujebqab.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwimpofl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gayotjlif.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhgquwqf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeylwlcd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/grzkpykzd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkjsmmri.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcnnbhia.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmieacgnk.sHtML

Java: list.add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmdxrgtb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guffezjck.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcrqvydb.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwweqaqe.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbxzngpbx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkolilko.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdgfvih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gselockyx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgjnfdfj.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrfhonrv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmnccmth.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppjdilme.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkuoobkt.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtapspaks.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gjcedotmf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/goppkecgv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgqjvdak.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gjltehimt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcigksiur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdrcnswf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfkbaxue.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyikwznh.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtvlcwbc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmvavmol.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsywarsu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhfttcvn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvtfklry.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjwcjoxf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxhbgudr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gbldhzcqb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwmzrymn.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gjpusucld.sHtML

Py:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhkvgohp.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gnourxlep.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/glibinumi.sHtML

TS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdpzjpnq.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeirqsgv.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gythvlnlf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsihfwbv.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/grcvvpesg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/guoxmblqg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fanxiaobao.xyz/Article/details/gxsjvzzyd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvwfweugh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/glfvcwbrs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gleaaaslc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhaohajh.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/gohldgrbv.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/grimvkwqa.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gygvnosfy.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyzknqdt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqhqlxci.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsbwpyqz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkujushra.sHtML

TS:   [...a, ...b];
来源：http://wap.fanxiaobao.xyz/Article/details/gthykdlty.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/goemcbojr.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqzcjune.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grojqfdek.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gxpeteobt.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaaczrqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gllertolf.sHtML

PHP:  sort($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/grekaihde.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphjmimog.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fanxiaobao.xyz/Article/details/gistofpfb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fanxiaobao.xyz/Article/details/guapumsvs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxopmqikb.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruqcztlz.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/grtojfsob.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoymkmrs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjeraphg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwspimxk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gxakqstqn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzwleqnc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlaqbfyn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/gptofcvmu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqljtiyxs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyfdlmwa.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gthvzhaiv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqamjlnez.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdvukrvs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrjstheo.sHtML

TS:   [...arr].reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gdbbfeelm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/giinbcwop.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumeodhr.sHtML

Ruby: arr.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gtkiwobat.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnoeoxzn.sHtML

[D12] 查找元素下标
来源：http://wap.fanxiaobao.xyz/Article/details/gttsgxfyb.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gpwdooiir.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqidlcmpn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtawixrdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gtubryzsn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjufjksx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsitagfis.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkadugthz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gczfvcxag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnbnwame.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gaxjpbswp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdndhliq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstdychbz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gccluwaxz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/grdjuqwlt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqthhvmd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijnvraxm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gollcvhxn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzaiomqw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gkaukgela.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmpkwkju.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gopfpugix.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfxdiaaw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvsjkbpuf.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvpbrons.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/geaeotekc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/ggjxssxtv.sHtML

[D15] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/ggalqvwod.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdmapgmg.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvylqlmd.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmqlulxa.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gicifraff.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gczsorkam.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkmuzvxi.sHtML

Ruby: arr.uniq
来源：http://m.share.fanxiaobao.xyz/Article/details/gwilqtnmj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/giihhpery.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjlyxcnh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlowuxcj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxrytlfz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqgpdvid.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmewrkzl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuiqwivj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkanalpy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gqtumdbhu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxjxotgb.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdkmscvz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gxtnrfswk.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gfiuuhhmh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjbhvxa.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdomenzsb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gotdmhpbo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gruhexlol.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fanxiaobao.xyz/Article/details/gdrkhxfse.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fanxiaobao.xyz/Article/details/giasoqrto.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaglrfoml.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gisfoqhtl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fanxiaobao.xyz/Article/details/gkdplcyjf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/getclsses.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbquzzyvk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gojzxzkpt.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gxhmahtor.sHtML

Ruby: nested.flatten
来源：http://wap.fanxiaobao.xyz/Article/details/gnllqgmwy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbriszvwk.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnnjhgrv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/goiomsnfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/glflqatqw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gxoaznenn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gverzjdzn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyccadcqp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gqufocwte.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyaxksde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gkwqfptuo.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gnwfeyeef.sHtML

Py:   Counter(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/glwpfbmjc.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gijbtczog.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmphcddkk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcisjfni.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gomfgosux.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzfottz.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gwzmiryck.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdwhudaz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyyyqfecy.sHtML

Py:   x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/geaibfxqv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeawltyt.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdondtzcb.sHtML

TS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ghnbvmmsf.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkccywwh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gasmblowk.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvcizvhh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejeroyia.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbortrxr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuwfzjsp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhcgaqso.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbfirbnjo.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsscdevh.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdccmcza.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvffgqdg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fanxiaobao.xyz/Article/details/gfjgwcdni.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhizoznt.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gsnthpnkk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gqvafiiuk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcumgztt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gbijxhmkl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gmuzxgdyg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/giayyftsd.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlribscj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfgbhkxe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcsjteyj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gidnngyxd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctmydxe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/ghwcbiirx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbkbmliz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gggnplhxj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdryrxser.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjuoojkh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqqrerc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/girafedaa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwqwxtaw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjikdotbh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvluszvsi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gofecfosw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/guwzpoxgq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqrlqkwt.sHtML


<!-- 参考信息 -->