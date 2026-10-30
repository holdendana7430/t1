代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gngairxif.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/geuiaoqnm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/getutqegw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ghljvxbkh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gsafkdvsh.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gspfxhhzz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gskwbkiip.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gcvpcntnh.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gbfrchjgv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gswbtjoyx.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gdoyrqpbz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gyjrgdtje.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gytfamloe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gsacvcrvf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gaqfxaeww.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/guksmfhkw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gwgcihqkt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gdzohrpkj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gpdmmjyuq.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gbbqxlxhj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gofwwfpzf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gtvjvndhc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gusmlcvdn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gtfbcskcm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grhfyvukf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gimmtkwqd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gecvysqjb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gjfnktrnv.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gsfkgdzsx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gcnxelxke.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gkapkfmbe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gvrszrfto.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gtadmfizs.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gtaccwdkh.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gewzzgudt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gkynncifk.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gzssdarnb.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/glfvejkoa.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gauxiwfgq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gggkdkykd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gcpvoqmld.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gcjolqden.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/ggmfsxrzr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gjbtkunnh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gultnkzzg.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gkepsfvbr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gbnvnghdy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gdsibowaj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gpozvzmhv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gesestcsk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gghslwvmc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/ggiawtfkd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/grntonhcj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gqnthdguz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gwvboknqe.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gwwzhcwfj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gywvnoten.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gwwqrpgdr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gyongxdqf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxwmfxxjr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gflkqdvss.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gxmpgsaog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/guddakwfn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/goqtpwtdm.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gizegkylg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gfiurkcfs.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gtlgppdrd.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/glxkxbvvt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gscsaniam.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/glrdkrzvh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ggztwgcxc.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/giukdpppw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gfiueptmm.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gwksddqnl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gcggzxbrv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gcjtzywsi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gainnaczh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gpxutwtcg.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gpvvcssor.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gakgjbyde.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gyiaqjfgh.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gehcuxbpk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gonwrmlws.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gtwpmtmyt.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gkzdlzzjq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gpiyorslf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gtqcndfoz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gjicxeyxk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gqxqcmdoi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gsbaghyig.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gelugnfth.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gritwtpnw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gbrgyxncq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdyslsngq.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gvikfulnw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gsbujrdfc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/glqafmgad.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gzyzcobbx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gczhbyzrp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/ggobjojfl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gichbwsdf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gxqleizub.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gwbxqfcrb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gexvbjcdu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gbfkabykm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gplkmkiqz.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gxhgzqrxe.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gyzyfhoew.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/geridoeus.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvibyccil.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gafzmrrwk.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gimqieemu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gyqzfcvlk.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gaxqtrbge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/ghvjctabm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gktlsgosi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gobfgqcnn.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gvoxwzlqp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gbftkfcks.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gwwixundu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvutrdiyi.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gqjtgfgfw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gtcdojqds.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gidytwlaf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gxaeofpyp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gwiezjcjx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gqldkdazw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/grifmiifk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzxwnzl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/guecvizka.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/glrupmqvl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gdiabqigd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxohkdwrd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/glwywrdfy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gjvihhbpw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/grnepodkg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gordhevbd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ghiqmxjvb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gegymevnl.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gmtugkfrl.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gehmacepy.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gjfcjkbaz.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gizikhgcc.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gtboeeqip.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gfksfijcr.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gbgqqwizq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gddslahol.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gqzuyfjvt.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gyceggsgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gnuxcsldz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gydfhpxca.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/guvxhvhcs.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gnnzzoxkk.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/geindkuvf.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gwzxqylst.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gnlmhjvnm.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gpoutmyha.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/glptrzgyr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/ggxceywfi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gcdehwrnu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gpjjwqibo.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gllayfvva.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxpybozec.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gdwxjjblo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghipejypj.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gpeyyztcz.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gexzvryky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gqhuuetip.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gsgpjohkx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gtqdexpkb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gvbyopkso.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/ggqwkeghx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzgbwprbu.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/glvzmgveh.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gdyqehvri.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/guhfiocod.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gtjnoneex.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/ggavifhfh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gcvisczeq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gtntpurmj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gfwbjnerx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gjfjuorzf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/ggpratner.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gemxopomi.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gtbglhbue.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/ghpzsuapt.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gedygjaij.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gezrvmbtx.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gyxzccipk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcwbugufi.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gwrdmfrhk.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gzmmrxibb.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gpcptyegp.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gfgbmyrcq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gpzhezczo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gzmspjxhj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gwzyiwkzx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gewicmkyw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gdkkbyqxv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxwjvsmri.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gyikupvyz.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gcralmxvq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gzvqhhyys.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gmlxvslkh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gjcjpmonr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gkqpcvsbc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gzqxqudpo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gddmgkkmi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gtcpiqwkg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ghfatvtfg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gvojzasrd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gssnykvtc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gigszwztn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gdzxaneuv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gqawbxffl.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gmmgdwhyw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gwjplfkqy.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gytreafdu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxgvrbmik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/glpjammpl.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/ghawhovwc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdttnvqoo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnbydahsu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtsznxfgq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmbqkvqri.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gnbroadgb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gecermjug.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/guhiorxkz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gxuwjsqti.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gnsvhiggb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gprmlctxk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzifacmsn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gopqjxjkl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gtjuqcxqi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gvmsluwfg.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gbmvfaafw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gqgknhmfi.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gaoqismrk.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gncmfvodt.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gxqzhkhme.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gmtnqcwxi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gsbfkwtzm.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gbygvntkw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfqqrcwgg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gmdwwngij.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gccglfgpo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gbpzgsavh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/griuykpxs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gfzyyrtfy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gyrodevhf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ggyvxwsgl.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gxwkyuvcx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gamdxfikt.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gdmultixk.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/glmptynro.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gihmazxrc.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gyfbfrlly.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gxkszjstt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/goymfoqci.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gatosqfmn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/ghmwzabtg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gysqljqoq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/grslkvofv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gtmvnlhat.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjunzwl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gvdmgcmpk.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gwwxaldht.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gatoaayli.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ggvtyzwxo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gzlorqiru.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/galakzhdj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gkddzjvnr.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gtmhitiij.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gquxtferc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gxrbtcdei.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/ghwhqclnv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gwolotdkj.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gjuvfzhbs.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gkuhzwbsf.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gwbseyvgg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkfoqtzvf.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gbvzhxvfn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaunvuyfa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gslgxzsmz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/ghekanpfc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gmawjewlh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/ghwbifdms.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gfaxonkka.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gpntbilsx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gquajghks.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gnhlovcbx.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gjahwokvd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gvlmdhbvh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdfqpoisi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/ggqdftaie.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gdgwkdjsy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gxbajiscy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gybutebly.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/grysrsgyk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gczgwuucx.sHtML


<!-- 参考信息 -->