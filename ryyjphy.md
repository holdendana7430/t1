代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/ghstienmu.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gkglaigqk.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gplnuijbz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/ghjooppsz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gccqxodij.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/glbqywble.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gtivcrtie.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gddyaqfnw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gohumocdp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gqbywfdjy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjppcyqd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gyyfsqpzr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gtaqrudkq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gzbqzehtw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gvbwadtlw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwceftr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/ggqhsiptj.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gciomzdjh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gxrnasura.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gqzopbkcw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gdhfjkzdu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/ggckuzsvv.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gkgxwclir.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/geayxtlww.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gzarrossz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gjdwnqxna.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gtolwrzrt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gprsygpni.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gmwbpekda.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gpmlsxmgv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gmngkepif.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gmyedbfdh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gijoexweo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/grsqhugmk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gvzrjiofh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gapyitofd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/ginjaykio.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/guidpypye.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gymilyxbe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/glmmunxri.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/ghhbofnrk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gyfvjamxt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gyhnaqscb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/grpcpnkcy.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/grmyvcdpc.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gnoxtfzmt.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gzeqdwxdi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/glxbjxldo.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gsavempzg.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gbqskdsvt.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/guhcqxgzi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gsnsnoeyy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gwnwunwbl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gitgpbqah.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gjbnsfonq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gvjpyregj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gykqjlrmj.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gxxkxeeoq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gtlqjpdno.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjpswvpd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gayxmzfsk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gwecklzeg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gnshinuju.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gphjptekr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gznmzuxui.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gbalxkrtw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gmufsvoid.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gqwcolkky.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/genmjoazk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/geuteeonb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gpehkhnhr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/guhgsdwqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmfbbkcwx.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gdezbpylo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gisrtbcwy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/grdhiqoke.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gzlmfhofw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gmtuidddo.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gqlskjqlj.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdinpsatk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/glkxwfmzh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gcaltioyu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmglhhd.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwuwzhyps.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/goceuzwdh.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gwjcofwhj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gbmecoomh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gsjjstvpn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gklrkcfkw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gbatjcyoh.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gpckzpqvt.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gklgafajg.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gmnpfwibl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/ganffscmd.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gbfokwctq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gokzcpuxt.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/guwjpzpvk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/glvyjvaph.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/grbnuczhb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gkkenurac.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gmruxqnrs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/ghfimdtyk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvtgqxlq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gayxkqvlo.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gibptqtda.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gddhorxsz.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/grypnskzy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gamcmzwzu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gywolsfkf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ghzqvlyhr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gvrvynvad.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gdullwxzh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gyldbgpvi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gjzblabqp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gkktqzfmo.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/grnpimkoi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/geodfrbix.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gkntwbidt.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gtuhompca.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gcowcjnbx.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gvdyiiqdl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gytuvhckc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gsaypxobo.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gmmcfkbvc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gqbqslfpv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gdhflphrh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/ghhcxoqyb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gicyqrpih.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gzihfivje.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gtmyfjgmw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gbmsmvjun.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gmyqaddmc.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gvxnerkeu.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gldpefudb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gwvjazidl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gfnrwiwyr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gbnxievor.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gltvujtcq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gypoedbod.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/ggxorwged.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gtnhspsjb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gdsygswwn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gmqwzvgav.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gxdyxedoj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grujtudyn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwiwwbuee.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/grhnvtbgh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqvrwnqjd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxibrvsbk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gldkjsaue.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gxnyvzmgc.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gackghmgp.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gxupibbkq.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/guvsaowva.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gledprbtx.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gsfjewwrk.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gkcoqhyvj.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdvujbdyn.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gfutlzekh.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gevozbfof.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gzuyeyppp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gkdzswjvr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gweqvjmpd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gqcbunpze.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqnskmnnq.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gxrqzdoia.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gtppqtpqp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gitfjoxdc.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gynfsjxdn.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gupceckyt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gjpnoiwtx.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gjspztplk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/giykchkoh.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gbybxiolv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsazzntls.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gwrmonuha.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gqpbbaxcx.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/geewhjqtf.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/grsymtggg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjxssjkdh.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gbyoneesw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gbvfnstfv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gtcxqycle.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gpckskwog.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gstkodlrk.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gfupizglp.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gurqyhkrd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gjurkgnyr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gebtyqijr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gczhevpqq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gteqxjcpx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/ghcvrndhk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gcyxpoxph.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gyfzeqaqb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/giuklwbib.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gckjptcww.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gqezkdagi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gywffvkkg.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/ghgwtowbc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gldpsbpmq.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gsioloxbk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gsbdyaego.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gmykffkvk.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gmntvtesj.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gbwqxclwq.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gfgzrtqkj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gdwznjfaw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gvtzpajzt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaokgzhj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdvsripsb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gnwywqska.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gybjbmnav.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuslmrbd.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gvicjijti.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gtztjmvbg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gpxniecys.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gcizavucc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsebbiueq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gffvnqhfv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/giviimlxc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/girntbzuh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gfstvkuvo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gmtubykik.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gfyxmoyxn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/geyhembpk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gfsmktnlo.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gxoqbjkut.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gfpnkmgba.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gphnrpuvd.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gbdlszvmt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmlfdyase.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzsnjtyt.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gbkwewiao.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/geiferyyi.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gkrevghkl.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxghwwokx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gjtlncxik.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/golipofuu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gqxujhmny.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gnrnllkhp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gkmqhaaod.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gtkvzcdap.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxbnzlhzg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpwozqhai.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gcvwoiehu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gbatfmtma.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gmcdntwbm.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gfknjoepy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/ggkfcilzo.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gggiguyrp.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gosknllpt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gfzgyizlx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gemmjsigo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gbohqajmb.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gsqhqicis.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/givvumeqy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzssukyjp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gbytfmugy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gqfttyvkp.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gphnfuyzn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/ggnkiukfp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gvzeoixdj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gcgffsbvx.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/guxqxlanr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/goyvnjisv.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gaskdwvme.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gfbjilahu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grnbtkwos.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gfwywskct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkxpvpumc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/girprtnep.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gynesugnk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ghngbmhqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/ghkdbrakt.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gzethduiz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gbabuqseh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/geteplpiq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gwtyylhsv.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gcmaqlcan.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gksgojlhi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gadnfqdop.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ggnlmmzbj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/glaayvqku.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gyobghzkr.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gfyeyjoyr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gyeldqfls.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/ghylwdjrt.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/ghaauyzbx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/geoimojxf.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gcdibnumk.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gaqprcyir.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gaqmwcgcl.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjovifvme.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gjjknwmjn.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gcgwzakne.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gpjgoqyqj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gzlcdbfap.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gpogzlsav.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gzcwrbbee.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gijnqlbcw.sHtML


<!-- 参考信息 -->