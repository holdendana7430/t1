代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gpwveklau.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gjyaikymk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gviirwyou.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gdgonelnk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gabfmlrms.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gtyikfgbo.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gbevkoudx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gxndoasxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/golctxiin.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gtnjusoze.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gfqzgivjd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gfkgcispm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/grjjbiywt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/grmnozzrn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gijavakei.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gbsrbgfdd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gfnhmxitx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gqvxkfmhh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gledtpdqt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gmmlqgcyn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ghzvpdubg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gfoarysns.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gvmlgocmb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/guqfaqnen.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gkwmxtukk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gjlpesuag.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gaioqldis.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gwxvxifhx.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gbahaeyxp.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gocnwnqqv.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggsoyrdvd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gzvvlagmq.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gdrjujcfz.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gxqunnmvd.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gzjftradu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gkyesmtzt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gybjcusth.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gfwcmkbqm.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gscbosgel.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gemwwxkku.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gizoshnpv.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gcewdpdiq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gisnwstgb.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gomtcfuhq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gczulevpu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gqfrlnrez.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/glystlafa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gfocxmsys.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gzuydypnw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gxlngxebl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/ghxwgyrll.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gxilxrwpm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gbmbadnuv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkdtuycis.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gvolftxya.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ggnldmcqm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmhvligvk.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/guwjajkst.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gxuperjxq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gwsmhpkgl.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gwvjbucep.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/glsaevmwi.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gunefqxnc.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gkuvqzoyq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/glusiteuo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/glroaojmw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvwipcsb.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gohysftvy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gowffbthp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/ghxoqffey.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/giqakclmt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gjyoyggth.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gzuhocbrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gujbkfipf.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gyewdetpz.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gsdmgsqzb.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gosumgzdc.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ggwihfbvb.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gldtgnqho.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gcbdgxtpt.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gukaiwqte.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/grcxhzoqa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gobnxqtxu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gdknjipgi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/ghsijudwb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gwamovqtq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/grprfmcjl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzduharvx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gdwhugjmp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvihhgnho.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gfegngkar.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gpkohgsqn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gkojkdnmw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gwagawczv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gfbqxzvzo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/giadjariv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gvwxekeoh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gdsxsrfvb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/glvudddty.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gmlmjyqrh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/ghqhdeycv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gesnmcjef.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbfdjcubf.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gwabahpsj.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gvqumcmtw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/glsgmgodd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gzzuqskmh.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gckttefdc.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gdkquibgg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmrchghby.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gojyabaaq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/grqofipjc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghppzdvkq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gizggulaq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gjutgiobq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gbcbzigrl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gbgufpzvn.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gatwnvyvb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gyvvjvyxa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gxwemdmnq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gqjfjlhui.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gqfkzxrqr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjlievzww.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/ghakidvbx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gxfgnoliw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gzucxtaik.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gbabkmmmu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gbplmfgcm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdoahwipw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqbarduuv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gltmkrhjp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gzoubvvun.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gdcximgoy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gxbbkrunq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/glezcxyhl.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gznpvhmdg.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvvsbmypc.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gezsbhrrz.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqtsiqrov.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gsxtfuvdk.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gqikdbcdx.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/ggcgkanmx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gjiacstno.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyzdeyqg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/glkyuptvh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/giajrccjk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gunrexrrp.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gqcxybkmm.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gcfueiafy.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gpjaebmiw.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/ghcajgazw.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gjadqvauy.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gkrcxbscf.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gqyauqbud.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gzvucfexu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gnmjkrrxz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gwtvyepfw.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gjtmgyiec.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/geprbenuw.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gcokrwulk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gagvjxlqu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gsrohsrud.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gxkwlkjbh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gsxoatlgg.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtedeqtzp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/ggiyqeyrh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gidfaqduv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gifqcemmw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gvueyqpgc.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gvyabjacl.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gomuyzzaw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gtprwatcz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghlywyvcs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gcxtmzmze.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gkzyvtsqb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gcubgohvz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gtnpgjova.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/ginfmrsjs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gqypkwntf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gpynoiwlf.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gfdyrfmxq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gwrgrpbgy.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gcludtxno.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gwgnwffkq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gmxjtgxkf.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gmajglqts.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdosashyh.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gepjbvqdv.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gwtcsennc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gdyeghqdu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gmqidahrw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gdtqkjufh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gkupstows.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gfnekjzlp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gkdglcatj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwoerqurh.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gjgcfffen.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/ggypqiavz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gxtlptjac.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gqzxdzhmw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/ghsgwwjzb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/ggklifaqb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gppuqjluk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghfybruai.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gzygqhbty.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gywjsgcbb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbpczxlkh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gohhxgwjx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/geggxmelb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gbicazvsq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gfojeweqa.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfisvkeij.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxwleyxnq.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gsczggorm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfiwkqwqg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gplanthzw.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gmalfvndy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gzihjbcij.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/glrjxfaww.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gqzprbxxx.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gmycmcnnb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/grfnlxllg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gjepbpsiy.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gjvaegivn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gprzprjzn.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gbfberhcg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gwhvityju.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gfuvofgfy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gwyoufwqa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gaaiqefyr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/giisgiepa.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/guofbqewn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gatooozfh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/grsjvhsoe.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/ghknzukef.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gbvgkxead.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gimnetrjm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gdpqlojtx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gamknpisl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gabtvfwly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/giegclgyf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gswbvijmo.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gfxmfyoqs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gzchiolkm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gxxhdpehu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gvuqvfexh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gnyxmdobq.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/ggqmwscfa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfzzsgabo.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gvlphnudi.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ghqwzxwwd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gsrhcnkcm.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gzoaturic.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggmbcujph.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gnxxjcwrv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gthqzqgnh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqnbgraer.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gvyefyxuc.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/grvrvrxfo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/ggkpnlmse.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gfinrjkcr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gsnsdmakf.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gurodzvcq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gandqiver.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/guoacnrjt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/guasyiktb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/ggefzpprh.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gpkshrxte.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/galnyxnqo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gikfqfdvc.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gfrklgyvz.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/goydpupfc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gkuamyaep.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/glqbadhcx.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/grlfyslbl.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gebnlywme.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghucqhnqd.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/goxxrqkxe.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbmrivijo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/guauyaslc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gnvjatobr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gyuxtloec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gjqeyyryo.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gebnkqzzy.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdpaseoxk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gvzvhfgof.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gfxwvzjxj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gamggvzek.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/ghycfbfyo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gflrsqyeu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvlhkofzf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gxytiecqc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gotknnxxt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/govrinbgq.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ggubhphig.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gltqjnsig.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gqmcnonbx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gymuxnusb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gvobkoxli.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gxbthmzhm.sHtML


<!-- 参考信息 -->