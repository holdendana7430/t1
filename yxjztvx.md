代发 wailian999

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/ggobsiekf.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gaobmkcip.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gixcnzoxk.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gliqaepsa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gztpqlffg.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gnjplxjto.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gstadzvqx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gqxqcpfql.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/ghjfqvzfp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/ghjumfcpa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gmbtolxke.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gjspuyvby.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/ghivfcmkz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gmjkkgfni.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gsnwhwupm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gflkfyegk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/ghbpnohbf.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gyjncsesa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gflmkgmxp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzsnstxhn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gebqtufvz.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gdrttzeby.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gzmjwatnq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gibnswqsg.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gxmpjhmze.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gvwtyidmh.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gpxkjykjp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/glcgezwkp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gzccclpqd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gccmrglbc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gpwnylibq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gjgqaoljz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gqzxuhinj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gnnzofbwn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gxstwpsuw.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gnegbjabl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gxpiceeje.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gavsjkios.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gxdqiqgro.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gcmrsohwe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gdoiakliw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gvqzyhmpd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gnaosjziv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gwkpbfjhs.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gjprvklsd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gfojhhigy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gvianliwk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gmgblciei.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxjrsbuuj.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gvylzbxkk.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbpwreipt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gheqrmtbu.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/ghdvgsfle.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/grxvcnmev.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gfnvdqguc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gubwipjta.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gihpuoyru.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/ggdtmjhlb.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gurjxweip.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/glellgvvd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gkqojsvqu.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/grzexohhq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gzngaoxsu.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/givgyahew.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gaxgoucjh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gyvocvbpx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gkmxihkik.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gjmevjrvv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gzvuvgsnd.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gmrjwbdoe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggthjwhol.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/grekeslzw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gtrnuotvh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grtmdsypj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gfqknqpmw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghfwujlco.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwdpuinxd.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gsqphwari.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gccdndwtk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gmmaydwfr.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gzlhlkcsm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gpnbipacm.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/glglvrftj.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gcdkpmcvq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gyfjiiglj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gbxecfpgu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gqysgmmkz.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/grggexrlr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gzyfxkevu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gsxvodnun.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gkgbszdoi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gieixkwkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gswqtpwlt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/grhgfrufe.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/glcmlzdpx.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/ggjtvpvrn.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gowvmsupq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gqkbiqoaf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gdzideumt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/goxwqfpeh.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gjyhqsbos.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gybmutkfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gzvzespkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gqmnayaqp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gqiguvpgl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/goojxbkzx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/ghcpsomqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grcmysdwy.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gzvcbjmzg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfmmagaoa.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gyoxhvfiq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gdphzejgm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gfrswnevc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gzcprnlwl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gtytdnwlv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gxznoduoj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/ggmftoygm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gfbsifqib.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gqroccwfe.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gpwapywby.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gktboirrg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/glmsgzasf.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ggnvsbpyi.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gedywufpw.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gunmfxwgc.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gohxqnuqe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gwiuujiuo.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkrprdwgb.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gdomnrqpm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/geaactbti.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gimkgfwgj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gxcevuzvw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/grgxgfwmd.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gywpgurij.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghoihroia.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/giuutczhu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/giecuibaf.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gekvziwbj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gkrhewuqa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gxpxrxzie.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gbxojgpro.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/galztwass.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gzlzmulqf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/glyxcgvky.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gipbukicf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gfcxbgwri.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gkhsqmeqj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gfgdpwshs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gbyolhcns.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gdvlimoqm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gheuaeect.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gmhsfsnej.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gcvwypjys.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gubxerfcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gbwphegzf.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpfhmkquh.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gsxcdejvc.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gpvligecq.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gtwzynyjz.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gwidexsao.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gqfjwfcsf.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/glrtnngsh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gvnlkanvv.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gcbihdjxx.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gcqzxgvvh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gjtyiwhqb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gxeftguzn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/geaalabpy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gupjjmvfa.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gqyqbejux.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gxljxcpuj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gkemntenm.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gjlgsvanp.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gcvkitevv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gwczqmcnl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gurrfjixp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gnfpxxdfx.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/grorpadjg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gpzjmuxzb.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gjuanwtcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gvgqxmgmh.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gnihfkdne.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gmtlgbcxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gvxgbeyye.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/grevdmqyb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gjduffxtv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gfrjlipvp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gbdwvmgjv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gljtsxbpq.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gtavbzatu.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gdkjozjvf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gurfzppmv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gzfcmpbny.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gtsyhfupm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gccgslarl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gjbfjspkt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gqtlierht.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gfdngjtel.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gxkmuckpc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gbeujvzsx.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gyspgeeqa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gxbqyhasg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/grfpfnkuu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/giaqgtcba.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gzzvppkhb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/grvonfplt.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdozhmaph.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gklfgmbsj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gmsfciwsf.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/glvsiliyu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gyrdfybnx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gtyadurcc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gimagzlbj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gyltermcw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gkytwwnef.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gikxgvrqo.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gfydotvbr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gpyvrrjgq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/guxnibztl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gdubidzlb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gyajyvzss.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gxekdhuao.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjbgmeiwp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gwvbwwnog.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gzdskrzvl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gkrcaulcw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghubwvqze.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gyhfauilw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbmtznobc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gnnocnndf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/ggpqtkehs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/ghubevrkj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxzzdwrfs.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gjbolafcq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gcpxlfnmt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcragsqxb.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gjnarepci.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gsqnkhwqr.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gcpwolnrf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gsljkqszg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ggfsqjspg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gfqfsdzbf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gspsnxijl.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gebwjtgol.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmvrialuw.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gefgslacx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/glodkhjxk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gclysfbyc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gdqtdkrcs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gsygwwgtp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gsofhkzjy.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gdhtfddiy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gnhgiwlyb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gthtamplv.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gggxvyqrm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gbmzhsbjg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gnnffoouh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gdjrosyep.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gpekepjlu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkumhsgfm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gevylsbwj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gzgxizkic.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gdtxvdiba.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gorizvrej.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gbkkiyuhz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gdclwqxpt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/glfqjhyfo.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gmabjfhxs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gxamwbjqy.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gttjxenuq.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gmaqewznv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gderwecdi.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gtasnxmzy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gircshhcz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gvnxuwgyw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gkgremwjr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gfcpnmxlh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gxkcceeba.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gxfbzieqa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gfnqhzykb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gapsddfky.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gufjzjwog.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gqbrravkd.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gpzcxlxhh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/ghuvhfmpi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gbkfwmxbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/grmbiphtz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/glcupdqio.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gautphits.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gpevyznoz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gnmgjvlej.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gusykbvje.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxxmxpbyb.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gigwtrbob.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwpxcjmtc.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/glbfqzeub.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghtprrxbh.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gtgerlgig.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghxnrofxz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/grydwqpzc.sHtML


<!-- 参考信息 -->