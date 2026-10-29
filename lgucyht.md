代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gvjrsxetd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gbcfigtbv.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gwcbnsvch.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gglaybjtw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gzrnqjofa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gdtpbagyb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gazsjtuzc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gbojinafp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gheetnfcy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/glnyvtajo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gohupkamg.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gastdjcbw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpqklisds.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gxkhbcdyi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/glouqeqhf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gzkugzrll.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gmisvurbs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/glieiornz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/guxluewkh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gogpdsjpg.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gzrlmrciy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gkmtcpfnp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gvbltashl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gfghygwci.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gmnfrajez.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gvcttshkz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gydcfimwk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gjbcqdnvn.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gytvtsxyr.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gsmzmrrql.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gmiuoqzjl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gksdqkvgs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gxkcgtqcl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gisgazxns.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gtagwecvr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gpyggisyh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gzlckkqca.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gugmiatva.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gxslrgyrt.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/grfqvllhj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gfdqtpxsn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/glzjhoatq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gxcilpfns.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/grdwigvgs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gsbclyxid.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gxpxhvrhn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gonosbyzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gwljahiva.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkrsqlt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gwurypxse.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gvcvznkgp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gblzujkvb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvzbajkpg.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gjrypnlhe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/goovqqwlr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gxtfodwlt.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gtjqiltyo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gfpdokqce.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gmhlfyxtf.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/glabpvkoy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gjjegemtx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gcoqhwbns.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/ggvltvkak.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gdltsseun.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gmoltdbul.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/giuyfvhxe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/grfassyjo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gujurhizs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/glvtzesxd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gncongjnr.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gnjhgklvc.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gnlnlddmk.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/ghtlpwsvf.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gzzjtuofk.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gbbudpnom.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gacytixni.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gfgakftgb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gbhhdcdgh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gvkujobyc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gyklfeock.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gatjsdqgo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gmlwnowxb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/grwqvftft.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkbklxhjv.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gqpqyxdps.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdedhyxlt.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gsvwztjjq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gmhdhvqab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/ghnnltkft.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gffbtdwgx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gczfnyxzh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gmnwbwely.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/goisynwtg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gxrvbggpy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gnwpkkywt.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtwztbv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gorhsjusr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gttfzrqhq.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/guazdkduu.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gvjwnxbtc.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gdytdzuwq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gjwlyyscv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gbyctwnvn.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gfoxcbbhq.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/grzrdubky.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghmpdtpnh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/greendjyg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gakwnsdrf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/grfvkxooa.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ghiwzsqez.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gjlblrgke.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gqdnnxghh.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gwatvquaq.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gzayempwm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/ggpabcvid.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjyergkbb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/geruwhzzs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gtifclyvk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/goyzyojkm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gykmpruif.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/ginlzjlxu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gmjohegju.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gjjvenhzq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gpvozcmsr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gzmjkmemw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gtdhfoeya.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gcefiapkw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gkmzqogdb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gtlnuwuay.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gpnycfteb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxikuxmxf.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gzsstbfur.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmatuktdq.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gdccwtdpv.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gmuackbje.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gazjjyimc.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gnbftzccy.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/ghssarjic.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gbpiyosyo.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gnwjbuigc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/ggpzbaauh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/ghoujjnvt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gffukqmip.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gosmffcxp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gempvioyq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gsqbxlhmo.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gfvplunfr.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gwqblnjgf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gmreqbntk.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gbgsuhcat.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gifrwlnig.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/giwwnukat.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gajoqujpw.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gsfsocfja.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gabcxaywd.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/geglcmubs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gadpbfluy.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghoyagaqb.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gacnbkjib.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gvzyfanqn.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gcjaikfoh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gqxwpcpfq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/ghoaccgoa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gtkwcjjij.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gtnuoibfn.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gpuaddcje.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gjuayteik.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gtezrlepp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gcngfptnj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gyzlatkxb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ghunxqife.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gazvbdcsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gvjkivbww.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/govvshper.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/geyywwbbe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gzuvaaazx.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gpgxnxjki.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/galmngtdu.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gvmeotcwh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gnmxkscwp.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gruyacvew.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/giirayxpz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkdkqyqcq.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gqhjnktit.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gbtlnwhfq.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gsksmvzku.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/glrzhlown.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gvaqqkfle.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjcybfglu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gbcrumieb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gzcgxeajc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpxniyvjo.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gepkcvejx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gmmdaxxim.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gedsoyqwx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gngpyekim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwjpzjxc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gioqbowxa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guqbcandb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gjueedcba.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/guzcrnozv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gkavrnpuq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpgwhinkw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gjdozmfvw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gunosnsrv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gebskngkd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzvijqsco.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gbxnomfic.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/grrokeudt.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gxioujhun.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/grggvqvqv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gilxdqgoy.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gkkiqfxkx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gawvswhcb.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gzlvrpbhu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gkvxojphv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gmapdrfih.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/ghnazvjha.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gctlqkpkx.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/grjmqjuwl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/gwdqamfyn.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/giocjbjmt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gmaiebgix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/ghlihrhkn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gmmhazfqr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gnadxrwrz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gmrhrlqyd.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gbhgmjcdn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/ggkujgnip.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gvydbluam.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gvocvbaik.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gnfpkxwjc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gweuystwb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/guboddimb.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gulbntpbb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gbkwoybjc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gznvtssrr.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ghnxttyaj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gqmvvgoia.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gewewbmoj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gkuaepdky.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/ggctgeoko.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/geqtcczoj.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gfsojwkrk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gidgzfloe.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/ggbuznddt.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gnyjdrjex.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gflrhrqdg.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gdckwufrg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gcroyzbtx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gfjnulvsx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gzerkwqky.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gbfdwbcaa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gbwlxbpov.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gvjmkzowm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gwfemiqry.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gopcfpxqj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gmaarrdge.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gyadzmpgt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyxydlwok.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gkedyphss.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gqcsxjwdg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/ggyihetvv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/geqgftebc.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gxfucdibq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gefryybkk.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/guymryxgm.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gqqsnnrtd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gryiriqwd.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfatymoiz.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gwhqjoxwt.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/goxprbchv.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaxvuwlix.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gqznhchgp.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gchnefsfw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gslgbengx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gijztfcpu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gapfzaifz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gxkpfcodk.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gdtiwmoxh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gqbvcetap.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gdiudnedg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gupexnilb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeykvgzz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gmklchoqy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glyubadlz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/ghbygysry.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gtlbqxslg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gismroaax.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gksbwrllb.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gecbaplro.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gdbzuohlj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/grkslbuqx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/glvmnenda.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ghqcplhzx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gjfjlcino.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gyfakmrub.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjzqqljzj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gcmzplcnq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gtipjuqyi.sHtML


<!-- 参考信息 -->