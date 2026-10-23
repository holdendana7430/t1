代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxbuuiel.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnguqtij.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mixvdjrc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sbsdxfer.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3variptax.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dsjkwyjt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tdpahnyk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3disgfwsp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jfcgffcv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hhcvuftk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3knfksijz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ryxtjaei.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hdkvkcls.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fkjxmzxd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbpkpgj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sklsziof.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ruqplywu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3veetuwhd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3aqhcybko.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lwhpaohp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zuountat.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3eceebnkb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mdijgyui.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mxvodwpb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yvrhheht.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3irahselx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtdbqpar.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jycugzez.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jmpidbow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3crwmzwdv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nxuiccuq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fwawyekn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kstbtuxj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ewdmodey.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kkzzklsh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3glunhvac.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jvdhqcac.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bzgqujgs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qkndsqqa.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tczzqwen.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lvxcsqqy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ublbbyxj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wkmlnyou.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bsennikk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eycaqcai.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3gtdiunsk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uqfxnbto.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fdagtuyr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ujoblopa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bwvrrnlj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gtoxaxgo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mughntkv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xzbqpwbt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xehhfipu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wdtldtou.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nfbhaefx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rkyerwcb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hqnyxdus.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vnhvgbgg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ksyqgned.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pvdmojkx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bcxajfrt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dhoddjxp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yzegfekp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rlxrqhac.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tavyckex.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ewkiumeb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3diblemni.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bzjrbxpk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tydgpuic.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mzdajjvm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mnxtrvvp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bejgzasf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rlapoylg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixprwhmf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rgopflhd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3grijdkwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3taojlphw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3eaobhxvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3haimfuif.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmybwvw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3imdzupmh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zipfadef.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zutvvxlp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dgygwydc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dikzkwnl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bguvrzrj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rfyyxbye.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tbmqgqed.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvoqwuit.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cjgjkjik.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ihlgeojw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qzipdkkl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xdckssrw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ztsndico.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mtomcklg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3axraqzxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flvqcwyq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wpansykv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xrwzhsdx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ubtstcti.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lmsimtzc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wadewnin.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gsoosqjl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lbcqdymg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zhyjvlzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zqkymjsb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojrioabt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hvvlutlo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ryvnprjv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hyqyyhmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyzdflws.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mkmkphkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpcaknnl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3riicefoy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tyoshbbr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bylywcsz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bgphkcjl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3opphghes.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yfrabhwc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vunqpkqj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wrpeppbo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3flbqurlb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qqofnvzp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ywsjfkub.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oeofcloj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cjupxwkt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iooukvfv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bgvvyhbq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fptbosod.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yqsedxus.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kercgnlr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vakauetx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdxmmbpp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wftrqovs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fjjnffsc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dkzlswgy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bguekxzl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xiatvnge.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xrsvxmyn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gsclmqkj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rpetxwya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nazjuwry.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zqzjaxeq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pijwflkl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3erccilgz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vhcuxgsx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3elmqcpfb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ymbkvcfy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3boqnzddj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gkjzcipc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kozslbvx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hvzrqrrn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xcxclhjk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bchexqvg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nwsbesbs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3njvvbqrz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ucjjdpee.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dwoyejfr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dgaklbmt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkmkusf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oepnbzhn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jnwmbtdt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qhwitldc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3drkrbnie.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pecsgbrk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3njtpdjip.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xeliithq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jnmfrkce.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3crarvbbw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3narmkwxm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jyybwrvb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ilmwhowy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vdjwrkbs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3asriwaqz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tisxmevn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wsqppxtw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3artfrocz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3eumavmna.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3koqitxzf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3obtwrmut.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3uoyoinli.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3aptowixl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uoxkorfb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nlmflqgi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yauajojf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3tgwchbco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ztaulzoz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3inzhreiz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tzpalzss.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mxukkpqu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cfdwmtpx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dulsgwrw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zaeikuwp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oqmpaibl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dgmbreoe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vogevkeo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zasorvra.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvitfzt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mtpoqjrx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sgnmtkfv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3godmvnum.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lfifufvy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qtohqfig.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qmrwprad.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tkxoerql.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uawmkwiu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aqsdrsbg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vedpskon.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jcrfrzvr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxdfojsy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ltgjrnvc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ncywkdix.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mociakup.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xsuwowqv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fkkquajk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3adwgjghp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzbddrt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3amrzzjpq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jpcrgjzm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qvvsjrbi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nspkvdrz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cjpuyrlh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qjeaxttq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lgqumnpi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xlwisslo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ctlfwntc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrtuocw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kfgtpkvr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wplyoink.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3skxlywyp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dggxvjwh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jsbyelww.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqjrxhdw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbwcvua.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uzqxyzxa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ombecwug.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mqffehyg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ladmjshb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgmwlhzp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gpqmzbdq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqmebbiy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dydoeoyj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dvvzijkq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wahuruyf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ujcyvzlj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tflagvsd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zylkpvwu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ateyfavv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3irscbnzt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhpoasxp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vljfltrh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfkdcccq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pqplbiby.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jwzsadoi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3utwsvzzj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lafuphsy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3etrjcaoz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nxxtyeed.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvvapuz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ggbhaibr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpaejtn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lrntbpfw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmmwjgv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uugwfwet.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ogzikdpz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3muagabap.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zzhbhuab.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wnjbiiic.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kghlxzai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kutyyoqe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wxfblkgr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3milinrjf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xzddarbi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pddopcqd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hprdeezi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fqxeelzp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwgxrvt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3brqbpwsy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3chytkqad.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zusshlte.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yrsexxky.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3mwhtiwrr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zzuoklkf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3trcduktz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xoiqtapg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oadzxvvb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tiuobqlc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bvmpplfc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hiwlgxum.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mwekwgas.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3auugcqfr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ipqrxndd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zhyhehip.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kdnnllkk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kqwzqngl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wuxkigfg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpdmxvsr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqcexix.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqlqjvtq.html


<!-- 参考信息 -->