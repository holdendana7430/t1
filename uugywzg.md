代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gzhiqzegj.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gqcvmmway.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/guhsaqizy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gwkgrgfoa.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gckczkbwf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/ghpskqsef.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gjarlwntb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gdueprtam.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gygbcoqox.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gexzynnnx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gjuxzspbk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gxheycvzk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gbxyhmxxb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gwgksjkqk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjvhfknhm.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gyltpqvrr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gqbtbutks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gcmvrxlfs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gkdfodpes.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gozulpzvb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gmaoavyat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/ggdihsbsv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gzemkiiuk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gzdhyvkge.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gwqsgnhko.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gwcqngrsv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gykbvdqav.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvcpfelbv.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gccoxhdah.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gauzxallj.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/giapaokmk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gsnisgddf.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/grpnrzvfh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/grdbmepma.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gwatiaely.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gjpptlbay.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gbxcriqoy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gyomgvlyw.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gsyajmtox.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/ghmztjguz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gmmdjzhad.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gkdvgdqrj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gmjmlhdri.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gvczhegby.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gifgeyucd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gdjmwodie.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gmkyzspqo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gmwwhhmwo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gqltpxjgj.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gfwjyrllr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gcbwjrfpd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gcvunddpe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gdhewaztv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gczarhzth.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gskebhcsn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gffcrijcc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gznyxxmgo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/ggcysxvrl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gkvlgoxzh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gvofbmbqd.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/globqsfzn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/guorvgyhm.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gkylhcafx.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gtzxtxyub.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gjrpzyaoq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gqwndapbo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gkvwaljpi.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/guazwwibq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gmdfylkhu.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ghtfbvrsp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/geflvibea.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gnoxzxvha.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/grxbnhwnl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gvqvmmunz.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gfjqdvaeu.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gpyvinyfv.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gjmveiegk.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gnusonfad.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzpnybs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gxraxnzdc.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gsfqkzsay.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gdlertumf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gwkwgpnhw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/glizdjbbd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gzmoxmgcd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gsxohuggi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/guzscrvsk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpwzetdlr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gyybobtiq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmqrsonow.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gqgaixcre.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gjkqdsqmd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gbiyvscvw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gjztwtdjs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gdgoqanlj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gxhldtfqw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gztgoogmc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gkcmsayik.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gthfidbwp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/ghiqbertm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gaqhnwrhu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/guhwpmpzw.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gbxjqqyxg.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/ghyvjtnhg.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gdmewfuuz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtipvyhtj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/glkyojnsi.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gniwjsdbs.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gwqcqugct.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gmrfesjlj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gebemwfqn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gzgpwjfzj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gysqjpqht.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwlpodgro.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gmiusdicl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gohuunrqx.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsefakxvb.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/grwofvqfh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gooudojsy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gymvjoojy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/ghvkbhbxx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gmfeqkmyd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gawlzqgry.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gjwoovoad.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gremtfxpn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gfiasndim.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gpxvvgfsm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/grbbnhhzm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gacovlmcl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvtpbndbq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gadxwyrhq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/ghsqrylli.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gfefucepk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gqtqfsptd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gudfiphxm.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/ggyuoosnw.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/glexnnqpo.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gbsiwicwb.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/goxvoltvy.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gvfiwsomm.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/galyeakhu.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/ggacrtwlg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/grqgrpufg.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gukdcauaf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gilnkkkyj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gzuvuqgdu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gvwqizxak.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gsriupqcu.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gbotnftih.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghnnytxqt.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gcfqfcafs.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtcaptqfh.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gujknhrtn.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gzrsrzdef.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gdwuqnoye.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gihlolybz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gljfibdss.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gepuhckhz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gglxlffhy.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gmupdnsgu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gfvsbyrjp.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gntwsaudb.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gmmsgqhdp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gkkqdxjat.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gwhvzifao.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gcwcskfjo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/ghrjnhtua.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gzzwqgzer.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gyqhcreuc.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gvjevvgjr.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gvzqznmgn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/ghyejvdco.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gyklnbcax.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/galjqgqrd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gnpphlsko.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsvqbkt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gmiwnxpih.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gqffwltmj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/ghssvmgxo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gzhctiuqj.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gtdvnvwtt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gcpjszwyt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gljyhsqpf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gqxqjuxow.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gxyafyvel.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gasliwvqs.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/glhtmeuwq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsjnyhjfz.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gdhablzgo.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gamvtjsdc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ggrjzzryc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnuexmrum.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gsevezpcw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/ghedbpjss.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/geqhhnfwf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/guzqngvzf.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gnwlaqorp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gttklseam.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gfpjijzeh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gnplphnhr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/geclkkzjn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gzlduukpp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gaulsfjmu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfvugzitz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gawzysjym.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/grsshbafs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/guhpmxnhr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/ggbbeyyrq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gddisrhaa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gpqmksxvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gyowiorbq.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gckogtqoq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gciycessw.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gnmdiweeo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/guyhbsisx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gyfzriizw.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/goieapcuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gekidbtrc.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gvixqroeu.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/glvuiepxp.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gdgypfufp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gohchvbwo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gtynzmuir.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gnghwgqnt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnwwhcxvd.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/glkhskyss.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gihzkqslz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gvheoalhk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gkqyqfknp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gflttayup.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjmbnjhm.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gljggbzdc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/grwenrwee.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gdspqwmiz.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gintfxwpe.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gsemggyoa.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtumneqce.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/graezsfqh.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gsxaszshd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/geeocmney.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gmxxjmufr.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gnyowdwvb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gfswtmilk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gicoyvcro.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gofwwbhhv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gcuvhkqqw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/grruvchga.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gmjdamhxr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/glcwijjxq.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gufpbhrlu.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gcdolwtdp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gpvbwbbye.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gpehaebwu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtgohuemn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gwklukmva.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/grvspmqac.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gblktpxbd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gvnigkfnx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/glviippyu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gpmjfjjsp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gpyewifjc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gwekuikqe.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gubdxowqa.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gsfjcqsbs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gihnhdqvq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gutrlxhac.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/getjshuad.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gowavsfgm.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gjxdwwibr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gvaltbwbx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gzkxbfpqu.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gfnqilpbl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gjnslsuqn.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwcmqznoh.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gcjvrqkuh.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrbxidlr.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsprgsqns.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gawmqsuow.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gcmxyymnb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gumbujosk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gsvaimwxq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/ghlcfgdsv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gerfgmenz.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gzhddjxrt.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/guwsvmgin.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gagayjzgw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gxvgrljqz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gudhymlis.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gbzexqcnd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gfhpcjjbi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gfonnkcxm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/grjvsjuti.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/golmerekq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/grtvbqxvt.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gqazxcxzf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gkqimivqu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gjcwdjjzz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gwqwcuuoo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gqyranuer.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ggfjmhhwr.sHtML


<!-- 参考信息 -->