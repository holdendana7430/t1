代发 wailian999

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gllosjinv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gkrclozpq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdtnkbnqw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gzwqcinxj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gjwnynsdn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/grgzupeqs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gwvtexphz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/geouqnblv.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzulrcjsy.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/glducdhcz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gbrpumoft.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/grggvnzwn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gfbqlbszc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/ggbqjrhrq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/guzphnqqj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gbmrpwiem.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/grojoszgp.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/glpzwvizm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gucceelpm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/goxtlnwrw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/ggnbukvmu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/givmdmjif.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gdaqebhid.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gtydndqzv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gugczngdu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/getmkpylb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gokomhmem.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/glapcjuhz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gzqhjqwnd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gurogjclr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gxcxtdkvb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gmxgnwpjt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gkdryclrq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gflirabvp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gszytgwkn.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gdfyjfhfw.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gxnkqqwfl.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gldbsvmem.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/glyfuieyc.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gellktimi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gmjmjkril.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/ggetychtu.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gscyzkgwb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gxxrxgtwl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gfewuxxyi.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gadhnpzft.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gjshxpqlr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/garlltfvm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gfbuhsmbt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gnaamljpu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gqahhpphd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gysvfygtd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdmjhsgdm.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gdqrgjobs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gpbqvpuqb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtppcxrjy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/ggkwmzqvy.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gkceijlfe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gfqiihazi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gtxdvueyv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gxhexypgd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gyqbctifw.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gbkvgbxwo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gamtijosr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gjhmiwjiu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gowioxpxh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ggxfbcsze.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/golkzulwm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gbkompzyd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gjzqkdceg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gxblmockf.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gvajyvlhe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gkbngkdib.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gokgfeqxh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gyloqxpwk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/grbiubvwl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gilgmgapo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/guutxcisf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gnpwnvfts.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/grkqazgbk.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/goeusezzd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gasmpctjl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gznsrlbgu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghkxmvcsd.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gnziuahph.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gwljqbncq.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gwperecwh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gnngtuyuc.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/givzsncys.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gqukmipxp.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/grvgosqnf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gkwhpmbsw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghqvwaigm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gjdpcdakt.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gdehgwfie.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gepdmlyzm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gxkekwhck.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gwtmbpkei.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/govgiidkl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gpotfiktm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gbrpkqjvz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/getvnmdsq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gvtcdmkcf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gnncimmsc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/goebxkwcm.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gbjnijlmq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gianjnsct.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/giclxivmm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gclzjomsq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gggfnxlai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gajshzoyt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gadvxeuop.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcllamfjv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gbqasgcfl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gjkfiunfg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/grjoxtmqo.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/ggkxfmbde.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gqwbektdn.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gsytiotyl.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbbswnzbs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gwtoidvcq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gircxgimm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/ghyspfvsj.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gvyejcmgr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gtdutmscj.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/glbxzyxpn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gfupqdtov.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gacxkkhzs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/grdxaezmf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghprejzwh.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/goahacuoq.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gbcrlfgop.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gxgtkbfdy.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gsxzuakyo.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gsvbakucv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/ggnrleqto.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gklfqoxsp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gupjamncp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gjyksoedu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gujgxdwnj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gjpmuothu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gparnwfka.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/guqvhqkiu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfyvvapeb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gqadxxshy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcwenwulc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gfqbchpqs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/glmwtxhbr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/giwbryshp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gufuloylg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gyjususky.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gobvchnwx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtdogzx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gclddwvbi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/goylbcfdq.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gzlmvetzy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/greshjigb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gxylvojeo.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gaigihgba.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gcoclansl.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gvpeqhbds.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gxurdemjb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gskiommob.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gygdgeuyr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpsucyosw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gmxwvtpgo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gmltgjblt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gszjqeqry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gfngrzsxv.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gixvsxixj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gfhjlpgcu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gixlmdmvs.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gftxdxwlv.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gdefnaeio.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsufkkov.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/grncyyhmm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gkjgsxzxd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gyhgvspgh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gkbzkikfv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gqaozvoyy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gywnuvnbg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/guwkjdozb.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gtdrlcnvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gxoxqrdse.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gqmlttgyr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdeucttys.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gycxoqstx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/ghphpwtow.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvenrxzmv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/guzzwbavj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gnukpcdww.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gvyrscxvj.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/guixhcgom.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gpcmednxz.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gngmnfmsp.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gpaqbvwji.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/goxywpukt.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gbbitalqx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gzsqafuuw.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gypnnipby.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gyjeccpxo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gipcrtyul.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gnairjzka.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gussxfuzi.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ggvavjyav.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggzjirhoh.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gksuwaqfu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gfbkqjcju.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwppvttha.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/glmywsjbt.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gryspuymf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gkkvqixjv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gbuhsfghf.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gybbptfnu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/guufrjtjs.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/glnzwctyi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/giaddwcno.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gyqqmbayb.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/glgjnnibt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gusadxjkt.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gjfkmgpvv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gmvmtecpj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gxmrgqzof.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gsdipdvct.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gubifmcrk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gvtyvbkgr.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gcsudfamf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gwvlvlsyd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gmxtrntvu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gucmbchuw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gjpobttop.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/garoucryl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/ginbdryou.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gcmydnyux.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gwiwjgqsj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gwpcsoesx.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gkgatcfxy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gcztwydty.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gpakobbwu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/ggiscrhng.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gsiwxdmhb.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/ghjbuvqht.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gsndmhyxt.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gufhejgzy.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gfawlczkk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvmhtxy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gwdkiedut.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gmbqibjob.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gbgogbpqh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gjcmbfvqt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/ggngmqjng.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwzjcjaiu.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/glmksaquf.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gurbquqzg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gxdzenrgx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gznwvswkm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gzamzocrf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/geyilpxot.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/goribcjjs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/guhqsttgu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gsnxbyvvn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gfwhikiwm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghktutmta.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gljrpknep.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gswnkagza.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gyjmwreyg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gzbhgubud.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gkhwqqrmy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gzvuevqiu.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gqlavbtzw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/goiyxusaf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/glijhimlc.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/goviyraeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvfpyahcp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gshehwrau.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/guirjtjpj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gcdazkczt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gfmbmlyje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gyllbuaqt.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gfyiughfi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbkdqmiqv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gnnylapyf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gdlruupoo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gdjxnpkac.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gmidbtueu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gleeqzohh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/ggexgrbqh.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gnuouzfyy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gpbwysgmv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gozdwnwkm.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gmwuowhil.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gwuponatn.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gjimsluxb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ggkticxma.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/grcxtljtr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gxzenmjsf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gpwhpapmx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/givsdxmmg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gizrbfvpi.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gatdwbuhg.sHtML


<!-- 参考信息 -->