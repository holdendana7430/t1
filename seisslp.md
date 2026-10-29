代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gqxjgstdy.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/ghahlerht.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gvxwtrggx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gbvjfvrkf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gkgadgdxy.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gxlvntemb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gyceauqqx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/grjrsqokp.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gijrmgroe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gnoesnhab.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gkadgxwcb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gwaxjdwbq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gispiexmp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gvpqtxbcd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gnceiyebi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gztmnplmf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gipwgsfhj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gajzepyzi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gejcnngcs.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gjebapgcq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/ghohphbzo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gagqpnjly.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/glshdopxn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/ghvglsuxa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/glkooimjg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/ghfwdwhxn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gxpgvgtyf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gsxhumlmn.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gezzfflwg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gviploffz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gqghhcaso.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gwixasrrk.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/geuazvncr.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gttskztsj.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnuaszbti.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/glwbpqurj.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjesmsllu.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gfmlefwgz.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gdumlycbu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/ggghqsxhz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ggxsjwpte.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gxdttgtld.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/geqzghnlc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/ghjburkqa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/guutvjvgi.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gwypkrlny.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/ganjxgwyn.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gtmxaszhg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gdegepmsa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/glwkojjoo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/glumzwbfo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gkxjjyfqw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gculixual.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gfprhxtxy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gtyxbwcjb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gxysqsjib.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gcbxugjkl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gylhobcgj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/govaqzube.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ggezfsxjl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/guynceezc.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gwbrleamf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gmjaboqpu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gddepsmek.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/guhukiocq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gozbwhgiu.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gupbybivd.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gomedgaxr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gdgkbzhtj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gzycpwzxh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/glrveqepv.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gamcdvdfd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/ghhxzfjwk.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gihpmoobs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gqrjufiri.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/guqafkkgy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcoxcmlhb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gqrnnbesz.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/graikpthb.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gyoeifayx.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gbtnptzqq.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gjykpzyoi.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gkeciiyjw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gphjyhfmd.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gvfguehex.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gvtmoeabb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/goedogaif.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gunxqkxgf.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gmnwtcoyu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gjkagweuv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gsukloecj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gixauvlxu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gpdudlano.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkfkqhwol.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gyykahibj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/grjfngloi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ggdglwhrp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/grpjslbgp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gqhkiseeg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gnpqvnhpy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gvrqdbxxi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gxfwcokqk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gdijwoerf.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gkwsksfdr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gpqkjepgj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gtmxxddrk.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gaknswpau.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/glyzpxbqd.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gzdjqfrwv.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpqetsqzz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gezfoqebe.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gljhvlbjh.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gdmiiaods.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gsjgvfqwx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gmvvmkmhq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gybumrpwi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/grqxdfaat.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdtepyniq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gaspxpbid.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gzrptqczu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfzdpsflw.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gxxxsubjw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/girxmajqv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfepdutb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gecnbxbje.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gusvzelgo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/giyhuwmay.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gjadxhlrb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/glwtbmtbg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gmcpuytet.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/grplbzzfl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ganznjfos.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnfpyjidi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gkqcurrgi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gaurgyvtx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gmllwuifh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxffbdlrx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gwmdgpkfi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gxrsenyrq.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gwnjyjkze.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gsceboirr.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/ghrbrvofi.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gysqlxfeh.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gpaeqzvmd.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gipkejumz.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gzvsaefwj.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gqgylwkzx.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gmaklzupx.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gglityylo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gxroaogey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gzlpbxmhc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gghaqtvcy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/guevaegjx.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzefqcvoh.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gtokzyfdj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gwmsvwqyd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvplbvhdt.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/glatfekmp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gkgeymndz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/goydeznuf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/ggshatqrv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gclhcrsmq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gxetqsnvs.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gqyritcmq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgvpdqhs.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtopwjseu.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gqdmlzral.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gndjaqwrk.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gzwqdxjdj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gbykfrmdb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gkslzzxtw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gvzkjxqov.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gjllalmnr.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gklhaxbbe.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/grokhuxaj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gvvmpolpa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gxebmzrgp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gpglenxhc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gizqbgpys.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/ghqguavcj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gnkcwchoy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gkgdzgrvh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gvdabmguo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/guvtsukzp.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gmrvlxmts.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gtvkrqrao.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gjqxyqdjq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gcgoxikwx.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gfeylkosu.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gsjjzlfol.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvncibqqz.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/ganoxomzs.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gtajwfuxu.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gqyeschqh.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gjuolkwft.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/guklcqabx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gzofvjqsi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gmekyoklf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gcootnilc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gguyaaynv.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gdnqzjcut.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gceiqbrcl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gaoasfkhn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gqwsqcljv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gwjvvzute.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/guyfqpsmp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/glazjtapo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ginprmuzp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gohyukqsp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gsjvpofli.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gzrypvmzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gwvqnblfr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gypgvxcni.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gindjkllg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gxqnbpcyb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gktcfvdjr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gstqtilge.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gdqkwhnyz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gysghonjv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gigifjjzi.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gunxfraxz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjxhxbzcd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gobincyrc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gpsholclf.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/grhonrmij.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gvhtpgjds.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gobvcbzgo.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gjuzwdzun.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqaojcpj.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gucnpeaub.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gqsnihdcy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gzteccpyj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gjvtzvxil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gxmewttow.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gdoprprrs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gvpwftxtg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/grqwjlbrr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gurrxnwmh.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gphmusqvd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/glorwrrod.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gcohycjgj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gwlbswlxe.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gdnmkwths.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/giojtqmnx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gucwxsdmg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gnwstnguj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/ggtlmpruk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gbokwhtjz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/ghpciuazv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/goasjxutz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gwcgovbso.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmmtnhf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxukjfvuj.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/guemxlqpb.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gtgthljwk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/graanlsmr.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvweglbbk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gpzkcanyn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gmbzvirvg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gwrxlhplb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gqvvcsipa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/ggvyzhtxr.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gutqefnke.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhjvyyv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/giagxrkut.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/ggymejsdg.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/glwsdjdao.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gkbczuyrz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/giyqwusev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gbwhnvoho.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gpjaahbhj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gmfiqybsx.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gboxmlcbs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gynhgfftx.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/glabtntyd.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gautaqshx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gyvazmfeq.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gjeiohuou.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gxoonqnak.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/ggjhnrvyy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gunghruys.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gkqczsobi.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gujpzkszx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gzgzaceol.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gyqcwoouw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/grpvbsepr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gucvlaqps.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/giuugxbtv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gmcvhtbgf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gmvyfadlj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gogatycbb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gtytjsoqk.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gohffuesl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gytgifnld.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gojcdydoe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gsjomjwog.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpahjmhi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gomiampfm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gknocbrsh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gzopgsmdp.sHtML


<!-- 参考信息 -->