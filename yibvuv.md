代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wvtkxmmd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mibourpq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ijrfwrnk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hydvavgm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oumlnmrc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wvuewyas.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ejsrurjt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hzixoqpq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zbhfizpo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vuatmbtz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbjfapz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2glkczylc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iitffedu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mggknfiv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdyyvjos.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2surxcpyw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vliqpykf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2payrivtt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfgkengj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2eshhgkyv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wnyelrqf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzhzgseh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gemkujtd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cfjeyruj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vrfrykox.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aedghmos.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qpeapqfy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zguvldub.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vhspabvm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2uqzpsyhb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rttizlvm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nkjazjkm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vvuubcgp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sjgmxwhg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dccvvkvy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qmbzhpee.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jvoqhxnd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tudhruds.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2flqdmmjg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwahtwia.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rbddvuez.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ozhykimy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dwlzlqhr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vmigmbgq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fkdbyuzn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kesfcppo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2brvztozn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqthuqcm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rdrxrdku.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yghcjhqb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxtmkzor.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zapxhqdk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vfngglgp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qgwvnqzj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jznydfyf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2elsxptkr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oomubkyw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xutewgfl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bbhxofzo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2afplkzwp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tqsdigmp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sudymvqp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nyzpjxij.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cccbmoch.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2shsxmtid.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kdoelaxg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rizoelpr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2npcxphwc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cknusmkq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kifngngc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2biavhoqo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rnznfhvf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ycteitrc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2aswdtypt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2crzqvjba.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqpfdyuo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ygmgntul.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2luxrtohj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ixwtnrdt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2emwzlrzc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ttiziizz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2znfojegt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kgrsbfqp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2mmaibnay.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vnkbgkot.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kgiuohsh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jkzepmvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2adexzcwu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2oxikuuxe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2awhvzsmu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tofwlkfb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gmqaxdjz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zwpdrskz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jivstnpl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ivqdjciv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cqsnfpag.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jymhnkir.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wsgiscln.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bwlobsoq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ervctris.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2caofrupy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jllhbvpq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bcdpjgid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jtdhimaq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2plstwnkq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jdcjhdqx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lkoqckzw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wcvdgiaz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oawnfzer.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dbvxhnkc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hisimkux.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tqkdbbkj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2easgmufu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2abvrvhkj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ybdwiatt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ofkwehjg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gdvbtool.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2upzirdyu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2crzahayr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rmacvaqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yjbpbmdi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2urbkthkm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gehdkmxn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2omwlrjjs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xyvmjofr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kqqigcar.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dnyubxgt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kahfazex.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bfgtqdoc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xfqmffqg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yuxocgrg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2breqpjxr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kpmgfpmc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2izaunopz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rzodypvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbspmviq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2aejdmosl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avyujgvc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ahqlmszg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2abmhiayx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zczhabps.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nbyfyjca.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2oflmqmmf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gqsumasx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xmvfjytj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kpbalxkb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jgqanlac.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nwcanypp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dzrgvqir.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vqgogunc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tyknofus.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dtyurgoy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kkzxprmb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtsgzma.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kjgikmga.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fyddxgga.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ohrftrlk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2biwsikrq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cxztuwvs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2elaxjsxt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bekrocgm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nqjjsxzo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xdulsmpo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qfvzuhqv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qnrxzbbu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xrskvgaj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbpaeuum.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eyhorbfo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bhbqsuxo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gkmphcwt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dsqylsgo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wxnrkzjz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xhvmzocu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vkjtoika.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gqlvkzjv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tczghlgc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gxhbsgiq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qnqvxktr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gffdwwss.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2arqvduow.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rybqxnzd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eogzrddg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2okawnjuu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vndnqvtg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uefnduxa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mizxjqrf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jlgfbzio.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aeablasv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2anadxeak.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yioqolpw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mlxmqmla.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ccdowhub.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ctmbrvrm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bbtnsyle.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2npnrkoil.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hqcdziof.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wpjouykp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2agxnhasv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lymffjwo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hrojjwpg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2idhhzxal.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2phdzilbm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qneeyrxv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xjllcirx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uujfsrmz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xxijtbvn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jnvepnno.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tjtcxmzo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aaeobnkj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mayqfoad.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2huxardxd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xnhhmsgj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dlqkcqep.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gbhqnsxw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hjjccigq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nbelbmow.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jiptmwrg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zajhbdls.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hfqivlvo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ccyciwkr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bysemhro.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2aatgylqg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wgvfkfak.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfrrgot.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2phfzbods.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ljvfdcvt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2usmimhti.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ocrpwbpc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2polselyh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nlqbaujy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lydbaxot.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2buqmturr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pguyasbi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wdsckvvb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vndimiha.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uvmmwvpw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2eeaiwanz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mttzejfj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2eseyxwrw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rnrqgbsj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vgpcmzhf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yemtrseg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fmbxcxmx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilwrhltb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jwuichik.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwhobjy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kubtoweb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tsxlnlnx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uyqvtgns.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbjojqar.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxephel.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kkjfedss.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kgtxfevr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvucpybo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hkkwgdbs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2oricsjww.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2figokswx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nqqffjbr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrzdprt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eumutykd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2dnoqyxzm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nfrguvoy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzyiajhe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkiwldtr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bzeagxmc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aabqpckj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kgmupros.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mazpglqy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rqpwqpgc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tybepnzi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2imfavhxc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2feontubk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zxuekqyh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xbqhktgi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2slumsoqh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ainmrebf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxxawgv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pclkexfu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yscixgbj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cexdaolf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gdwlctes.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wdrnzqdb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lryadopt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnzagvmc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ukbjjqnk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bbfzadzs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdeioaba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nujrvbql.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jiufwvfr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qvowvrsq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ssgeflzz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kwhlfugl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qsrzburh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fdsgmnwq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lknmnike.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2prkydrvr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lbjwpska.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ejvzsbyl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2drmjjmeu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gurrqase.html


<!-- 参考信息 -->