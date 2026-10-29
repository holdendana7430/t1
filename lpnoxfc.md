代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gkqrcuzvf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/grmisbtfh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gryvputbq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gupbgvutc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gkqfetmyw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/ghwatowgs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gnhnmfcbd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/geswzqxip.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gbzllfsum.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gmijmrszc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gcjvqubpt.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gdoifqyic.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/geoxtghvz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gftrtizlh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gxgyoycws.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gieehlcjj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/guygmmjlj.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/ggolruutp.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gkrdzusxm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gxaujvwin.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gwyvsnywa.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gppuucjkb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gjncgwnfu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvmumuxro.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcugxzycq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/glllvauew.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gnnwcndmd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gsdrvlybo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gkiwidfiz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gywbztlkg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gdihdjmif.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gvsgdgriw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gxnvehqxs.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/ggsvxxwso.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gytbioift.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gcismmisg.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gjktqiuff.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gpejwqemk.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gkewncmxp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gurkykxej.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gemswthzl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gqxullanf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gjkpdhhqz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gdbsployw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gyqtlkybx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gvduqrpzs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gojrobvuw.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/ghkgbtrqe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gygksooyb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gtoeobygj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gspkzanxr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gkzqwhtaf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gusakdvzp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gvxbupzfa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/grpdpgmct.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/glsoxixiq.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gibthglso.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ghlidfkoj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gikpwfqmd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gpwydtwqh.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gbaouwaba.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gqwsgxlia.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gapcbiqee.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gvkfwbntq.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjqpqtpjf.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gavvvruun.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gijmbkrle.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gcwfxbhzx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/ggmmbjixy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gltboppkz.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gsuguvlwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gqtyoewdb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gpmahxycp.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gnhtmarmr.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gnbbtlfiy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gelloornq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gjrpoeugl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gihndlvmu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gfyukpmvm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gblnoawiq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gsrscsrbk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gtxnlzrrb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gchmosquk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/ggwckzqli.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gepekelts.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ginudbkrp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gquwgqbrv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gmqaqjobx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqzifxogy.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gknbmvkcw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gkrmvvwhq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/grlwxftql.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/ghcgqqyul.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gdjxgifvg.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdanplcei.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/glghilpjo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/guchgyomn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gkyxinatb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gpzpdjqzo.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gvswyyngl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gzerzfxux.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gzvmgbvqb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gyxrkxhbk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gsloyglxx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/geynkbtbp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/ggydtpges.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gmtpatqkb.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/ggqmvxijq.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gbfswzpoy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gaadnokxm.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gejyoddaz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gukihzgpc.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gwudjxvaa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gukytsrlr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gieykqibi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gptkrzcpl.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gibzzckjb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gcxuuhaxu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gobtvfasw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxkqtflxc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/ggljsucnl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbjwvtzcq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/ghiggknao.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gdaoinjez.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gtazbhqfi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gdsjxwmtk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/ghpeepdpu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/graamhpxa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/grdsssvsc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gfkqfjogs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gzgtkmjtf.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gbbdpzmjo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/glxkxezqh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzosrqas.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gopkoosqm.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gtoqjafqh.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/ggapxvqwc.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gdjbjzxer.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gnargmhji.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gzcguubqv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gzqrolqmg.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gxwnychng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gfwgmbgzb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gtfrsqhjv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/ggewktcqa.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gytxdxwex.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gmfvbllxq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gjyxdffrg.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtegbjyio.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtbkyzoli.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gvxkqlwhg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gujuhpehr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gcakptyzi.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gnbtwmjhc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gztthlxxm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/giufzntat.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gjmdgtbqv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gchdvzjwi.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gfbeljooh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grrdqxues.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxoluhsdq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gmdbrxixc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gsicbcpri.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gloikpgtt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gxaqqunyp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grfnlfwtq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gfflvfgpk.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/glxsndrbb.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ghfeixgwk.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gdmkbmhts.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gmgwlhvvw.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gxwpiblny.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gdkhvbehq.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcarlzenp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gaxdqthlr.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gmrengbgw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gadxqcpqd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gyxygjoxt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gmhzzqstj.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtosjciqi.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gyfsldhli.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gqsaptpxu.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/grtdcsegg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gosacjihq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfekoppgg.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/glpykndbe.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gzjkhyxlf.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gzzxtndjg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gpghfntmn.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/giicdxnkh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gybpyqidm.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gqwstszla.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gsjmmtnry.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gyqpddswk.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gwvmotmdy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gkxqmgzln.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gpyqaqfjv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gyqwpynbg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gxsxabuft.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gybfdhsdc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghbkruxot.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/ghhevvtmx.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gesxhmgad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gfcfgupsx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gzzkrtgby.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gsgdgjkml.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gkkuluoxq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gulhwooqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gbyengcqk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gmxjqraxj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gufttinst.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gadtzwcrl.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gcwfxonyl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gscqkcdaq.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guvpdmxbm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gdbvpvvxw.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/glxnnlzfl.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/ghoqjalik.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/glmzusdow.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/givwaduid.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gwkjupmwj.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gtoudwnbb.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/ggecngozz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/ggacuouis.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gabmydggc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gakrubhbe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/guuwqzprb.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpvlikqrj.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/giefnplcw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gtkczpkkd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gxhrgumbg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbshfesof.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gukaehdsw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/guznrfnne.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/glagrqaqa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gdelwktie.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gplsxnjdx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gfmorvlpo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gfkopcofr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gergfctrv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gasdpyxgk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gkvmwahzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gsomqhicp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gakwcvvjl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gldnmqzhn.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gfjgvtwkd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gcxicrrtm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbiczsglo.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/ghggfheqv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/grohatrxj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gdjmrbsxd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gwlanarqe.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gprcpcqyy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gmqmlonko.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/grgpykzyf.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gbjfdatga.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/grqbadibf.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gshbqcyzc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gmecwcemg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmfufpglr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gsxoomgvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gaimwkfiq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gxxwnbpxb.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gfttlvgjf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/grukuxdci.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gprfilqkx.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gicjjxazr.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gilogvham.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gpnasjpuz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gehwtupjp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzasnjmkm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gvfnirapd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gvqtowfrp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ghpgwueid.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/goobuwlgd.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gctdlxhpg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gvojmnykx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gqkieurjd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gyylwuvoo.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gizgvhowl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gfldkbxrb.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/ghiolyhiw.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gmgeqwbzk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gyyoptgjl.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gualdpxet.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/glylverpc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gfdjukxyr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/giblinllr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/grhsunsqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gpxknkepi.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gcfjoaygn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gtotxcnda.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gotulypma.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gzfujoizy.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gyccjornv.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjijhlodf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gmnwukatu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gabtwfjdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/glgvkqktm.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gmmoasxho.sHtML


<!-- 参考信息 -->