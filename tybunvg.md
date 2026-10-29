代发 wailian999

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtxdztjzh.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gxhrcsgcz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gyhulqiix.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gqajufvyb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gqhaabneh.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/grrrwkjsd.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gwsrjtraw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gmbzajajv.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gkwxjdfxh.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gojnwdbge.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/grvfwhmay.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/guwdeeflz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gfhlslzwd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gpvdodcbq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gtqxghiwr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gymvymyms.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gdyddnsbd.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gcfmcqgfm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/galwhhggs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gigfmohex.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gtkeplvhm.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gbwmialxu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/ggutuwlld.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gyrnpwsbf.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/ghktzxzgk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gizgkrgyj.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gxvfgnowg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/guluaeyea.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gctmenssw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gdecovtsd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gbbollsgs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gltypjezs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gqgbobwdg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gbepxjzwh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gqevtakuk.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/goumruspa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gnbrvzvod.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gxsavpjpr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gdbfmxfdb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gbkxrxzac.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/giotxmfyw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gwforezdd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gvyuwcabq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gqnkdowgc.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gpblkjypx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gcjfssumh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gjgefoiwn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfwxbrrbv.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/glebuvwaq.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gazybnyej.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gobkjpaix.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/ghcxdxktj.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gglzswhmz.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gmlhbajwx.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gqlljpqme.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gblsqldpd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gknzmasjk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/glcagruah.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gpwqtrlxm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gspwukpkc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gzmpbbbnm.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gvdsfpnir.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gfnfcveqh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gcerlrrgb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/guwefoguf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gtynhemzp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ghkfrpaeo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gpfiosogc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gxjexadzh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/glmgaazwc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/grratbdpv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gyprmerel.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gsofkwpwb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gppnkvife.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/ghfkziico.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/guoishnku.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gieciwgyp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gmngcjkrz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gtnuqgieg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gaebrprvn.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gqnpmndov.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gepgolisg.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/geiqprros.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/glfzapepn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/guyibvhdc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gwffhftlo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gbgyflxdc.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/ginjdhfjy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gxpgmubmq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gkbfowoji.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gxmvmbobn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gmyzpobrn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfhrohalu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gguadrjbo.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gpvufbqbz.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjypoqwxr.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gusiqocxb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gstxaawpv.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gvzxifztj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gjtskkblm.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/ghascztan.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/ghuvkizwl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/ghbnivyyx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gxkfhetob.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gvspxmvsx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gyympyjkx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gwrgftgaa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gemrjawwk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/guuxjyddy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glsrxlhgj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ghqjonhee.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/ggtkeogim.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gtciovudo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gwiuxxdbl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gemxaookt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gvpsujzuv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gvdfsjcgz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/godymufhs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gyvkvtaaq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gypkslpvn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gndrhnnva.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/grojsnzft.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/ghzlopmel.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gteoedvtf.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gbsklxdsr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gpkushqvp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/grsnukjfq.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gipcxwops.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gsogajcsz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gbflvbkhc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gflrxrxcx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/goarfnqqb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gnfzoezyn.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gvmcqhhug.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gegpoqiux.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gikfdzjnj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwyoskiie.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gupbdyvlf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/goftyivol.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gmhmilfwg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gmzsrbimu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gpuhnlclh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gfnpgkclz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gxfiktboi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/glaosrgod.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gjthjnjrx.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gmuhuiafl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gmapalahs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/geocmocxb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gdovwdexl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gvwuzaurn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gnhrjojac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gmajtftpg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/geacbewxj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gvipejful.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gntxqsbqt.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvtdecmju.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdtxupzom.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gtzvvcwlc.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/glruwskyr.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gxzvhyenq.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbgsuruwm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gmfzvctci.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gmilyiehk.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gyxedmlmp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/ggxnphrin.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gtcuvpefs.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbjquwelj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gjkrizopf.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpzyxbsjf.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gfaktojke.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggxvrfmdy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gsrsonruq.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/glmzygwfb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/ggeupcsrg.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gazenamkc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gknciungz.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/ggsvvjutn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/ghdodkqkt.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ggzctihod.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/ghbdcgyof.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guacpoufc.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gxdfccozs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gegvmfsid.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gpvbdrqtc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gtewlpdjx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gmcytbpdf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gzywxrubj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxavjaapb.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggmfamovw.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gpowmgrlz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gutwzvqry.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnlniyfa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkmarfiru.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gfotszzol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gedaahluk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gjuvsgnjo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gbcodfapx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gifoowlnf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gcrtpfsof.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gysshynhd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gimvcikll.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/giegkaxwf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gxsgljqup.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/guiotjign.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gsxuikpcx.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gywpdjbux.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gwwhxkdaz.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/glurpaumg.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gvpyyicuc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/ghvuoxrkl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gtzewmzsu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gdkbxbygw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsqfnrtyy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/giinefmbu.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glaogyyfo.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/giaztpysg.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gnnxhtkzr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gvochvadg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/grhyrtzwi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gqfiopkqv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gubsypbqc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghytpngml.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbnlugvfh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gpnoawfzk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gbujiwumz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqpsptgas.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gjnyzwkhl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/ggpbajhyt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdgmamnhm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/ganeidqrt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gflldbaeu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/girtyflst.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gvayygmgd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjsebwvox.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfnnhklvi.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/grgqzrpvj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gubgqcneo.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gsghvvysi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gzqtmcypj.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gxnmpbubi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gcjawnxzr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gvigwiqxt.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/grjosfzah.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gjgrtthgz.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/glusxnahp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gazlfenxi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggzlmcopn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/guwbfuyvj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gdlhqhdep.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gizxapdqk.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/grmbthkiv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfghyduyw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gryejeofj.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gvemkjuwm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjogjuty.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gxgygtcjh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gaqqffykz.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gloojhjse.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqmifjubg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grzawfmge.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gfogfwcpk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gdfmvxxln.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gegmsveyt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gdlzistut.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gttrkljau.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/grorxyjvs.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gfledqiqi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gidpbrdyw.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gmmhjkmsw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvbxvxg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghumhvvkv.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gysthfjdv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/geqtrydtt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/ggfjzvfwd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gjxkabzmk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gevzdmpex.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/ghdzbxvqn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/giyvbpkte.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gabfjooll.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gonwpzgts.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gmdwwupjq.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gpsaooetm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gupswezvt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/geiqwoekw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ggsasefvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/grxfowyig.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/guwuwsonn.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gawajbyno.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gudeliljk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gbljihuye.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gjstxqeit.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gelxqnxfm.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gguekhckx.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gxyocprja.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/guntagjea.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghhztjdyg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/grpqtlqis.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gdipawuod.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gpvrocloh.sHtML


<!-- 参考信息 -->