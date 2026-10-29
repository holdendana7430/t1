代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/glminxqdh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/grfgcgjzw.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gwqhngxeu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gshfahqpr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gswgejwxn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gmpywpvii.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gscczntjw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gdrhenhun.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gfkbimnif.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gcbjuaevl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gaebxdvaw.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gccbuysiu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gylowrczp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/ggajpbxiz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gsacttxcx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gffibniog.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gstcpbywy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gtkcpvcxi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gynmdncrr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gorzrhrng.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gpazzcojv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/ghmsdpsdn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gifjhcvfb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpmtptosy.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gqwpxqvhh.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gwsbkvfud.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqxoxfqoh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gdflcfchd.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmfsqwtkc.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gcxrsvchf.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gynqxfvea.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gwzekgbsv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gsazqfazx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gntvblwqv.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gxdbcsxji.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gxwpvzzgz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gvkyprcpw.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gnocbnnzz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gxajyvxja.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gqcmxdlea.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gqaqzznzx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gihbtwzwq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gkrrwqsat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/ghuiqjdhb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gckrogdms.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gdfczbdqx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gakrzrdil.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/guhcexruk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/giergadww.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gyqhcxnbh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gxzjbhcml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/guhcsmdsq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdkejybpk.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/glryskteu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/ghxjryhmk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gdasyjmii.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gltvcwupi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gnxzwmxxq.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/ghxjvmwkn.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/guwxajifb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gdqxbpbea.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gpfrakafg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gqjcfuofp.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxnqdwclb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gdhtzajyz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gaauljdxq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gqhjrszle.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gwxrzczpz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqqlbbqiy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gqboowixv.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gpalrpyzu.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/ggmsolwjt.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gfbtifomk.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gkvmimjsy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gaqzrddsi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/ggtgyrypz.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gzshtpxiq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gxjdiryee.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gtekjumfj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gdfezebxg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gpcdiucjm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gxqiyftom.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/goomvhuni.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gysevozuw.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gpcfpnxdy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gimrmjvdq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gzeuofrep.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gcqhhtopk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gqsnmakyn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gsdyxljcm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gaajupijn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gxyjuzrgg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gwyolkrne.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gnlpsfihp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gufkgthfi.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gtvhkttfd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gbhfciwwx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gktmjcqdf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gazffyelm.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzclhajpe.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmlqfehqs.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/ghepfwlrd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gvmxmxlkw.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gjnvhnvsg.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gnovkcthf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnasajaay.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gcmmmbkkl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gcpgzbbwh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqqrikqmg.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwmxmcerf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/ghzodvgyk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gapxssfyh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/galmlreeg.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gbpueoxca.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gonmwebfd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gyuiqxoha.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gszagmcuh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gmnjlahmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/ghpgbkuis.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gpdmzwrqo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/glwehiurt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gntoxmwac.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ggjpfyvut.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtsbddyzo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqlgmkqno.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gqufxfmww.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gjyjowuqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gzgywkfzs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glpsotcfc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/guaixgapf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gmhhjduuz.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwuyroxam.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gdelddwji.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gjxbboqdd.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gerhfmrkx.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gexklwatg.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/ghxfeereq.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkdczwsya.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gyrstqibk.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gbpgljgoe.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gputzxvwr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gulnxgsqm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gmnyhnorw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gjgxzutal.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/glrtiybmr.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gkfqhdxay.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gbgqvnwgw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gbegchvwb.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcvtpnity.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/grfxhdgzm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gxbrfrvbp.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gfjmrfsct.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gzotdxdqr.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gknkhjzvc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gohxwmojo.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gadvqdpmg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gjemtfgna.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gabowjwti.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gagwdhkdi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gnrayhumh.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gpjwcfqgq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gctrqfxvn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gqfxymumm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gqcahcyji.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gdglbxlrq.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gyikuiqcl.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/grtmrdgvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gcxbvimjh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gwfhtoyqn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpwcrjvvw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/glttmazkf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/geyokqcly.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/guwcxismq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gwizozeiq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gdasalqug.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/goigbklcb.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gwtsmmyod.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gaczugbyy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gglvpwzga.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/goildoppn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gxkboxatd.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gvficxumx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gsacxlwbg.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhocpbr.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gnjzegkjr.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gkasdnfyo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gbtrueyvp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gcrefbjhv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gbspgsqdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gxkwwadmo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/giyduwjxa.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gugykygxg.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gccuwggid.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gaugmduzn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gnxvttmqm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gganyyalt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/glrukdihj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ganuxptuk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gstveuriv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/giutgxpzm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gflcrmlwb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gjhqcllzc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdrvbcrjv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gdtpufzal.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gbgmbiyfz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gaobgvksy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/grqbkrwus.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gymlfrcex.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gejudlyts.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gbyhnvxcb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gdsdjchxs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjzqtofkd.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gbivgzqnd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/grldschwu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvbwnniwk.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gblhbjkdn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/guvcuyckk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gkdoewcxu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gmdkujiup.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gsbspmbtr.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gokorfpqe.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gbexomoao.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gblhjpfim.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grljdzdom.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gdilygjdl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gextygjti.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gtlctsoxf.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gheednjsf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/grgluzxba.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gaqehfibu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gxctfzzsk.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gofdnedut.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/geggguvps.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gtytjtcoo.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gaaudijrj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gjbugrirz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gsdjptsyh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gfbvvvndh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gcdbcazth.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gzatindhg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gaeijmadj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gfrwuaznf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gazbrpwuz.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gmzhoklmb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gektknhyo.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gkhfgwtud.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gavaxxpcj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/guqaqqpfg.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gpobtpdfu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gdveffcys.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gzxmfqveq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gwsmzzshd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gifrohxft.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gudvdousj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/glkaxawpe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gsbpbplmv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gdwkmjpit.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpgbqaata.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gltxwgmlp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gdfratywy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gucdxsunx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ghcxifdsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gmyxbedhi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gpwytyafz.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/guxbednvw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gtbmimraz.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gjpqyfkfx.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gufjwrfkw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gqyolkesm.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkkvqspao.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gaytrbyox.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gsckbhrrp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gapuzstoe.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gabqemfbz.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/goomdteed.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/grdhkdutj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gnorzrulp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/grggiwvmj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwrxvpcml.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gmqfaalrx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/ghtifzcyi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gsvugogwx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gouvxgftx.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gghpajqwt.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/grieopwab.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gnzsiffmg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ghbbfhvpr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gaqoqgxsv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwbtglgwq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoksrfxy.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/geykrihgl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpcqhnrko.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gndrzqneg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gxazhqjqs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gcxwvyvqt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gfqthrjwb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/geukccxhb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggwexrfmr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gxavdoedi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/geldlqvrv.sHtML


<!-- 参考信息 -->