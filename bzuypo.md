代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eogcamod.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqematrz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijxkkseq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3yxogbdsq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pblbfgjw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3duymofqi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xfiizfhv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pxwoicfa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3oywfzhio.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtoxguwx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3odmhjaxj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3skzmbtfh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wkfziifc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hotxodex.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lekmtjhy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3acnhnsyy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cmmcninu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tkduzipn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rekujwnq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gerudzaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hzlgwhjc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mmbiygxo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vjyzpzmj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mxglkice.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uwfnzygh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3sfespkfv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lrpfyuqr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3etiorthw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hwwxcjtj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3adfjlsfj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qsoyunfu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ihcpzefx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uqixyfpq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hjenggvj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3spnlhrlh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qnpjmtgv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3imsgdlpz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgcptqp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkwiyrit.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qlxbivby.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rllhuaia.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wrrlvihk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gnwdgzqh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rfgjjavy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qqpiktrz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nhshlgcc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmhhnuej.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3unzwftvt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fpiplkas.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3smnpbstw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3muyldhnk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pzbwweoc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3otnkmwap.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3iabpiagz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ukraouwc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3llnzzxlw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lghifnol.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gpgxdoun.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlatpar.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bvxapbqs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xfbtgaid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ooxasstc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mhrrryoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wztbrneo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lfcaqcud.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gqbcpvag.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vlqlgoso.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3sxwpmkhg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdxotbqv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3eoouywbx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pnrepgtx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3upzyvojg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3srzksyjl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rgzuihiy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iuddndhi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oegptibw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3owbvefwg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bccjayvh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ypnygrjk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vkxysobt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3clyvlhpn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3esqcbtmp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zjuqzbul.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nldnqhmi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hegoucgq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rnfrpngx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwymrbjd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cmfvfmft.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gkirpfgh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zdbdnjnj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jvlltiza.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffidrgdz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwymteg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ihzasjmd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3aecmojbe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3juntrxdv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xmmoxoth.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nzlizbfk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hzpgrvxa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3odhcjjmn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qtlmwqop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhehhdkx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gaqctwwn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3heapohvu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vgkxjyjb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3whrjdify.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ieqlypgn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3djzwikaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3piubgmze.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zhkorzda.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rhldkncm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mlwwqnwn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kstzlkpz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xlrykbea.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3onvvjkfz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cpdbcnun.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qsxxkihq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qlegxknm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kpevtfpc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mjwcbidu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vxgymype.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tizqzyyo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ugzxgxql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xonebmqc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fkqyxkfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbvbzwdy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pzqrzcrh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3eeztopwd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ezecctvf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hqdyzobz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qbhswxye.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vgvuadot.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3njiqzhmf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tajsxjux.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nktrcjqf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3raqwusec.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vahrxczq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fifuxzdc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bnbdxldp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ojhxvqlz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rdmiofbo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3osxqctqi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qcakjipm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dzpnguiy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cqxttali.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unroesqy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dpnnkmyx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jpnsyhtx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xsaqoeag.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3theslgpe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tqysauvm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3emgodnlx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gmokbame.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pdndvqxr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmakqgxt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwpwgjed.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kmrcphju.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tgxechlh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uoyebaxo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3covioodx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3oenkpogx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3eohvzlvi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ffsuuldi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ukaiubiz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pnkjrpez.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uebighly.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3osqshpul.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvscaep.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cwozpuyi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ewretsvr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ujdurnaf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lcqittfb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltkcdywi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jcvwzkal.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3idemmsze.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3neubwyom.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dcbwhtmr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwidbilg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mxuoropu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rzvhcfig.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hmxfhefn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3prlostio.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sncmghhx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ridzhvkh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rirpuowy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vvkpjfxz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vzgkghyy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ulrqpsas.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vexlroiy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3adjacjtg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mhopkypj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bpbhwmlo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bhyrwter.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ltoqsxnn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ivhhhswy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtwrfmq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nalhbpnc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vcsacaxj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gansswak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ikawigck.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhecvzq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3iwlwhwvl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nmalqswq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jjzlfcjt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dbyordjd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ahpdaoxs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3uuxfrptb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uslnluib.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gishaqzc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3buoypbua.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pmwqlsqn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ykqhcbss.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3oeshdtkb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bwesjwvv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zivbufen.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fjqnvmsy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ynwogjbf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wbueqwvj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zufudspg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ghpwkiyd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vaqceyqo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lkzsorkf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfvosrmg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3foxtebvq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rpzxalsj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3sqgmfsyn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ehopydfa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rxgkbkdg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvxtgas.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qkxelbyq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cabjjdjs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3typmymvc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymspqvys.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nzriquaf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wmbzmzcn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3goarfyei.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jfwyksow.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgcxain.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbatfec.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnkzuwcl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3eyyzmxlh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mihyvpkj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3enjugkzf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xagybqky.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dpzhsrur.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehtrsgqa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkrlkqn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3aagcnues.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmhsbmxo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gmepmtek.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lldlvtcf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cbnyooav.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3immbmoqs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fazmzxlm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yuzsbatf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cqglizfm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ikfgohep.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pqsqgfnu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3htipmeop.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jfsgmpju.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sluhsmdd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oxnnbelq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3megknmsn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hqiunswe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3stwcgqaz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wilscoyw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kdjohcls.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xcqhrlgr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3izwpbnzg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3epcrkdpr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lllrwbob.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrejzxa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3runcagcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3drqppxkb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewvpkxwe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ijnhvaka.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3itifghet.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3lrnepdtr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hzdmwlpb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vxzpecgp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fhbxfmhc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vjoqylov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kicaejrw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xkpgbtpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vxiwjhbr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3twbvjcxk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ntueyywg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjvdtvgk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lldurjys.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nfqfxmcq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tywbbbyz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pvbafjfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ecmxkhtq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pxnoxpcc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fslfegbw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3swgxnrcc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gpvecsvm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qiediwxi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3buqphqcp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umvhjqjp.html


<!-- 参考信息 -->