代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ohrwirxt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xvcenibi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vqvkwczh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mdluoobd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gbwgmloq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skzctkdd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tbwvmxgl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rcqugppb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xuneqyxn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3scujniey.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbytmeqw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nbwohiup.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kzciorbt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ifecunre.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ykhlbrim.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3acjtfgdz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3eylpfwfr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ytttpzmw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vkcymoci.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jtpfuybe.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zvaxqtqn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dnuhkvqe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vtdgerhv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pzfjpwlp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zlqenfym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjqcwsrr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eltxznyc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mdgfakdo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfljgnsd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dwulqohc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ggdppcmb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjbxdoqt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fujmplob.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtikafm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ytpxdlox.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dxntrjab.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxrlqnp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qgbcvtyz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3swbuvflq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qqnarefp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qymahgsb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqfyexzd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3daehexzo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uonblcpu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qpvxxsjn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tvjqjsql.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bwfuygal.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogdsfcqe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zkdmxnuc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuvbtuyj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gdjsbgmv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3afrfbhfi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlatglzd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rpwkdbjb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpfpivs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ctpgngvz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mpkvjuof.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kdsbxhup.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vzdfoagf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bfarbtsg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qdnfgker.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cbegtsyf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wsubtloc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lhlijtxj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3macxumfi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rwosnviy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ohqslqin.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ploumfpk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ybdfyqak.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3coanncxf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3szikyazs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ogegvicl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yeqvifbv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gkmvkkjf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tyxoaiaz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3oxsguips.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jbtpdlfc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nlgmmfiq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xaksycvu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uvbybmdv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3yjbvtoct.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yusabcps.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ypfwuoih.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uepopoip.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xtchvqdt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vagbxubd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3gowkjofg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ltqkuuae.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wvcrayka.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yhlxhfpu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gmwnsssx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rzzzcowu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gyknbjvc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zdpjammt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ryzrtjfe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bxvpzpcz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ulpbtwfy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hqgqqtxm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3oeswktlk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kqrlazua.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3dtzgodoh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3thdlrzgr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yskhwicj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pquniqdn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdckrlor.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nlnwzyvt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3soiepmia.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qygxwzut.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jueltpyx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wplorwul.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mrbzxbsw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bdmhwivd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3egogercq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hiiqobjb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wyusniuv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3sbnozxev.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3miwdujqu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xujmmfjd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mdhjylfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxdbznic.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hpwzpoel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndvjwukv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iqrjjdug.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3namnjvsr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3medfdlzt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ezdaglee.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dnvfddno.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vwksehqk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fvzfmyql.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sftigmjl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3upuaftou.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3uzfcgkfc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iowcuyka.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fqgeyvje.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3piydzjqo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mymhexdf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3foemsxbm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3liibanbw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3aaasiqlt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3yztgjgux.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cccsasih.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnikqci.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3npsvxgcx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dyjnhkzh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ooazvcff.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bcjvedwg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bftksdyl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xzttxzmp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oswjllbx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3izfrycqj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ymeoiiep.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phdxkkhz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jdihvxmn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3czgsjysy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kgwtfego.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nsjsnrzz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uoafjrsc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcyigzlp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nmqfkayr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fcmpxwtf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fnplxafb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqoiri.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pjzxewqq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qdgzbdin.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3felgdjyd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ymotcvhx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bqlwdfgm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ukgregxu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bnnfzhwx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srgljfim.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pmrehpna.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xwhbhmzt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tgyoffov.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yvyuhiiw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gnfxdgxk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3caiwvfcs.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3igrbblsz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nkykfhnn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mmkmtlpc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tasdqyme.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3egiiiocv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pnfedngk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xfslzqcd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3slxrgvjq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xwbgwgny.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ybzvrjod.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dtxogytf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3famwuccx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ueottfng.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gnttzrwo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtmnnnul.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wxkniigw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ppxrvecp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojkknpar.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mwymztfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sbexkuxy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmqqfyze.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jxluwjfg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vfrzsvtn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hzuvijsk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgcyxfiw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wlbchthd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wyodktav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3azhoktgz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vkilgkcg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qhubbfbx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iodzdnrx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lvyilxqh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vuddddxs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tcopmnse.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jwlllcxz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rmbjlzkn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qnmxaxvm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3erjkyuuv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3oxpmgkxk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3grlkzfoc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3buxtjsvu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cazpokiw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kykvxbbn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oiwqlabv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ltlgkrot.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3igpmrepm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jzyyiuss.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hkmtxxcn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jmhkfxdy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3smvcxkfg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ovicmoog.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyssydxp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vnbpecoi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ncrmjnxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pozfnzlb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tmvptmrf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hfdicdkf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qninkxds.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qhonshxg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zeqzrwch.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jcbyammp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ovmspeka.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3abzyxsan.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3erbosscg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ocapsqoj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cqfkywxe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofuxpbfd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yxvuktft.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlpgmeia.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mhynaniz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fggxpugi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kzrytnth.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gqpeelup.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oylglrea.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkjlbvks.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qxrygfjj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xwvszxmu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kdnsnlvw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jgfhglmu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qmegbaey.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vthmpnvl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3svtbnzju.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ysyzabdt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcvafsgi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylpkrtrn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ffqkuhsw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ymslfbpw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ddcrwgxo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dxqrnebv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uorsykrn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mrknljpp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfhsdcji.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eoryyxfd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udkktojt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3npnndocd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qkbtxfvs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjgenoq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mzlnogoj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lkuerlan.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nymgwmms.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3iuqmgpfj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rkeelujx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pcokfmhk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3kylndyfa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wdpvlybr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3nlmgndks.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3obsflobu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnfypnwn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tzlkgigm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3anwghule.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pqkdtvrp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dnqgcuxw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ugbsgkay.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iebuumcc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3isgvzede.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bxskgwst.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dhqmpthd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qdnxbvwp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3iizfrwkz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thmbqgin.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qfbdjuif.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dkjjrnak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vdeadfvu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vxyrvvxl.html


<!-- 参考信息 -->