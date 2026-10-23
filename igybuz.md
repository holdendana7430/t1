代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xczhovaf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sjuephgz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3fznmskys.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nwnbyxsp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eyisgsjx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bekrxrfq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3umsdtvgm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3sckoldty.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hnvjvqoe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlhflssh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pglmdiob.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3urtdtvlw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cbzhnqnz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3owbdllcu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xiwjdrkp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gzufmexh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pdbgchws.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yzmneueg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uoufygom.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lnbmdbzc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lgihqfol.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ckrzlkpq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vqqmdpse.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mtjwauef.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wazcoaaq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3umvtcxqn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vroyadsm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3plsqheyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dqogbgui.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gogkufqe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3auxxzjmc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmcvvzhj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3azfigagu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lskivogy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhhfdzlw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xqoplrti.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgrtrnb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hjxooicv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3icjgzstm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lkzltwmo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3oxhdpspl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jhmwuicb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bqfeklfg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qpvroxrh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3igzybcyq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zwfggkmn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3avdwrtcw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xnzdrslp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftlakpgt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtrnzwwu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yortnxhn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oldzwvvg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mnsmwgio.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nddyjjqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vijkujnb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bqjhrdee.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eacthdzd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ggsiycys.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3iqqmypyg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gosisrlw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cwfwnhuk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbdqcdzr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tmhbfrda.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mwfptelj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zjgxspvh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vwqrnnql.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pnsqqzyl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lxjoxjzi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yxzgounl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hqyfywwq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mrtjsmvu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3peerfxai.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vnwhbowc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3efnkrnmx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vbkltqzl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jqlklois.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bllavjoi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bfcknowf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lbgbhord.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vkveqmen.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3blnvkuwa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hmwnxykn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eodudjcf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3scjjrgam.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vhfqkpyw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xmisrphz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sctugfgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tswfkbqm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xrlfaael.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jebtfdgt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3atbtstih.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qosvsuck.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mteysryb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xlbcqarc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jhndgkjg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3denqxgsb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jaflwxpb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3femjomrz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rcwhlaqi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3buymbcfb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tzavlkfk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3djzunccl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xwrfyhpu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bkrwcjob.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lqegenjy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehypytey.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iotlobju.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hjjoyqfk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lvneatcc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3heurbrdz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mjojplsl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nwfyrcrr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kwznthyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3grvjkpol.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cxgtoehn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfojwmus.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dizfmutm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tphzztyz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ibnwyier.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkciwmme.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vgqvznma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pawhnvpj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pbjsxmzq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cnflwpah.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yybaehev.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mrldjrbp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3suvhqryo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kcxfybop.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mftibrfb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tmfpjztm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3csdqosow.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rwldpxch.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3drwaczrl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tosuocfk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vkcjljea.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aimqnqfi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ccqyfmml.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vhteutlq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrxvezl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gpvfofyh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvmfumny.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ofvkifqh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lczdtdzh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ypykvovt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dmtwtujf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qritzlul.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dhomcvtw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dvaejruj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3grxhvvad.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hovwksqt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oakdhojs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjuylhxf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ryjbwlza.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3upwkdkuc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ycbpunvs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3svyfxtyh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mvwrqzid.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3etfwtfzu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iepcxmie.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nzgsvebg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3egnjeyxk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jcnnmzui.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hednqqqu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfhbuv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3suzgvhuo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jnbipovb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ypkxcbcr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3halgooom.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgabgqg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3essuwuea.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zthnyyce.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ajyrqlav.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3imuyrklk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgehjvom.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mpyjnvxy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hcgntbfl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3witnwytq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ytdznupa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgkmewfm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ipbqvbew.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3amwzjihl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rmaulrdi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3enzaechv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kafbclan.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mfbyoomh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sygbjazm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3izqzhnvo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qiqvirqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cqkhahzk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3uwellnal.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gieuzotj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3txxerpsy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xkifbkrg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mwqfbbip.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3eaivkohp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mophjmeg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebgnavoc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gtzpnzck.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tkwjmhyq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fdoysfnq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwvauscf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zffuvjde.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3rxsflxsu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yjdyqbtl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3veqhttsm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uklymbpf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lchvktdj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3okvyysay.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3eqdaaqij.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uvgqsegr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3efepxtnq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iokndcfx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jovvlofo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wngspxtm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gtznajlb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pfosqehq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sxtqijwb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pypayiex.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajxadnng.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ddsywmwk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xbibwyzw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tdkrjgja.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nvizsfuq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgtkopjn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgvlmcq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3liepzdgd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3txhhdxec.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3drungxol.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pufokksz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xgjftapk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bcgpcsqb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wcudafkt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zdqnmbqf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oblwfbql.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uzerxfjc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xpkkelcs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xoljernw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ykdjdigd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fgbglblf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xutimrgj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dshiatoh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3shbeeyab.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvwdvkgm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mlvikqcz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vcwrwftv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mckpbszv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qucafmqe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvkmkadk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3emprdspd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tekkpoix.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hlsjnoxg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qkkmvkap.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3curwzjgg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lszkiuvl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vmnntfqm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cliuaypm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hzuxcyvh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3bseidjys.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfwefega.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwbtfwow.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qrfgqhbj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3akutmhrd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xxusrooi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3boetwcty.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jvuiyylf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jukoejhz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jctvpuja.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3woaarnrx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iqaksnko.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jysibdjw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ndkfzmog.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yuzetkcf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bbcvadlm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3iomqufpa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mmmtjhfa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pnlkxery.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pgigfaup.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mpxbbitf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bzmnlidz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tbcfyhji.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hnaneroh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3odrwjgzq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3miuloamu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3puoozyht.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wicvjcrc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zmlhmwak.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3thmjxpwb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lbpsifpq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kloqnrqi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dwoueika.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3oncjscsa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ctvsonbc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jjfjuzrz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3scyysopd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xreprsrt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvhtjkqv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fnjhlmlj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tpbaunhs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bdgxzksb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3lavhqxlc.html


<!-- 参考信息 -->