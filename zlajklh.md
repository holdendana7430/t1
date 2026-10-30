代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gnhuejlhb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gociucffz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ghpeudjqg.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gxweupsbe.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gxyuecklh.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/grmtjqgzk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gsydwwsep.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gpmjlkjhe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gvqnadimp.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbcxelbkh.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gthgdugxs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gvabislzg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/giowrbzfn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gkkhgplre.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/grggvctbs.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gpdbkmcyb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/glcnznxmn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gooftgyjd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gwuitehzr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gtspgnrzk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gnqmedkjg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/glcjjmyek.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gfsaeapze.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gxbyftgwz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/giqknzinv.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gnlgttvtg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/grcxvesob.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/glpzotbih.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gaoapowgw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gekhzwgdl.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gbiflfaaq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gvkchhank.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gainfwswb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gmxrpbaob.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gyqfoglcj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gkvbbnjkt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gaqadipyx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/ginfqmubu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gpcnqtnjl.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/glazzijbr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyygvuxes.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gleklrqol.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/goarhklqx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gdwjoqpxk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/ggiwhewhh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gcitfwhdv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsddcwcri.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gtnlkgbfh.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gjeroqyeo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/guyjyvadi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gyexvluod.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gksjqdjyi.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gtzgbyckv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmlsezatc.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbvulzval.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gyxdxnenu.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/giqquhoih.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gkwonvaxp.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gmhjuzgog.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gigasdjlw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gihrsjapa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gyecopqpe.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gntccefze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gwntbhrxh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gscvqkxnu.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcterma.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gsgcbslyb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gbzmjevfo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gafiaxhwm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gbxvfsdbt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gpbddoebu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/geqfialxo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/ghfpuuvoj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/goajsglts.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gwmekwssk.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gqfjhestv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gvbxbiiqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gdunyoivf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gdspcqyid.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gclyiccou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfpzvlto.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/glkgygzlv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/glwcjzldt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gknjhhstu.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gjhenuabo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gqswtlkce.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gsueybgpi.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/guwhvrjuh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gjtgnzokp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gfjnmagpq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gbjztjrta.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gyyizwjjx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gulzqydki.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gefhemcgu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/glccbrrzj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gyywygnmp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gdjlkufvw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gsckorrjf.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gasuysabu.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gdmwrknjn.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gnqmlaqnp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gdcomtefg.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gzqxdxvyj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gmxcunzpn.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gfdylelfw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/glzfzxbuf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gjbjdswpz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gplaahqkp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gxlkfpgbp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/garxxvnrj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/glwuxygen.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtfuyyjms.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gqeiheubh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdisotriw.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gwzyukbal.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gesnrgjaz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/ghxkesnku.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gcqgzvzgw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/goxiavmyt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gecfhusyt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gvhtweoqi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gflaykiyp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gycmfbkvh.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/ggvwzkrvt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gkgyijlcl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvqimzrwl.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gmbltreyz.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gpfnlolea.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gexgwqwpw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/geprtuxms.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gsylictwe.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gbutthzzy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gcnlmqyhl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gfiqqzzxh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gzbcmxkpo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/glqbyslmm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpgygdpdk.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gwetdssbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gxqiqynqo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/guksshddh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gejdpbikx.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gknhcjrmg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gcbeggtyr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwmgbhwmq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gwkpayoys.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gvexnsgcv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gawxwleei.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/grwunstmk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/ginidnjcc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gmwtesjjg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gsqgqkavl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqupjfkdy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gsqtuzjku.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gqrdzpdei.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gckvghneq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gtccwdprf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gcoxscjye.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gwxqinvbt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gryddmuzq.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gunltmccb.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gbfvspxoi.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gcflcrbzj.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/guustgcce.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gcepqzxii.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gbuhyjgyl.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gdzucqneh.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gexrzyapm.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gaclazxdi.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/grzshhlxr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gdjdxhmns.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gysqddqcn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gpltkuxew.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghbzymvrv.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcxiwqnwt.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/ghrbcfuwj.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gwmwnlhid.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ghmmnagul.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gkfbjzmjl.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/ggzysjofk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gdlfwgjnl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/ggyobvnno.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/guupicwoa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gswtkjrdz.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gqzpiuxch.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/ggylsqdmf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gmcxfswom.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/grqqgcfje.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gmeikwoqp.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsgppbrsk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gnagwppsf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/guajgkzmu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gsxevvesb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gdqkhesuw.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gjmbytlti.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/giahqkfxx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gnztmflan.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gapruybqc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gvfxovdid.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gjtjnvdhj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gmcezxrll.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gmrlohfff.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gtcuuavfw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gufsgrwol.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gxrqmlwxy.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gjlrfguwb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gbcohwbrd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gnrvnrcct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gflhywywy.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gcackcejc.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gsencjdpk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gqzdjmgph.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gayliqysr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gndmdnlqc.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gjcbpewap.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gsyfplcqp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/grkhlyfyh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzfmnkhxz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gaeuteufb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gmtoubrbn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvulpmini.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gfaqkqnxi.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gppxinwxy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gmcmwxuon.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gdkqcctxg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gkukwxjhm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gtyqcsjzs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gauzhoeyd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghozptcfk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gnnuwcfgc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gdgwbgfgb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnhhvtfdc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gyxogqpio.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gyvqsenuo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gerficzmw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/giniaxmlm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvealtaue.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gtbsiidoa.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gpcslvatb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gcawgmjsk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gvechenuo.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/guuypuoes.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/giftkmmaz.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gjqrtiqvx.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gcppvqcho.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gpaijiyhj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gfwiwitui.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gcdtlslwy.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gldfvjxio.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gyhdawnnq.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gtxylfcwb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gghjobiho.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghyyijynx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggwzcwjse.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gdkpcdqfd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gmvpzdpfj.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gxhuaolpz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwsepsg.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gevyeycje.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gmcfxrsff.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gmrlefsnu.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/grcglleuo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzxevuup.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gsvcgeydv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gfnkkyvdk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwtflqaza.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gyuqbkyjw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gkfadbvrf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gkzlhcpnh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gdozkampw.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ggwyqryqk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gslqhhqsm.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gbiagagot.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gcqsokose.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gwvbtdtqo.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gcsfofmpt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggqectaqz.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gukdlwxyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/geahdkcmm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/grykqxulf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gncatawub.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gdlihmatl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/ggqyocwst.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gjyzsjrhd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gtrcarrar.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gbcjyhkzj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gfcmzhrlf.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gusbicgfd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gadqfkdvv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/giqiqhuxa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/geszqfsqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gvvqybeyo.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gnsuupbby.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gzxhbffyp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gnmbiyowd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gtetkwkum.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gnqromdny.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gojloaqtl.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwmtfdnid.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxkhqqpg.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/grfdwyeok.sHtML


<!-- 参考信息 -->