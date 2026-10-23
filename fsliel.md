代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbmsmrah.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ppxekqab.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3errkuocb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eqefaorv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mfzbwtev.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mbiulacz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hbeuuwgy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ofgyxhez.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fncyvqkr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zpysuzqo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcqaepjo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jaqwlxte.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vzrccdmr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hllqwwvp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ydtqrwvr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yfqfhlpa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwpfcqpw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzqhbrsu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eibpfvpz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pnjvuhkx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qazamitn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhjjrva.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjnyxid.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ipyighwa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wvrimlan.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jnnyivta.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bbgnebed.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aqogaqce.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cxyavcwq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3euyyrkwf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nhzhzhnx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3dbmcjwne.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3duoisank.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vyzqmsma.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vxtbozex.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3egaarkcd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qdldmmyj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qlupbwek.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkijcst.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dqddkjtm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yzbntsqn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dmkxidxk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3prftjzit.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3injhsheh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nfnaxtoz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lswxardd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pqtlvtuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ckecmwkz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3frmgneqd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dyjpcvfg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ebjrnrly.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dhjnmhwm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlqgzqdo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pvwfcqqw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rvmkvpub.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ifrhcriy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gtfcubdk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ckrwjbtn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ncfoppoi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3usuzyefp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwqmzbd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bpijacnq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mhqpazjo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3thtpibxd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3amtzcafj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3eqsgxcye.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vulkrxhl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qhxzjhcb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pobcluiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3iziqiltd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gqwajhte.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dlofvbva.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lzthbddr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3spmhywjv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yykbmwms.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hmgccecu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fjimitrp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3maavznqu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vfeiyboj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dwvgroto.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3poctlnxz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yxkfuvhx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jffozite.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xvmixqtq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3asiqhzcy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yyvrakdm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eqgswrji.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ittozwbp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vzqggqsx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zbezcigr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3aavkipmz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cumagjdc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cdfubyli.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3czlqijwt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bbjtlhhu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3twsrzivf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ykdhqppo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fhhzockc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3yncapjvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3blavvinq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3punckbaw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jozyobmq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rwikwpsp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vmpfvdwt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3abmxepbc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ntmtgxqq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3acpkzera.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nlasislg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iblsmwxm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqjqbcw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ijaonjih.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cwrocfuc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sobjhylg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3caanhpgu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3simibzzu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mkheuyjw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlnuxtkx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qkrytrgb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hieeocyh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nhdelzso.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rpnxrthu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xdjnukhr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oogpwaox.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wtzewfmx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3roujqxry.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3uzhtirlu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lvpplmlu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vptzccwn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mxcoigej.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bwotspvi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uyotguyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbrtisga.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vzmsxfvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhgcmmjq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pckltndw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cmqopmhu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kqihacxs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ciioigpo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fhmpztsx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pypcujoh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bjwjwhlv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zhicsijh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uxvbkxni.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vafgtcwb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vgjsaidp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bkbujpmi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bybtzcea.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3chuvmhyy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxjqfzd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ytboesor.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3puzbkfgn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzxohpoa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vhyaexbv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vmkeufrj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xievtjyi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3nblxkgio.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lfrhahuj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3agarvxlf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hiaczhuo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3oqopavyq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3saowgtan.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hmgkvvxl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkrtpzh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwdwgzua.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3anupzzfq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ijcicgty.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3debotuqg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lswgvzfr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vejrxrft.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3juansgyy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3keanuvaa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ztztqmgg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dlkcrqiu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aiepente.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntxhzzdj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jboluylu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3khrvicsq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wxsmdcpf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wfwvhfjp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wgbmwdec.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkavoxj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kwmaxgnr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dmqqddiy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dcqahplv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ajbqmqdz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zbnnvuhe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qyrpzthg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3iojgktsy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3naagizdp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fbsbuccf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wejmnxpk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3omoczahz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tmrqceyn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bchvtbmc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fnvcgyfg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jpafvbbo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qbrxzzrq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3agcajkeu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fslvrtas.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bxizzjgl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rfsvxaix.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zozlebae.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzrmxdoo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzshvtp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wuwcnrog.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hlmaynxf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xmohxuxv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lelxcthh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejjxznsg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jnjbiilx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kltncjlh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qsnxsiyx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3owehycee.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wfumeolb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kuhkzocg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wucdswmt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zunnccie.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xngrssvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kamfkyzu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3upyvqfyv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yljlyleu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rxfxrfib.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aisjfbwz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3eybqyeqi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zzrjxrfe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jytqkfrf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3sjlsxbgp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vfrikglb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ertdkrej.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mhyskqya.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plecbkzu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ddgxezhe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ouzlswzk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gbwlqwmc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lvhemnsf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eptbggct.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qrhddpzf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mwiohkei.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wumlzewx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zblldolh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhnxafqt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wqnzeies.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pakoteqh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqsprztp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqhkhbmt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3akxpynng.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bygyfquf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wrdaesww.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3iafbzzuj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3cdvdgtgy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hiyesajl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3axmwrkyy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eqwlbfki.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mhqgqfqf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yquhmmvt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kbnykeyq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mcpjumiu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dokicaxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dojuxrto.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3errdpboz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jvmsscrb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yexkrjxb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kcaqdwuk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cllqninq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tfccezjt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3imngewxd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lrsucviw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wujretjs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmlxsetu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rdugsacm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjgsnpll.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lsagpfkl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgifcxrq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lopepjjj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xxknktkh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3siapusst.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dxbswoyi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3oltgjpro.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3eqishezv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kpolnqpn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3osorxyqe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evolbhan.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnqgdteq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vhssprka.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3irywakim.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3muuwvask.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ktmqpzof.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wjulnwtb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tywgdmuo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ezzeslya.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbspxqy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pisemwud.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvxjhvsq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wrjxowmn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ezpnaiob.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3orduawut.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kvjcofkh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rammzmyc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3todiicar.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ybiozasp.html


<!-- 参考信息 -->