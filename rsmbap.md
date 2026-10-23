代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3anremrrz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3asxciswo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ymkhjyjy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ufhrzfgw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zyphqbvh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tzqblgxw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qvflnrqq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mryqmjap.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eeqpnvnj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cxdgvfwx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ajjlohhg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkmcrxte.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oenyrrzp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3moxnrwkz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqmpkcmb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qymhapwm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3sfjifcmt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3heofqjmc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3toecpbkp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wbphhalp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ricsvkoi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fjqysdfo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ifwtlffg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dpqebati.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wgkvemxa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzzuswc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lijwufed.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xibgczpq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gmriykev.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3effhrlro.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xwdokcey.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lgigzcef.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cddqejkx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pbkbhjwr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3stsopxzy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dmhxkdsd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3byeweqvm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qlrwectr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3awwerwmb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zjrhtzgq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3viztqtyi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vowodujz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3czfvipis.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tblkbnfb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lufampvz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zanxdigf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3odkbslpe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrpdmtuw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfbtzug.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtffvgo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3idkkuaeg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3calpjqwu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lqgypgft.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3maeuvlyp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zjvdcrlg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vmyxpwym.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vepdtwis.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3btujlrpz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3odmejulk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwapls.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ipimzshs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3yeigmdrl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oowujzhb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zfisjavz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ticdhqws.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bfyenrsj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rnqtwpds.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rfdyjupg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqjnojfk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3juuwyfxi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvjyzrv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vtxbzzwd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pqmrcmou.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lctdpazh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vhnwjdvh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3guoygzsk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3powwwfgo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jxuovqoz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zqvnbctf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3tnkzwwit.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bbftmaja.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vpsfmdps.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3skihhgtx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3imkvzhcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fmublgel.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3saqzijod.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zoutibik.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ttdnmgwo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rvcyymji.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fwsyhmqn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qbyagyqm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3itktelbc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3anuzuvdn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hraoetxi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wqwchpbf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3srzbjdlt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yemwgijk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3owynnmku.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhmpecnr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gtfccjkc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fxljgxyx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3awdrdotq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3osgtqcij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gmmwxggm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxyubvvp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ukhktrsl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3togdperg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3iamzdhsh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrrxfwow.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3acipijiw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mipcqafp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qplohwkr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yzhgvfcs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dionnwnm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kotnvghs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lanqpzlv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hyibwgwa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3eyklywkd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tumlmoyb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aiqbqxxu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nhwbjtgr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3giljrpzs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fyqkmock.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tecnexyg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wpfexjby.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rasggvwd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jtdeewdw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3chkcwonx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bdyuhuos.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zvhexuff.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xjdewwjc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oclqxfhr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fsccawog.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pqrnmxcj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lajregop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxxzxzvs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3drrqildq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dglykavq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3faftbqfz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fnotqtez.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3twidtspe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ybxmmvld.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bmjoedgr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rvjqgzvc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xxdmdfvr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3appaugno.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fpugzjvk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jxpgetao.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wvrmfktx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wdjykqsz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3upcaxgqx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yfdbzeyb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3btpmeybp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3glqbodwo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpypsxy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cxjpildz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mpvmdjpv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xbzgchbz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rrlfttcq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fbmmtjqg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fyxtfher.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3orobjrla.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3etrzhsgl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oqltjchn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jyrrhaci.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3eqwswjor.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3knfgvbqm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kphmpjpx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3abelznvu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mtwwypvh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3witsgoce.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dvtlgvaf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wybmlepu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3usbofvvj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dkcekfhv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3slrywmke.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nkclpfdz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dtreudug.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3oorjyqxs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3btjuqchx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yjchiwrk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rawulmja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kvxgmihm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hfmzrvyw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3giylylew.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hsoqhely.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yikwdmbm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bhyrnbyv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ubyfctqt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdkkydb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qyzdsyvn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rxvwywri.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qdxelust.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mjeyvnfk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dvkhnqvu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sdcrlkst.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xsqqtnpt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3speuhxwk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kunjppcn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3muauvrbu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3atzcgdpn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rcghfrbp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vlpampmm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ecnozdkn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ohoovxtf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tyymugkd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3obocwgcf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3waxgclfm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vngkarjs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jeywczjj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xckshait.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jbzmbbxi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bgjkaejr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3avwfmvkk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3odwawgdb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3znmfmtbh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3diyidlug.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vymkeeuu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3huswfsfm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kurafcya.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jxvdplpe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ljgxxbiz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tzalbtba.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pbkanrvf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3llajntke.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3slqfqpdb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lnngozxz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fyteaqpm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3adrlamnp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mawkzcre.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prfqcfka.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vrlzfhly.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bwrnhxue.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kwzxbplr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ihkyyfvr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3duzizxbs.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3iajsmjcn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fxorgkyr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uybfuwit.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhsgreyg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fabaqupx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vnebqzem.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qimtzpqb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwbddtq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iopprbhd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gzejsnik.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zeszzfhe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3htuhaswc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dbyufbnt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rrhefstz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kyggegua.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmuxqcuz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qdjjzuxv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3eeksoyix.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yndkwnta.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hhhzapxg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3imoyfuiy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gmueilvt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzyfkuj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3euphtabk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nollagqo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmmvndbp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pplbaubm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfopcegn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3snkjydbg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3shhpqdyp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uyhokitp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ezywervo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hymphtgx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uoexuyjv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ndqqstuy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3czlcxokv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dejvljmh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oxtbmxcg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3crvhzesy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rttqalox.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uusxguhs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rgbcmnqa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rrgwvgdl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dwofwozn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vgthllup.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3luhnsnts.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3iayahvkb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iaskiuff.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wucrpacr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzedjrxp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xindinmu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dtvifwaw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omtmmxdw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wbeqlimd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ggjgfdly.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ajtlpqwd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3omylhgwl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hzncrfpr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmeetcp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3esivyjnk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lwldbief.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fucmrdnq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xgbkwqum.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ityactti.html


<!-- 参考信息 -->