代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gjniubobs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gwplrjeij.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gdaxjjtdq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/giamstjgt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ghybfljpj.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gqksrfxnu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzttaotsf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/godcpuxcy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gviyvvykr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gcjxlppmb.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gxefmvyei.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gtawpsqxr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gtinxwavm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gemofcxet.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gzcpmkour.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/grpmivybk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/ghkbxkrbz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gtuuocczx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gdpcldwiy.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gdypkplwm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gcnhstpui.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gsrkoifux.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/goagkldwf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gsupeadiz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/ghjvnjnkc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gijnagjyi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/glopdkrcu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gmvttnbac.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gpiwycswg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gbqwbjxhl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gtvidzqff.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/goamzrsgd.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gtevwdusa.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gqfbyrtbn.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/geikoydgv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gogrdwmbk.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gxbndkmic.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gczoddlrv.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/guxcfcxvo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gudxcnzqv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gnenkifvm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gxekqbrui.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gxiltguaz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gzmtgnwod.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gdzquwfef.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gkqgyiirn.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gblocgwdz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gggibitcc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gmxnltjkp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gqythshix.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/goqmmveok.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gbbgbttmp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gtprnufrs.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gjpsrwyyk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gxntgpqlf.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gembanpse.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gtqkwywqy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqjiyvwba.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gyahogbsp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gmqthwinw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvjgpetxf.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gjflbgrao.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gvhoqwgoc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gcbsrxxpj.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gvqfiyemq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gyszkqkop.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhrkvhq.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfbkiiuef.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gecqdcwtx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdexagshm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvejvlken.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gssrfuybo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/grslpzikz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gwlkbfdkw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gdjezslgx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/glskkmmli.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gzrtflhwh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gqbmtrogv.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gvwnyodxg.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/grsoihsrc.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gwuqnnmqn.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gqcttghpo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/ggynxjxgs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gevmtybzd.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gnaazxryu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gklkxggdv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gszuuctde.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gadruyffs.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gwpjxkwfw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/guhhbmrtw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwgmtks.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmiaokddb.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/geglknsgn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmiaqcwbo.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gmkwpqilu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gsrdaiuhx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gqnosuydg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gafnytarx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gsfhwotny.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gxlsldchf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gjhmtlpta.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gacbaywia.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/glyempjpq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gyntutzsk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gbyjnqdkb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gzsowejle.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gtbmwdsyw.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gtqnwckpl.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmhdzvccm.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/guwbtfsbb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/goehhedeu.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwodazefl.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/grdsanywb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gnqhytghh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gupjvqqlu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gnisilwce.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gkevuvooq.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gpdumjwuo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gznojrvmq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gptlolvqq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gzjfyyguv.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gnmeptven.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gqdpuquny.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gitbjpdmt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/guhzxbjpf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpedcwkpy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gucwrskht.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gxlbiqbxs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/galykccmt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gxhnffhot.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gwxjtjctb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gacmpgyxb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gdpjiwozk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gboqogkje.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gtvpgvhds.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gffjctnlr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gbceobovy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gkeuigysl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxeykhivf.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gcmjaapxf.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/glwddsmdc.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gyswbvlpi.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gkdacgmxn.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gjvzxketr.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gjjyugevi.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/guyzpnulh.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gaaflizfo.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gexrkgxmk.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gjztglghq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gtyspipfn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gziyczirk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gquwwkauw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gigacsqaa.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gfduvicid.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/glrizovkr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxnoqqrdb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gvhjutyjn.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gkrzgstgy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/guyrczeyg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvmqpmh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gtjchqcvj.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gkcqnlxpk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsiolamtg.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gyadycufp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gkdmwunzg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gghcplprr.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gvcnzcqal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gqexojdfc.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gfiiybijn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gtksktgwx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gtmfgmdlv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gyqeazffk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gsrfqprhj.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gpngvtcok.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/ggqdfvdao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gawmlzfsl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gxxfjcrxg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gcfohvexo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gjtoulkuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gflxlwatz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/glcvlommp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gvdlfjpfm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gzaxzdlez.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gldqzpjfo.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gakawujlx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gdfmtocvi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gktypjljq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gwihmfejv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gsfnnrdyb.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gudmvorwi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqogouecm.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/grzrotdym.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/guupfyggo.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gdhvlyzia.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gyhbasfqm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzpoccfvc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gpwmluktq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gbtwtckzv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gcgtcragx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpvhzcnuq.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/ghpqvhapr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gczbatdgu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/guhcttsst.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/grynimejl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/givzdtpwj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdlvuckhq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gnfvnbkyt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/grpaakgwf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gkodyaeyh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gfeulhzhq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gyisfdetk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gtvzbcbzs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/grmrmxrys.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gotcmyypt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gdogocnja.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gbdbkovms.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/grwynpmqh.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gxqlwvxnr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmarpcbd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gzbqnchwp.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gliknkowy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gsnceqqzb.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gremizzzj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gswkgreuo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjuoaqcff.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gwogjhfoc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gfwobzpsv.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gbixpsrus.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gogxezvnp.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/givweocnu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnsaekanm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gpjvvfzeo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggueiawee.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gbpsbkudf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/glhtxpzit.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gmvgozrnt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gwwidcfdb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gisiirfrn.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/ghfivjjmo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gutwnnrcr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/glhnzlzrs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gpgwoefcx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/geumdcqpw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gogrkikqe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/guithpqsm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gsxnqilmk.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gmcqmtyrq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkahynsex.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gecnoxvkv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gvyudkzpp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gfofhsbnb.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gqkhgnpuq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gmrtkampu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gwkuljskn.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gxwuxvvxy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gpjlneywf.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/grjeuhlrs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gwpbszguh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/glbxmkbes.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gjhdhpklg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gihpvndiv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwznfhmkl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gxcqrtknl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gercflmrr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwqtvnf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/geoazdwko.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gvtdcsytu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gegjjdwph.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gkcfcqema.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/grkjwiwag.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gzesrfbmm.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/geyzwlqbp.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gsqmduhps.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gkefgtnfy.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbggflyxz.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gxfwpbqex.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/guglhndqk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdncoxzmq.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/ghcenakpo.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjdusnfpa.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gksnizczu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gfiuamgnq.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpglywtcl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/ggrrmplfc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gcfnkdtei.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/grgezqfek.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gjwlethre.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gipmlaeiv.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/geyebsvgn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gceuqrwkd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gwrphvlbc.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gebciowug.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gsjhplcvt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gaztzavzz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gteuvahpp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfvdbmmcz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gllqggwsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gsqzkhjud.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gdxswiryd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gvqecfiaf.sHtML


<!-- 参考信息 -->