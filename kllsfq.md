代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nkpsyshe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ryeqvmbs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jenjmxjt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tixpccyy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cjtokaea.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsapvlxo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wusyaoqm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3whazrkjt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bqiblrry.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3crijvfbi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lklbgewb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3alkkauwz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jdnowjee.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ttuzwlor.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zmfkckge.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ccnwofno.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wsuybmda.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ivzhvgwk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gfqxwtqe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zjlwybfj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oqzkorye.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3evykhjkf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qoqbbaiq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3phrdmvmn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xchlafuq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ooalcuge.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ltjvadyg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nzdxerdv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3buhnihum.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gmrvhksz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ojcxyseo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bnzkrqqg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbhbmtu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gtcmhfhc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dcbtivyj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3spwhdskl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xwonkxmx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yncnrxnr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wttgvkls.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pjqxikfa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dtekdfuc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3veicyzvo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3imenktvg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xxczklro.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gbqasqzc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mrajbgah.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jqauaqvz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wnhmvaga.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhwmowet.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkewfjng.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jejmorjs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3txqpfyya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3mxtatybo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3usrpysmb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3quujqmdu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rdpgfrsa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3frmcpevq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sddjdupq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fuysokmk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jclmfyxu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bplnxxhu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vdichinr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3znmzofki.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qzcelnyk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iipmkjey.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jbtnliei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3civwjfvz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lljhnxkh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fifgvcdl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bspavrfy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fosvopos.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ofjgkoxv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eaovelaz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pneliqji.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nxebrzcv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hdfaiswh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cuaygxvh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ascjzyek.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zaefjpkh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yxdmugvm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3iafrfjxc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3faogqhkh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cyhzoqui.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kstxlkge.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rvvmttti.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cpkosnzz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bohcajys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vjuchwxa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vqbsqjrd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kzocfzbr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bsohemct.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gcgxdtoe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3oixduxab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3klhrudic.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bzghehun.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfnoxxs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjcxqzb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oxiflgsy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sjrqwbeh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3aqutluek.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3btvwmrsa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vlgdjsyt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eqccvlbp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wxiiubms.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lscdnauq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzrjnefi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ujycvjgj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ssytvfdx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dskkgeyn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ofuffdpf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qbyreuvz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxgjjcz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xpsgvobn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ktotoanw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vfvufxzg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sdduecpc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tkwdagqf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3glcwexhe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fppdsvsa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hzdbkqzi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3lhtzgahh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ztsjjeow.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dqzoscgf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gctvenbv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dlnhtmgs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxoumtcb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwxlwhch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsatgynt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pezikgri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtqonlqt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hnambicy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3sysfmfja.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tmodjiqb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cdycyjqa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jprsxayn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jrptuycn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ojyziffe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wdlycmsv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qxgjwecn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dejujqhx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xegkxajc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pvqcnmjs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhxjvgwv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jduffznv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lkdqhpjp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tedtmfgw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3njvgkavz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lwpuzsne.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3miwasilu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnkqqtu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uajjskbv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bjecslhu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wtgzvwgn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rpxsfysy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3npyfpulw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zjezjucn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bdnoojrs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bysetynv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wybxnosj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fngfczcd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lhwvdpcf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rqydzbup.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ycmpkure.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zfhsesln.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eorvllbw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwdywrek.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3soumobab.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mzbtraly.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vjltwazx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nvtdqcem.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jynrxnfy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hiagakdi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3daxofecb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vuxirveg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qxeytixz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dborzwow.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzdsiset.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qepjdiwh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kzkankgc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ondgmehc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3geednsan.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqepznql.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hisffeta.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bhmxgnnu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lyjazmhf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3reaaqsxw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ghiyxlkj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qranucvv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ciqbalkx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xftmylgo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ctztykjl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bkodyvji.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wpkjmuuh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bnrsvdse.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ggotxyrv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kxzsflqr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ditpykqd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3amqftzda.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rfcgsgsa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjpbwwa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jhoqmhqm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lplmyuau.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3quiyberd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rbilfunv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uadtavsr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zvtxmxtn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bcshqmtn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rxmgdqbc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3quecduyh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aiscasgp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bpgcbttl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3anwuokcm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ishgtpum.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwjifjbe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mokjdlcy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwajzcm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3aeaiijal.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bjptupyq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3bomeyibb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bcdbgqps.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jhkysyzj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ywtytcmx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sxbhduig.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oodvvmuq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vnqcnirg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtzjtch.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvnyujxc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bgrshbyl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3iylpaonq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qkcltjqy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rtcycxyc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrcrjffm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ljvjlqnj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ylsfbbnw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bdawuidr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckcsayal.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ualonzpm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pkipcirf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ejqblpeo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3luavrgvu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yhgbqvby.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbaoqgt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ovhooqfm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqdeuuff.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zitmhsro.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdxybsuw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xdkprwxh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uxdzgcyg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ediiayol.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umdipzay.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etkgspbp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rzjxjtnk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sclaxshd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cjeoaaej.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qpallidg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3txdjmdee.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hgmxudry.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mqyfjteg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3agvgefhl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mygpnxfu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3auljdjld.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jpgcgfzg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lfslysxl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3numskjbl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ejrooeae.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ljtfmkul.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3awzlyffg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iujfmomb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ihfyudez.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkjphjb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ezdtqfdg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hjmdbgud.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nlmhgehs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lnhqawfe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tasuszeh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psqiazwk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tyuqudhp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3eqktnxch.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3oeqrmmxw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gninojql.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znthfchg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vrzyuwra.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3syfblvsa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aumypweg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gancuwrs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xbnhlsng.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mjqzmeyr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3colygnpa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iadvoxiq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3repeiplj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pjqirusk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3srelvpmb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cyhtiuln.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzgzkkl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vwmlmehm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3onzqflaq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgrmegi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aubehwux.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3embnfcxv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3otxgxlwx.html


<!-- 参考信息 -->