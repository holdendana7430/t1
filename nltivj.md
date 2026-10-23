代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uawrqqku.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vkqshksy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eyxhoqaw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xxrevpga.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bztxmdsy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zclyqcfu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xdhpjuau.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kmxqkrud.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tgeuslfe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uqetomop.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ksyexhaf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nqdjizvi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ldfediwc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fhqwndwm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qohnmzow.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fllhdijt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nplhznew.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3advocaxx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3frvfdjeh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ziscaajk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pzzcadga.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpwaebe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fdahaokm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3phrxilke.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3horbjwsk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3firliits.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rwcwnmcj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3idgpsbox.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hxruskok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cypynwgb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lbylqlfx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rvntjqaa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ymutjyzh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcqksnvx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ytambgtf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kjsncnpw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xumbyqbs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3czuwrcty.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gblktytn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xpmtqpnz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uprnyqrg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrxaclq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fcunocky.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jeblmmsg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vxocxrye.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gvwrrnlv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tnkimpkh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ljozjzyc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3klsgmzya.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cwolmzkp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mpcqiuuf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hwgticbv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vtfiviaj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vlfoobhd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3iyrdxhwl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3konquuux.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pgscxsco.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oagcmkan.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wqgvvmee.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ckkrosiq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vkcwubag.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xhujgpoq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dwmvemhl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qflxmyev.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pnsejqqa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3udesahpj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3clqrehhz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fyyzegea.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lmqddqip.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3avlivgwb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzxknvro.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fpwqqziv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qkxtoxdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qktaxpwn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3navijrop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueckyknc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mczwcusv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gurwqycf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3spmxojwp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wkbomrcx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dlpecudk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jxkxevxc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3caodueqt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jouljgtq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqlkvhq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wnzcptds.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zczhbcfv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3esvsrrap.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xvungwsx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfjodgui.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3goqfuwrz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mcfzokht.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chyiarrc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efaffpzm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ltgjjywz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jrdjxnvn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3clujevfb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lsmxwxpb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vnlhlatt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nbxinych.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3aucsrhcw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xkcmvosy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ylktieoo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hhxlzsnd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3diidfewx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wlrlufhv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekxqbbee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juxmbvqw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sfrkxxns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqplnfvy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aimzmyuu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gsfoween.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hbbizlfh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vszxukkb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3cmcadgag.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zlbcjamf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3acoguimo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jflfuwfp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jkukqgxn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hedxagla.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uyguovpv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gfkbekhv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ruliwowp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qqvgbelf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iabzguju.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zphfushq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qbabbiqd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3frpeteog.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mqjsiecp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hplftjnz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3idftihkb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lbrucadp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmjgawo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akjplbcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ngncgkin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zxfsugiu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bcicbabu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ljiudkgj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vbbhhetc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lezutrop.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ggmrdwxl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rnzlqxwv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uvjiqtba.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jutdpqpe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rvpaqjdb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cbpeaeso.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hadqeufw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3knmqpnvn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eszhrzpr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3whploidx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3duoxzuqu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3doafzbiy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ukygmbno.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mtmiydwg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3trpkawnm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nssgdviy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxewmnx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3szkuebhz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jspqxolr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3crjsyzvp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wuemwazd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fulleidi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3swrnbjgl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mttludgy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hhpttyev.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fljymwaw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ymonaira.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxftdzfi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3joyexkkg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hatvncrj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kocyxdtw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zsdxmynj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nqoczvqo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wvqbhgvv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfhmarv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xgfvaorv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qguchghq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gnmuzghc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lpbtldwo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fzmzlxlg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tyulineb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oiydjptx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jvuvfjql.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sepzgeqe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mifeptre.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mxcsfpcw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ipetijem.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rtlcfsre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3btpzuhdx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xpiyccgv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zrhdzdtb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3igbqyoda.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxeddad.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgbxbpl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sfjpqfch.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3okbgwzpx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sbsejgyj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3thxmjrqb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rqumjorx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mqfojkok.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvcbdtdn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3htvceddo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfscacjs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mpdzksrq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jsjtyxds.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eglgpsdu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwxedxp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mhnxypoe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dqerkrva.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zzpgdkbl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hgkudyez.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lskgjrxd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mmejvgbx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkajjqas.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gguxwijy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fifzsegr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vetozzro.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rpduydsv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ilpucezl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ndkdchan.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iuptpzmg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mgodjqpk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxjxjea.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tsjzahpb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3snknhddp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmeujemo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ucuwmqiv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dsarixtu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gwaxnjqh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdufyuei.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wvxoyjsm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3puvoxkdj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xljxsodm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cnihejdo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qxhgguqj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjfgpane.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gzxmxlla.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wzvdsqnb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3docjytko.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ibmcyjsh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vvhnyonc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3psvmeajc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zmstcnfs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zmeyyoll.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uyazfnye.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xxpamfdp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gsumdefl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hodioxmw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwdhytdw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jvceyttp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zsxobofx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ifegtzum.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3exnjaxni.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zhvsznsz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xsqrfrcs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ofonrejm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3amzkciby.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nteqyrwf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wjnxnafb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3shcgycdr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3addqiazf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nmxqigdr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wpvvvorr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qlcskfxj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gmlynsrn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3efagntiy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mpicwemw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3effylrfv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtzjogac.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qknifahg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ppsddxbj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlmhrhfn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xzkajnuc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxyahslm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mrrqpmvn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fhfrklsk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhzvezc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hhjnesir.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bmhgdxgt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ntrplioe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kpoqpyje.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ayvqsgme.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdsotma.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxnkjzss.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dzwgbfzi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qiockroe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lmespdbi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ffuyshtg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rcgreexv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kzkdxvbd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yshecfxd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qagkgptu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zkwrivok.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dvdbdkvd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mucwwvjx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ocqtmsxy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xfswdzqp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edshcwmb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ujkeaojw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hrolmmdu.html


<!-- 参考信息 -->