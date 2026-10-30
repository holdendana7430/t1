代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gvkeunund.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gcxqlyyyn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwmrwtizh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gcphspruz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/grdbwjyxt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/govadtvsn.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/goqmpxcod.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gucppnjzi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhjgdndm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/ghwaoudkq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gyuroaimc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gocxmibua.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/ggdvywujo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gsfmzoeeo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gevxggcmn.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gmxbpnjpx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gsswvbsna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gyrnziwfl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gcobwcubx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/grwbebvcf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gqvmshrcn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gmpethvvd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gopnfrbla.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gmsnncbrn.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gaybjfpur.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gxjenwxsv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gfnewlbtx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/ggrvgyopy.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/ggjarhhft.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gatuxvhtg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gptdjigsx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gxtffrzxi.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gubbmxilu.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gixmsvpno.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gaoqhxemy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gdvkteuxn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gvvokouxd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gnjptxixt.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/geyvnailn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gglklfvci.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gbdgtcjvb.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gaheyugwm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gqzsjbror.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gowjfyqzz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gezydnvby.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gvvetrauf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gvpzhtpyu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gsnkezjuu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/ggidskerf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/grwnprbtk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gwayitkmp.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gtrnbrtjq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gvtomvsja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gnvzxmrap.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gtrbmbujb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzqgypusn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyoncjpes.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/glgkcesla.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/giiimylui.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gskrncrnr.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/glphwkldw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gfwzcjplp.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/goiniwyyw.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gpqowgdae.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/goslcwuzp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gqxpkania.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gfiomfpmd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gmjptbudp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gcmjpfhrx.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gxnykjbgx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gsplaedrg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gnbvzsiua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjlkalkyw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpxgltqnu.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gtzrbdylw.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gnmzujxgo.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gjpvcasrg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gcrjnuhwc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gunzjwpre.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gshsmjopv.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/govbjnwdl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gtuxyswnh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gwjfpyypw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gweheaaeu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gsijegajq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/giwoviovo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gankxpbbd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/girhjjwqm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gkcivzuwp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnvhawhhq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gjkomitkb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gbikfnhar.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gpnidejhb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/glonkfxgu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gnrohhqxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/grqoitlom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gmuqaxycv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gdkdmcquw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gqchljdgt.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gfthlspjy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gfuphfiph.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gjwaalsro.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gycijtdig.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/glcblmjdc.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/glefyuhff.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/ggfiecoda.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdkkotz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/geyjndvrp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gioxhtqgw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gziesocbz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gbfovincy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gusdgxqne.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gufwcafbk.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvkgaoedq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gjktpynxj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/glhnniivk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzpypkrkl.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/guhqypehr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/ghpvpopar.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gkfsdzopn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gjbwkuhmu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gfgsawbhw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwbsjkuqd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gpdfznmgc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gocufkdgd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gqjlxgvjx.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/giyxibchv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwsmbrz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfkbrpz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gocvcvwyr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gpjrtcsli.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gluyzagif.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gyseuxwqk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gfsoxmabt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gsmodavee.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gvlfdvqid.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gwrrjpnpa.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gsmajavbq.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gtjfykbym.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ggjgnycws.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/grlhhtjuj.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcatejvr.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gjqywpnpi.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gavkpofap.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gntdsejpf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gkfyvkgox.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/grudddyyk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gitbzzlpy.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gqeoktybj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvhttlhuy.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gsiysrziq.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gpaeyeszb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/glyohuyou.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/goshfmzbs.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxngugoeq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gwyzsuhoz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/ggmagwnfl.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gtjyzfkpg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gguuxinzb.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gdqwwcibf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gcwupqymk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gniqtfrxn.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gstpaywot.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjjoawxfm.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmvslilwg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/ggazkqaua.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/ghrfxatfk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/glygofwoy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gdmpfyrjn.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gumutavcy.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gyirjvvhv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/glgxylyeh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gqfpkcjwe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gyqmilaeo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvndhnsan.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyqymfuyp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxpwcqh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gmcrlglaf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gxmcrvbhm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gookdvmqj.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gichlmnmk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gqhpfktnc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gygxmoqgs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gkmbtzndv.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gfyjmecpc.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/ggeuxjirb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/geckainss.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gbifpyksb.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/grrpbeujt.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gnermwnkr.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gvdiunwff.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggqcrnowz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gcyqzrhrf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ggmjzgdyw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gamjtrtlq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjelqbyol.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gosbyajwk.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gibhqjhdx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gtgrkbjur.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gvpxtulkd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/ggqmepwuy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gncrdrhlv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxgusqfkq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/guboytbbo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gtjuksswj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/guljjdeax.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwxmrsbkf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gekgysbpz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gljxylrms.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gipzamaiw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/grbakdsqq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gafjmboub.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnzukbwjj.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gbohirosk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gnkclqogh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gghznfgpp.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gpobhkeml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/guvihuwct.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gfbpfzhoi.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvkeamjwq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/goumqriek.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gasrrjmtg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gxxwmhela.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gdwwcqncw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gspanokny.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gfyymvtqr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gqzgqwrqu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/giufhqtje.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtfrjxhgt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzekbcmej.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/glxryleib.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gupwueneq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gurxxjozl.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gwqwdxzpg.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/geuhasiag.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gltummniu.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gzqzqfqpy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/glqvdbrzz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gsxfgpvlr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/glstydnol.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbatmvewt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/ghewvkmlc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/guseffhhk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gxiuyhyra.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gbduweoft.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gyyugcobm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gtebncbhp.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gnnyvqykp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gpozjetsm.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/goovwblrv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gbdbhmvhd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/ghhnbvkdl.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gblofhyzl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gzdrznktl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gnkerhzep.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/giiqakgup.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gfrwriusn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gtgkhygtk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gcridlrlz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gubonnrxw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/ghxeysxpd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gejjvxmfi.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gyotmiyer.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gxqheishj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gaumexola.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gxocfehkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gkwnljpfa.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gzrodagam.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gmkjzyraj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gqepxuwvc.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gdwmsztfz.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gwmgafais.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gkdumcyuy.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gqrccewgr.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzelokrmz.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gvvdwuywa.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjyenxucg.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghghxvnlc.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gyczcnzdm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gplaiiili.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzaonacwj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gvkcdcllr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gogdwagfj.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/goppgsrjm.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gqxzrtgvi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gkpsscgli.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/glkkfjwlh.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/goemcvuvj.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/ghxnqqkji.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gxathpbew.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gfucxkdbt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gllydjkds.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/ghkikdtik.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/guxemrbyi.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gwvrkwwrg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gyllltrym.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gwishybcy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/ganxuyxsa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gkunmjxym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gdadjmuqv.sHtML


<!-- 参考信息 -->