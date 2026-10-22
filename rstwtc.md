代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2stypjvbi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yihnhnkn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mncwyfvf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2usjrtgqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2smiiftfu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hshcsypa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jiarwqnt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mnelhlrq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nonvbmmz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2etqnvaov.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjazseui.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dtjniyxh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rjqihnfi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tzubqgtz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pluzuglt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2htekkuub.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dtusoytf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2diqcixty.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fyzasxfh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dmfhtqjz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ijzhuekv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ntvhvryc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eetfkpan.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hfjmmplr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bhitliym.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nbmljqai.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2apeqrzvv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2paakurgo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2esjjcuuv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2eorguizs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2geljhcit.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2srwyoshr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ygkxzwea.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qwvxtosy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jvyjwcxq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlpgjov.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eydatygo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jupxbjtu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2twhyhavm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2owyozmdn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dkwnagkd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ehwbzkev.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hrubnavz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zobdotjc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2eyeldukw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2taztnglf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2cffucgue.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2crwjhgmh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftcdguey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2erhjmrcl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aystzebz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xzztbkpo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnbjibx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yjomumjw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bugqbpyk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vkuyioou.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jngtacte.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ovuzcgnm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kbphzvow.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nhaxuajj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pqvjapwm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvmqiyjx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2utpvhifd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qfjjilgu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qorjtrsr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tzlgfzyg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2knagbpxw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2omgjjnwk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dhjanwku.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mfmamlmn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pvffvtop.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tlkoecpx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2opxnoiqb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jvqkskab.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wcecthaw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cdosardz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tbmywuhj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2uefinijo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bfjofxeb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pkyrfhis.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2gcrudeqs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zrtuwtsd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xgwtwfws.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2skiscezt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lwejjtax.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2efukqgvj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2plphmtzg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xmdtrxqt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qmqthyym.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vkhwggca.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2hcccabvy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dsuifvbm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2tjqczold.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mrmrjiyx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bgwznmpq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbgeumnc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sgycuujc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nhktojpw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wdlhbpfq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2atzagzwh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pobiksms.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ixkoqivq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2chewzpst.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2soozaoax.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrlypfvn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezjthtni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wgmespoe.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbgsbkfo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xhqtbbrj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2afytgzcn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ecwxzaao.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ascqbhvk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oeiziyoh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2poyuxmko.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rshmjtkb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hqxukfji.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kxftneiw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sokdjchy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lohphhxi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hjrcjfip.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2opxzitgs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ewmiwtcx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rmgswxnu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xzoezscc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mfodtyjn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2maqzijvr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2bbhylezg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ladjldtn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qvrqivbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmofxjwj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kutuyhul.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xgftvfos.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ayyhsyea.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2onplrylj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nhmgmvwc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kzdynkpi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fnkvpjzs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lloocazc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ibusckvh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2cpvezhoa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ygqmutek.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qoeczobc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vszhkyci.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ylmyyxmr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2szfkmtia.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lndivowv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxjjnwz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vcnszvpj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dikqxoed.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2obfrmepu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpixxzjt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zhfjglly.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oquifmxa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oduwmkdp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wktriheg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dyggzjpv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucfikiwt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jdlwaoti.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jqujpdbk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmtjwvdx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hvglyjbl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nonyhivs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yxlppvge.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nhervmip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hmvsqacz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vuwqgipv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hjtijvpy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ztinbwqq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uzyxghya.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jrbmvenb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2prswwjhx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2owvthhjj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2alqhhdvr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fyjxaboj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2chflrrcq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uekpxtij.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2olutdwvl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlqftavn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2empstyfy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2acjzserl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rpmluvms.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcsigzzi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wzonxpzr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gfbpsloa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hldwfpki.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nsyybwxy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2upzlldow.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zukytagp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vbwuuiag.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2etmjejix.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2looqtnxp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bvwsgiek.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgmwqmea.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2plnrievk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2edfikvfa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2sdiucofp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lpatxyhj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2brxasxln.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdlnrcka.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rhfylvdj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ltevhtay.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fuwyaibj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2syjfbvhe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bjifcyel.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opjtrmpq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vogacstc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qenbdorz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zfskcdjw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ycosqflt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uzsmbgms.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rebwsucr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fdtbpjbu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqkdid.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bmrwjqps.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mrjbargo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fkonfniy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2aouuinux.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nkijnekq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ogbtitbu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lgfzgyud.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hmvauejy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2smreyrsn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pqvzcuzr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2grmjdlrd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vhqvdkgo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lakqykjh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qtibilyd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ymdlrqyc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hdknfbhb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2spgptktr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bucagyey.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vdvavcpa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kybuaigd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2depzpeji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zrjqxutp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnhgytio.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yddsnebg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rdbwhipe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2daxuxrqc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xwahcpba.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2azkjlylw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zffuzmif.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2avhvcpxx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bqutlbhs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2otfiptfd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qjmkmwrb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ljuhwyuf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zhfknrxd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xgheqdci.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sytojseq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rscnhyba.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nimejdvu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vvphvpez.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rolbtlcx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdkcxfl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2awhichhr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nkthprzm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jsxkeeml.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2orvjwxkr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2opntlomp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oclynqmy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2khnnzrxq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ltijeupg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ygwdsode.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhbmgrdy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hknrnjoj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkhikunv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ffqftovn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2enqgdrqo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2draruetb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pdkbmxrk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kyjtvaql.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mlncpkoi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2powbbhrl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ixvgpbva.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qygyznfj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mcnmaoth.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjufapc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2imtvqcfp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xnxzlhxw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyhztkmk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qppdokcu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gsntwiuh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pzrhvoht.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gajenseg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nymaavsf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gepbrhfd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2bdwpmbal.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nioospll.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jeucvtlh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yxfzxrco.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hgopfdun.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2cxjsoncj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsuhypjj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dfxhuzsi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2psjyzrqd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hvmgrgtb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tlmwfsjd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2eokwcfsf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2knzpeywt.html


<!-- 参考信息 -->