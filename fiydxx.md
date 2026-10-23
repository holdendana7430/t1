代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryhsohpz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhjfjzgq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdlgxwsq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uzawqfpu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3huadqpac.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nkzifzhw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yjvicyhz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxcxroqu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vyhxknzj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xkzgxryw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kvuxnoqs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nabqenim.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jjexsiaj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qmuacidk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igqvlfgi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ofxvndxi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3baehxezv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3irpemruf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dhcpfndw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jrjozqvi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3melojxaf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3casjrqne.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3thwjlhey.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3laytqubj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nioicsmk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3eficcdok.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3edehalsq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cautbdjl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hfxftvom.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hgdarnjh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tuxxkhem.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3thtattfv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3haovvmkz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cyugykrs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgciuwj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fmoojxfh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vngselov.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mvjkulrl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3twbiqmsp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3esgdfxtc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kmzynpfh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bqvuuxke.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tregivps.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ntmumncl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rwzsqttr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uuodpyrk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3paincrmr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zpewwtyi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkhslvq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nmnnldde.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hselorym.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tpggchdl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ffbboitr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jpllhyyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3euryfxsz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iqkkovjl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kerkdzpp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3osdqndia.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ybxvslba.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fqwdualk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fhbvdkwi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hndtiovd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3sgatkogd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vqpnfqwx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hpanuowk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pnvwpeys.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hxagqfsw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3yafspilv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dejaixcj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3glvbwrgr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3asxpkscs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rvprqjvw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yzocykub.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3qozkppos.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3naefdziw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ypojuqia.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vjirrarv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vfsxpdml.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zqosgpdq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mhkntbnb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3azuwmkwa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3woutwzol.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xssbiayg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zbigsghp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dfbedxag.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bwbhzdpe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggntnlmg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tojlxarl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3plytiwae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vkecvatl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kzjrjygr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxywlsus.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfueuagw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wlifdlxx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3piomgubd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ucfbahhn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibgpxzll.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qmwhcahv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3matqgjgg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oslgfsdz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ntgywidu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ptfkueya.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jkbjozqh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mekpllgq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zqzgqysa.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bgmddwdh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yvbzpeqh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wwrgsdnc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nszdjyll.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihxvpyqr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xmiicmpm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3spkmivvj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cvleuxmw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qcseegmi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rssonvam.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iwnnuuqo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qhbccrxj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tzgrzyzz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tdykhvvy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gzunwjki.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hreizlyw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bdpurhju.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nsvwspqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slhwtotz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zqdgqdpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spxuetub.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nccncbsh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3aexcroln.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3iekrlfpw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3djlkssce.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aqluwvmr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cvstoriw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rturdasg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mbxuhtpu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dkgwkvid.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fktvzodx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pmnrqade.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3nitjgaff.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bteiszvp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jjbbzslh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3oxhkvcda.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtkiizc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pdbussoe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ugacdiew.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aibfnwnz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjxuspn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vsgfbbhc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bdpbzpmq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3znomecnd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qosarkmd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ugukvkvo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bfbgxzwg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tokvlwca.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uyvjebhz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lhsjqwjg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wsbixgvm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lxxyynnr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xkfezlaq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qpngomrn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3riqfhxmv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3esmnvigi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gixigfih.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nipurpwf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cwxxmtcw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wnbxjfms.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3seifqrpa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3psmdsvli.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nsqngshl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eertqddn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3olizxtdc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xnalwinj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hbvmezbr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3layeoewb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xysupnly.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eucocnfw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3todmwysq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lljkfncm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3grbvmpfa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nwnuppll.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wpvmouhd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3unlvyreu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yqthjigk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mzpakuho.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pqpkfjda.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kbyxeebx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3njazulcn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fjqpdsei.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ksnkitnj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3btgnmxwj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qhhnnckx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zerzddir.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wfmeyiyj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ehpstgur.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zzogrprg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mwhlhjac.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3adkbwljw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lukfdsra.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3drocbftu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mcrxrwxh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hbtsfard.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jvezkuvg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3shcbjbas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tfdpkwmu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hkezkkzo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckoonvhz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vntvvxqo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aazveqyq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mbyzaigg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qjttdilm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkbhrghn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vogoghna.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zlduhskc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3eebxepvo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tvcapzlm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ubzkzlnz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3grhvihsa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3aetegbup.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pmvihpjn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yakmwcgd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ewjiltzg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mzhoaeeh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ceuvmfps.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmqsbke.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nyqeldou.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3thbfaudk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wohhxdah.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ohcphmud.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xknruljo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmizajb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bxiwovur.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wkfsdfgz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oaecuxrr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sodsaskg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ducyyaha.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fisitius.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qegjfizz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehmgdmnf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjjlqhe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gzxttylo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wbfvfnfs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3djnbmpdl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yeolnuun.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmcartfw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3thfwcyjd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3romnrigo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pnukxude.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vylzaigg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byhbgioc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwbuonzf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uucsvihf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgmykisa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ilyejmqk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cbrjozdh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3egyheism.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hbulxzmb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ngpfnjza.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3czoxqzoy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zcbsgllo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pjpjbdaz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xwwnmcnd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ngobhlpv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xdpbgpew.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzujavm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gmmaustk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vavsrjao.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opdlwrqt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3oylcolke.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dbgzfqjy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hcnwnykm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nrakblsu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ubizcwnu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jyuwxkxu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3skalzpjz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghryheay.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlwrpyzl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vqiosrmo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmdzixva.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hvguvyov.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yscaorlf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bobopnko.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ttdwwnei.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rzxpchcp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vtsmxrkr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yrlgzpfx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rhhdvuwl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fdxoceus.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3tbtledwt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nxznjzxr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mqfeovvh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3armshxqd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3avfpjrdy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rptddqsc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xpheceeb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3doglemfq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3oqomkbdf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wcrjvfrv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yxzzzwio.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3opjmhyuw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwhtyyds.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ntytdeun.html


<!-- 参考信息 -->