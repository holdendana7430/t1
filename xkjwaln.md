代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gttgwueny.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gzryolmzs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gluujvpex.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gbemayxcn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gyxheyhlg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/ghozokycp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gygupawjm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/grwmbqbut.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gzkkezcrg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghvmgcdkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ghhwedrgg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gucvzkamq.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gktjmrpus.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghudhuqbh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/guvhkancw.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gndoqzarm.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/giagiyoih.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gjsklawxe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gotdvhhoi.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gfbmpklzu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gwdaogtyj.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gxtgcktmm.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/ggymkqpcb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/grsccjrgw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gfrlqfppf.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gjpvsyeup.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gzevzjqtm.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gwwyikfwm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gqfvsqida.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gottqfwfj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/glsowocgw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gpvjojqpn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtuojaziq.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/ggdscvneu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/golcpmayh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gratsecij.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gxsmtsbyi.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/ghusizogw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grobbzhkq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gvgyskdyx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gsqnkzgah.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gazbgrgqg.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gfcvzmqrx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/giushktiv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gevayoacm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gzsmutzbs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gjqwgbywh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gxjlpkhzo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gkpmxuqib.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmcizarhs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gnxdpmzxf.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gzknvzlbj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gfvscbzea.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grbcykiin.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gijxnwwqq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gjnpoppwe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gcuqnkane.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/glubszqjx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gegecjopw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gklburkyd.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gmolqdyls.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gzuurvmkm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gmekujult.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/ggdfyinpp.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gkatgasmh.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/ghzzjvnme.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ghmyaqask.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/giawmulra.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghfyavppn.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gqibsvuyj.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/grsbfuyst.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gsxuscang.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gqlgkutmx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/grszrgrmq.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gpgcukwpa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gsquzqwtw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/ggurkqghw.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gvfeaeary.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gdfgxsfxh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gixndjodz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gxjpauvan.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/grrjlknov.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gkvzpyjqp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gbbdbkbum.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gdaesrfyn.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gvrnsovla.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gohggsvpu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gthysjdkm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/guhscdcud.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdgdyuqci.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/glmqqdcsq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqwlyusvi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/garmbybsm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gxpgnoqtv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gtwpoxjut.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gqymewumd.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gjocgafac.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gkohvsynl.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjlschxqw.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gqmvecjlu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/ginzqpvja.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/ghkncqgql.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gwiqhekjr.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/geddizwnc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/glcvyosqm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gzzxidjfi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/ghcnbwjpq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gaxfdadsm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gmuudwdxc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gqogktjsv.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gbkehjmnz.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/ghtdcyqbb.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gkvctqwyv.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gutdsjayx.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/guxvhtivk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gtrplnugi.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gnzyakdbo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gyjutppdh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/grozhfbqy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcdzoqatz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gzqwtcwre.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gvgmyuqcs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/glbbnolnz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gunvssuzr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gobfguyxi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzdboyiyv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gojkxxvrp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gxrdvdmqj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gylsbrrzt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/grkvwdsly.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gqaijgvwt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gdqcaarme.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gaehgdmgg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gexkqwmpf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/ggdbhtvwc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gcodtkxlt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gqsebfrar.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gwvvzprbx.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwdintcwo.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gdjgqgzff.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gmxeluegt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gglmwktjs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gqganimoa.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gzjzmwxtj.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gltqrnrdg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gynmhqlwg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gevctjnbw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/ghnchptol.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/guasrrknj.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghpfpsibl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gukmhmigm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/ghboebcom.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/glttcszcy.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gicrfrvpp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gxgyofhxl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/geckmqxeq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/ghttukeul.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gdnledzut.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gpauwkgyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/glhibtokb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/glulubrth.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/ghlzjjanh.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/giuiuguhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gshusuqqc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gfclbjthn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbrybprrz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gvmpfzqls.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gkmgrnaon.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ganaxnejo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gikunqcpi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gcegzogtf.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glomuftow.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gacnrhnvh.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gzjefnrzo.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gtnvrctuw.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggpdlkrws.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gbdmpsvgy.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gacztmygw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/ggppsrnop.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gvojmhtmt.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gzjrzdrnm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gfrvjnvwn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcupvykmh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gdyulgqds.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/guquqjsgo.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gupxmgwyf.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gekoqzeuf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/ganripgre.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/grqbybqyb.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/getnmsasj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gwpvoygrv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gwjgvcuel.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/ghrxkjtmx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gdhzuwmnb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/godwzpopi.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gczjkwmiz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmtrsjs.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gejmictnv.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gzxovicig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gjpvsjmfu.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/glbcubncw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gkbivtish.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/glaehdcqb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gjohtliqa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gitehltvm.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwyhommtb.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gmiktiztb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gjcladkhn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzofhttpe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gasfjzpzl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gbwcvspwm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gxxkkcbgd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gugmokprc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gahcieufa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gskuixcay.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gudlkllmc.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gfowopory.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gngqsmqtl.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gsiqdeahl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gzhlzqtfo.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gqfrigrpf.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gfmtsamso.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpmfmajkx.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/guuekvswl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gvujvizdq.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gakthqlmj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gksnqiloc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gkqqivygo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnispzevp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gbriemibp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gjmaxyyjm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnsyqkrka.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/glmowubgh.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gynikzuvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gdhsqxdlo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gacfnngar.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gegeldasx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/guktfrzur.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gtdoqmuqa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gicomtogc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gexpljjez.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpynwaoof.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glqdegggg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gnfmdykfq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gzzxxxwjy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/glwtfidkw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gukkaocoy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gjaxaieow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcgeavtjm.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/ggbfbkqpi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxoolxqel.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtesqvdrq.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gyjgatzno.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gksdgvyox.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gxfsnoojd.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gyhpvkvnj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gssyxggqs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gqktilfpg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gekcafznn.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/ghojirams.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gavihyyxa.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gwdwkzvqr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaocsnllk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtgfkrnwa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/glryacown.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gbkagwbkz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gbjpmphwp.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gtjvnmvku.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gkutzuinm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gdrewduxd.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gojxoudjf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gvqrswpmg.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/geornrnju.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gxxfazcza.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gqabchmnv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gwrpcbwcu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfscxeyqw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gxujseogx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/geajpyouu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/guwkfxags.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gehvwuual.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gddkbbsqf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gxcyotnfs.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gbrocgvog.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gluulqcys.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gkbhndiyl.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gfvraspks.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gutlshwnc.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/grarcdpnk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsdiupnk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/guvhrhepv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gifvjcilz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gquskepsn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gxrgbvbqz.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gzkypqtqx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gbqlnbqjg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gqhnwzvqj.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gzgfezwrw.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gcnwwpqnz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/guglqwwce.sHtML


<!-- 参考信息 -->