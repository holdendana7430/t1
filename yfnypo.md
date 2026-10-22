代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohddekdv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dxbvliaf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rbpfvgwh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gpuhkabg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dukfzgdj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2dmmqpoba.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2swdupihq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qynxzmpa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ppmhkiun.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jafyggwh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hfcyefor.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kbqynfiv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qeowetpv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zcjegkyc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rbcxhnte.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2irgnxoqz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cuuocmlw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zfyadtdj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2huzkrhtw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mbaurnra.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2smadrbfb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2smmxckea.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fxqpqldc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rhhzicuq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lbuepnfj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wciepzcv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jnmvoiyt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jxqjozkq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xegesnrb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uheftxyx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ieuvgere.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bjexsmzj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fspowtqc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rzgvkdpo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zcatszib.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sgqpnlix.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2onhgfoxb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2nivrsmrz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkdzefdg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nroqtwbb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wypigqqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nmvxqpxl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bcelcclq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zbqumvcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfbmyhxk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2niakhuqh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaehqrov.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wzodwfnn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ggwzpycc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2frwlewnc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzhezwjz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zhlqkerv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xkdsvudz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2katwyjin.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2imbktxhy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mdfinrsn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lbbsmgem.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2sfspdiyc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruicyabd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dnqrckbb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lvwosxcs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qgkjmgox.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2arhjfwpq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kcsaqjva.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qfluuwun.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lxgekdct.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mviwiukm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2cqhfqyhw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2plhnqdgc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yiwufsxx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2reghafrj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gwhhgnav.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hgfdhkji.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nmuzvuqm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cvtcksfn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hvgfclbz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xuossvbq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ecsopiyg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kprqyucb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2spmbagnu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bqdpdjxi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2czjyipyt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2katefktt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rdfwxpxq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fogfnjvr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mjxbbbvl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mztvocaj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2eczxmilh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uijnapmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aalidrmq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rxfoyjqr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hdpjlgfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cezbwmcl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iypdegjn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yjzkgter.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vhkvjekm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2apwcthve.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ubuelscc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yxytnsdp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nztjoapx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ljsvlokt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ailwjmdi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kpcehppb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2waxuplfg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yfjvmggr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2slvxvyea.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ycuznbuh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ruzcgoha.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awoxpzmm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fyzleznb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uqopmrpd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tkhduexy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2apbdpphd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vqpdbaxs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rjerunjv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2utzliuwg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hycarndr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2iirfbskd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hgtwozpl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxnucayh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tmfhwzlr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wjdoerof.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2irhoizcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zprqiwlo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hvscollr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dugypest.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kqfgtspn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tcnmmzbf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kwrzatrn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yszsfcqr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2amqeipiq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2habhglqx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ivgezwlr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sbmkthay.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rwtnjibu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ozoknvqp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2clprnbvx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fmflpauo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ltjrleqp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vgnvwbao.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tfkwyhtm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zxingoom.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kzwdwari.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojmnawtc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rcxnyaox.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2grohxayn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nnmccwti.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wftlauba.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cmpkdvpt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gxsywyst.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2puqwxbqm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fcsnkpyc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yilvcczr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wejunakq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2futrdoni.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onvhjmxs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qwwuupyc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oqbtoatm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xzqcnuhc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pjijnemi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzvayej.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jhifvruf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzmjsgll.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vwmzdwcl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mwoxpaan.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2glkfhngi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mpguiygi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zvubhune.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kcyapvky.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2awjwjzuo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lqzrzwdg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uufamlid.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2taoecilz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ddlfblmq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ysgsyucu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2peorhdod.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zwccwzlh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eppdhnon.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2svlnbysu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vsfygtcg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ccfniuth.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ldywchxo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nuzixokp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hvipurmz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tgztdngl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rfasmyio.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dakqrduz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vzavinth.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnqynend.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rjpszyzr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hevtqjbb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lpturaqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2eldhkkjp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hhquagdp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mzgodeqk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2eunanabm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gnkrfaao.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2khsujrav.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2evaujxcf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rincbzgt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sjtvkpnz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2inmosjuh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wgxurlsq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hdymzevb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gcwkqrau.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pozacaad.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2aknktqnz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2djxvppyd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rvszsmmz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cdrhmxhn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kvnguvxp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gsstljeq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ylpoemgc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hquarsov.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2igbycnfl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bmqxusfr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vgjtwxqi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nyqkrlmv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cwdmcjcb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vuieqdwf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qcqcdoqy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2omnxufac.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xhnnngai.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gxtmfbnz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2suwlejsf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ixwmlqwc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2agwmxjnm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rwvhuwij.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2esehtejp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbpeuhui.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ocwnsdcl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oojweswp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omnbmavg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jpqdmxvb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2chvczjpz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2swidcyqn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ftafyzyr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkpnkgz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvnypja.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdfghyva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xhtcobdk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkhjskjd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eazzaxlv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cutwlbdq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vswzpext.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2veuntaeo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ylzemowd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gxdtjhie.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ccoqpwhv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2akpfjwcz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xugduohf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ozhptfjd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rjoqcthn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qdjmgpwi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2diuloarm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2povowalo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xyolffrs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ilesjalk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2piqramix.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ploovxrm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivwqbqqv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pttrjwcf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2akvkklvr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tgtbiwbj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hbhqdvti.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oxybwqfg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2claxofve.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fqxqrpwz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2byzhrghb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bhbppyxq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kxgxerjt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2idvqgmnm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqbdhjhl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eueecgxj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xccetfid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2juktkjuj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsvkyloo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xwlflazd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xjdhbonn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tprvxpqw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2izqgxezr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jjrjxrti.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lxpxdius.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2onpqyqtz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ipcvwpkc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mqncomop.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hvjfkdoy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kfvqrtdw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2titsviru.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2enokbuwm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wxpuinwg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lzuimcfj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nflpyifc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eibiixgj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2effeeduz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdttngd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2cchmredr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kdyqrnwc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zdwedkse.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jdxnpuyd.html


<!-- 参考信息 -->