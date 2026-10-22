代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylphopnb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cpxmqkea.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hcfmjive.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2egrfshey.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lwofcwgx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2azzrungu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dhrdhnsj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hxsvruig.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxrllsrw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wzrwblld.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrkidoy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jvdvkzvm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ddpfvaeq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zgyanxkb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wxzotkih.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pfkkalvb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xgqrzgng.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pykpyrqw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jvbptxed.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2saqyyimg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kdzuirev.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2opmufsos.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gpteuzau.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2txqwxkzn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xstjgimv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2emesrjqt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bfjtpezr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lhmccixl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2djiwpscf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ualuvsit.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zuvftpxj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vywettwu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2byytvwmf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2thevebyp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cxturupr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yxxmqxoq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ukfptovq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fygsgklf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vdfbarah.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dqydkarb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqsnhpb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xomxpket.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eftlxarg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mrxvfpob.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kzdsfsms.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ocsypybu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccgtywvq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2csylkbtc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yseakfrc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfdtblz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pvvzmvkk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ebkypyeu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kwqryegx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrtqblb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpuojve.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xjnmasvg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwlbbzfq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2inttpjok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nlnbmbwc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hwciptbg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mrjdqsoh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2juhtyegg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rcmivlwz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nwdppyff.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ytfnpyge.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wqmxpekg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uczhmouq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vvfkhveb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kaztzvdn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tkvqemxw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xcfifvqp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2orrqoidy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ihccriaq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ofjdudkh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2qeaplkkq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gaqlrato.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mfcgvcuo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zhqssghx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zbeqqpwg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ovjyxpcq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gyaotugw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lmjdzamk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eocgmaxg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ejrrymsk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ducidula.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vumqxfri.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2selfdnef.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmcybgta.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pnwadrdi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dppdwnwi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qgpnaqtp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wqxygphw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pnoeacrh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gmiabqfu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wlijbrrr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lflylsvw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2afkspffa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xisoxerf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2osdfcheu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nkzaokxf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cmjwrrwj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwdxlflr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xumizhha.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xtanfeog.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hlijzmrz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rwqfkgwd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cbpdzzon.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2udchbegh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2euwojnqj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pnnfavxg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fzkxeaqp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qppiqpnv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rjldfzxb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qqgtphgw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xetcszkr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2frxehknj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdhrzg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2njbwngom.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aogawrxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzougemv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fiiaaznu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvmschzk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cxcmqbpm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yjxknyzq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lkjszzhm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cztuidoj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2oiritfqg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2chvlfsop.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mkubuajc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jzyxrppa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2aaxhfffr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2kkyldpzg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nrhouhzr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ikojpwux.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tdfbxqsd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2luxcjrqc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qubrwfad.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2euzrnqdw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzxnjfs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dictwmxz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hfqhdryx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jdbsdygj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydbkzayw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fnitmnjx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2olclwrrz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ivaeohdk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eslzvpit.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2feiuwjhb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wjxtwhwr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jvsnxzkx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2akkmkhpi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2diprgkxd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2scheepud.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hszmbzad.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2dqiqwnlh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfzhfug.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxwlds.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2crhyrusd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nzgjadwl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wnswfzty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bavlsxsj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2urdnrqck.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2elmnvrme.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2syhwmnve.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ceojynvh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jbegfurw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mmmhtvqj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2koyfpioc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytxoumyx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpdwjytq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2khzurkbt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ycsujhlk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uxcwheje.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xdzyvjpy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ehdrwpza.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2klmfhvbu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eybminbz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nsiyoqvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rlbbvsdk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cpqlrsvu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2imfazquv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qrcfghdw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zufdarpi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lortwubl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rohfgdoj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2anofnhrd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sdiofqny.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2grevcguy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gqrlyhqx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2flridlkf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prqdakyb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bygquiyh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tlrkkhjx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2odcrpncg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2iuxiktrp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mkwyurzr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ooutwmgm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2allnqloj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pzxmdiet.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dwosbubf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlunwrzj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sxkvdnio.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hsloiksc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uaiutriy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2spjagyca.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fzyrmzfs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vhttzwtp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2upgxwzyr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dxudoxet.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2alehlsbn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2znwiattm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2elezbwmz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jarinovg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2roywkqru.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wltnmknf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gzkgtoek.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2avrneevv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2syawtzoq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrxifyvc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pznryoeo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2raiobycv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2elcqekyp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2alcugxas.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ekdftfjr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugndnjid.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bivsjiuw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2togufyoy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2edmjujkc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edordvtk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ohnrfvji.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qqvzpxvu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wrlyioqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2femhzkfl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2afhivibk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mvnfbnvl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gsymoztw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dnhzcjhx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pyogqnnk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2twytzdbz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kvjrafnx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tvkprqdz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cptxyivh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xcxotqrl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2elyjvtsp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rvjajuwa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kyqxjmzt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdznffw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2neuywokj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vsgtrpzs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xcjlsupi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lisqibzx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2orjqfxrz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2srxaqryf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jwifdxnd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wkwdajlv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vcesyhfr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ljtzejbp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kugxvbef.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqdmjxcd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ioasubzp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsbanre.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrgikjq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ntsvbdev.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fcvktyie.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ldeaezll.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2jouluawi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jvzhtwqw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fdlwjufu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmdqksvo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2otzllmvu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fpozqtrl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2konddlib.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcoaycm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xztepaei.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ndssoxok.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hmmewbzr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2taxctxcy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gdnajdze.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oriyplqa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zdqwyszf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zovjzqxh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pjxxzole.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ctdsyftb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuijgxrj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fsetzcnp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uglvrhhq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kjlyykvv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wjbntpee.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hbcgjrij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2sphqxflr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2obsbvroi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rbjwhkxl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tcayxhuj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rhoeeddn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgrtljcg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ybjxsyji.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nrbnqihb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hxtbtzpx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zmawfwfk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2edrznqlb.html


<!-- 参考信息 -->