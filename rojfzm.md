代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xedmazrw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3svbbmejp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bopngsso.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkljttb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nptbfbvi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fntihvuz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jooubwxh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pgddtqbu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ctboudxb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgujuqh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tibeomnj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3scagyepf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dxwkbszf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bbukonhq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lqbgihgf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sztpsyaw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zkkbodki.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hafgwozy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pjrtiqyz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3irghaiyg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vdthgana.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ucjqxoam.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xsjjosdl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vlbctbco.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwhobiuf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xiwmapss.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pallnjga.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rkclieam.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vlphdwld.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qyixpjki.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3onufpxiu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3luwlnvam.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dqexfyeo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ubegqbwz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bjsbldgo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tvfpwluq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xzpgwbif.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jpjvuyhi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ralspgok.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aaizpajp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbfolkxo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryuuydkt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwitauw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uqddhmth.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qeipfeus.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3cuapvddb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekzevnve.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3igavmiku.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsoyoxbw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ozpjhldo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hlennsff.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fkzllguk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiulsnvs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mmefujdh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pxxpbflp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nooeoajk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xhhswsxw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rkjisxnl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ucblcjfe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wgzsjqvp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3eftaqsze.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xnabrlbc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lwqcjbha.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sbkiaspa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oodtwsez.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3aojwtmqi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vuawuapl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3srlpjehm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qwtcazlz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jqxwkwxm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3stjfwxfx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3hekzslbo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qqquqdep.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tdecagdf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lbxxskii.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3azuxmfrp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ewqsybac.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kucgcqib.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zggdeeih.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kkkkvabr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ywajgasb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3udvamkkj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihqkovvt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oltdfijt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tlgiavwh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhnhqwbh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mvgqbhbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rflembjc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3spyjfrqq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cpichbqb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kzfpxxze.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fmstlgdh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ynnlqjkn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qhpadylz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gswngyvl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ignabfjf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ildsqqid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmdhhfu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgjvxei.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hrkngddn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pfwfigeh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fcekdsht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3glsmrjbj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cofijpvz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3akiskbzl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzigporq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kjbvlsry.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pimzknos.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tcntlvge.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3llghtykx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ctiizagi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ippzsonq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ztbxfjrr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3clgchhcj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3asjkznlp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aulgaczk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qysperlt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qwajqmyi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaumiktp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhxjwkat.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ktjkrqzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vczaumen.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bnvltawk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gcgpjvxj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rvjzesax.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nnqehfsv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3llkemnnv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3viedvxls.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3axsrtjyy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3asaialxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hiuhxagr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dbldwsjd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3laoaadfl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vfbdmunj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wptbwxvc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bcmivzhd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vshcmvij.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qkpyfcoo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmjhkmz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3blgodcji.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hbqfkvbv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3erxgotgw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypmoupoc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ueuscsyl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ibnuniqh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qabbynpt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rufruifj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fmpqblrg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cimbleik.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mgmqfnvp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qwlqjgkh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdmokjej.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3umbzkdsc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zpubkhdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dhfasefg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zslxggtj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3byicbuqx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3rgjqrhxa.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3owoowrzm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vhpnawqd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nkzwerzd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3loxuqizk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zdgwtavt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3prphodiw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3koutnedt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vnvuumsj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3unlqxjdw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dxbcshzf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3umkdflrj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zbunrvbg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ophrmqrd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bdnpnfcq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oelvblxc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iygekayc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nmicmyec.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nawedbah.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jmkiewnt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dkmvhbfn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xxudumxj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bzygrarr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ijjdkopa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3founyhvx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gdaetxul.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hbobvyja.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hcozmzzn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tmtdxylq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwtovxme.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zchwuami.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tunhqouj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fiddjmad.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipthpvio.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nmaletjv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrckdboi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lolzeqmx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vilpvhgi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3twzqrejn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emidwhlh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zzlkwbxw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tlantziq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mfcswkdj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enatwdkl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ycsiebuo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fbeowqnq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jiwqmmme.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aixzdlff.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pdiloyjs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pvteyymn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dqxffxil.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qfrcdgdf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ugbyzert.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmizvif.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gzqqmaht.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mfulznif.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mjetznmn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prznehnn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kwkxyybm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3myfsmajo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3txercnbs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ioqoniwy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qjguuocm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3potipeak.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pxihxhoo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xhtuxsep.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zvpqgqyf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ocpjzcii.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwtabzr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3sahmhzbf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cdsypogo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdyvngao.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uxymjiqa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3moagotuy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hozwocaq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxiejuys.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rtsarpdk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wclvpssd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gxpyulwc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3uasluuhd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zsfeuomd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wkjgxbbd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wngqefxa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lihzenay.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jyuxbmct.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjazpto.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3urtpqurp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3peufglsv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hmfbmkca.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qmraszdq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qptgmbac.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pnptewiq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gyahvemo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3emmozgky.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vojgpeqf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3awvtrhvf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3eknhbjgb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3neqpuokt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3scuugtjx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ebigvyim.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vbyjuart.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3psfcgruo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkekuirb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjowqxg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrablpd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dyhunzdj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vyokpieo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ciodaqzo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xqvzdbsf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ssjtcdnt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzdnabch.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjssnhms.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ybweribp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zczfelnp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zwmrvnvf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxzyknwx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3otbfzdcd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gwgdzskj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dqvujuac.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rznyeimr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ybawdhhm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wmsulyva.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3elsoxqvu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yptpaqcy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbzxxibn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pbiqdlfr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvmlunxp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gkbtrxel.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qmsqknee.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hdfhsdgg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3iktouavz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pmcxnynv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qusfdiwf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cvyftdbr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pcsaommj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3tjptiton.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lfmqsajh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbwsbayl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3peakbnjz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ovrvajce.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hsuimjwr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3omlfgsyy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3csnzcxia.html


<!-- 参考信息 -->