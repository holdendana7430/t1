代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hybntwcv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gsusqhda.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3uqoyvpvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pcyuhjbb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzekxlpr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yngcaodi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3leizfyry.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3soxvryqd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kytmqyhc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wbosqpjm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bneugzsx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qaycsubj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmyefkeu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qkcwomja.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ddwgfhju.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xvfadndi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jxwfpyki.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uwidhysx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mccxwlfi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mfjynthq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pafkiyjt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kbyciobs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vtrvsand.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nhyyrqpx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xgmdhzwu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3scvlkebq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3kdqtxwqc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3drhkhchp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nkhaiqme.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tsaqqots.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3sdvruueu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3euivehnd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ezmliuqe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3chrtkyoh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fcbmxmtb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3itdpfygm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wuhgeguj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yfydphec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3licxzenk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emlvnooq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kzpqchnx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjjrxqu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3buushjxr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zjqxrtxp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3myvxorvx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3enrcfvar.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3voimccas.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pegitkdt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xeehxvvs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tungtifk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vztmdhxd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ubzfqyor.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gxdfexlv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxvuaasw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zklcispa.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qlbvrksw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3swkfaljq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wwtdwbqi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fzdczeuf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ewetmryk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mrnzishc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xjpxixny.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdhhebd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hvpdrxzd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bgnyyzph.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3renpswbd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ollozcwi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3foesuhea.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qxhnbvag.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sbqaivuu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zogzqqyx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kmjlnoyj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ctrpcxlp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lapretrx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ziyabidj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kopktrbs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pttarmss.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jwichwoc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nevthani.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rmruahqq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mncfqfaw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vafolwsg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3khfiwllv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3whqdfreu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fnywgnxg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fyxswdjt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ovzikvbn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uvlqjfsu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3byktrxwm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3apvgccyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ovvnfxoi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3grtnpsub.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zwbfuvug.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hdwntndj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ltqillth.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmymioio.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bqwlomil.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fstkvaev.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jgjmwsog.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hlfgehlx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ptpsehvn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3umnlqqhr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uyhnlqdl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3juwqerdk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gumgvrmb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lauphhoe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hocxeewc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lbdmgaol.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3herwzejq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3howuxexa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3aikvrfjw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wttjjpuf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lesbgtvk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqjclyeh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3injsjddg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3doguynge.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cszjjdex.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kqmoebrm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zhgwssre.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yhxtzubg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ohgqodez.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xpotdied.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cpnwhjhz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qmamqfyd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xpeytfbp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3uxvbnboc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfbkolfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etnpywty.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pbfrhpxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgnpuxuc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3alfzbzjr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3iibmlprp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ksmkypgt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fdnsqgmp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yyddygxb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ubbpbame.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3plyycogq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3runqtlgj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qtqcwhzn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jflvoneg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qurckpnl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qhmzwdfe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yvgioshd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nxyczwqb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdhurbxg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sfguuxlc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3blrtjyhi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kidkbgip.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xodntbpe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hzyszzbj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rkwdabws.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hyitgnod.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ssleznip.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvglojs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pnvotrpk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fgyxglit.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlqlvwqk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fykarxbk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dguwozjy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqbnjmhv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3yrwyxoag.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fhxauspn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yjwapdnf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mfsvhksy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3emdtxmfr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qrxmsjgr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mclkvixa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dulqhxmy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gdqknraw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nowubbqg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kmqszfvz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvcpmzl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lfelwvoo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mwcfqiyd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xqvylzrk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uzhnfzhb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bymckfsp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rndybvvv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zqgrqhws.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kshpvqsz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3utwusnmb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3frpvdnwx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xnosjdwj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mlklmjvj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xelvxnkt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qsoauxqi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zwgkcplh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sajiybnd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zcssgjxy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rivrpidp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xgmoyqwq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tcjdsodh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wqygmaki.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wspspjqp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qauevuip.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qwcxwpon.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nhjtgqjt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ginazrip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kolggsne.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3suuryvyd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qelbgvie.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sewgndwo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3utqfuobt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bhkpltvs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zjezpqca.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aurhuxrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmpzjrg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3skcqiuhz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phrkmzfc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mppqmhpj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3acctqbrt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ydycffcu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lxewzadc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bakosuzp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3aspeyeeh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cqeifuqs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3brdxpkwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hjzmyxby.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3khhicxhs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yrymafmb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hampmwce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cewgxpwj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njftmtff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3idrwzsdn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3etslqtzh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ypzblbuo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3beippssp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yqlkgbhb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xinbmxor.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3krehiiwy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nszlyneh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ctfvmdoh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yxsytqyr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tcnroqjj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bkqcjhqv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tofrpalk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfsmunzq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ndjqlyva.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jempfzvn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jrobrdgm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3usgigtda.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywnkoydo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyqlyzc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdyevqyc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mactowcq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wpprmcjc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsukvbqe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xkqnvaqi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zbgmewwn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3grsfozja.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcdshbf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lpcokxoe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fzwwdkrm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yikehdak.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xwkwbtfk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qmscgruj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3olynkfem.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qyvxmuvt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bfciytyc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nchwqsby.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3acgnrrno.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lpbuseaa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lsvseiti.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3iygxqtdh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3izmophnd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3memolygz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yejxcajy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ancibipl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkhaybp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cxqxqshx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3txisvfgr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vkbeogws.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tzaetegs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dhcdktzq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uehkbcxg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxgxvtpd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egfdpizu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqyxnxs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ayjjgtjb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3iikblktb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewywwqlm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hfbjvkfi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aqbfscmd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zcbdbojo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ohbjylub.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3asginrhi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jbdisfnd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3eodqcevt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3umujsrun.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3krttqoef.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3yhvkdjxq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jjhxeajj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hrguvngc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3sbfxsbpd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mlfvzlek.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hxsgbzcq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3arpdlybw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fcmhkokb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3flpyhmyn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wrbgkmbt.html


<!-- 参考信息 -->