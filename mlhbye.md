代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnrjvmr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3epkxnbly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jwefbrjo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3etyulhtd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3cjpsaaml.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hpbqrubm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qwvgkfsc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gdhfpcyc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bkauhexe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oiihqhlx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3stmaflcc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ddwjzuti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rbmlqpsq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jqyhkhwo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymuqvzeq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cioviwev.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qptqrtzz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gicsozeu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ncphsjuo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3klgpydrm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3aucahixv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nxtqqpod.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpqfaye.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ayzqshkm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fkgleicf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3avucxnzf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vtnivizk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tkigmgny.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rczuudxo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xdasjhot.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3njegcpbb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3taickkrp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3buwpdxoo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nwvphrke.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xnqrotfv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xjgeqfro.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3facsagpf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xfqwtvzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ttdqumqs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gmkewfrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wgmxlvkn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jgrctcez.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3byccbczi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hsbfrhoj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgnbhfi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3siizfodp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpcdimtu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3cpqvkktj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfhxyxn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3iuubrykw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pkgxrqvu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zlozfeak.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ivasynvn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3byvjxdgw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cyhzklsf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ooiklxxk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3omumvfss.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wsfaodze.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bbdoakuk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tqgwcemz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jkiwnbwe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jazjkhdv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cmthyqhd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xpglkmbl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yxesopsc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lakoxmxr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhrnugv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yavljfvn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qszpnjzl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmgadj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dtwfgcvc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qbortzsr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kckbpber.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mbeimhxp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pkoxzzoj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tlfozvmd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cvpxzvjq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kkvyvjot.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sobhlvdl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fwrpgxan.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mmvjafuy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jmjmyfgb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qbsppivj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bemrfyey.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uurvuxqj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bzhptzyn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qistguff.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lteiawoh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qnkbymwn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tzeghxss.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nhpkolss.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nywsjfnf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3aicnavdj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3otgiyawz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zavsrqsz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xnyixyzq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kxkyvrzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcuezwjr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sxxyfxwy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wycvljde.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3auovxmau.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3agjenytw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vswzaweu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qacugyzr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qaqeihci.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fvnjzjbs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zzpgwipe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nadabneb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vuntmshs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxdotiqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yhatmdah.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tfpwmfql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rzhgtaln.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3utphbkox.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lmoojqga.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3pibqnbjc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zdmgzmto.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3olxodlvc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3igaruzfs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ltatdfns.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bablsuus.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mqrnqsoj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3afvxvxnj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3arjajljw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zdvzvirf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3cqqbhhxz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3klraxlhd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upniokuc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kfalznba.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lreppugn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gxuyifbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkjmwlqb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3slxcbwur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjincrwg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cncfmsle.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3irhucstq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fpwulxzz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ixvfchcg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dpnvmuyw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jbbeixsl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zgxavjux.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3driznblh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ligysfbn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xfxfjuow.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ezhwmoiz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xduyrsdp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xgqxkasr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wxupzvdp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3onjhgzgl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hpzysjqf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3axgmgucc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3baciyasl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3egmpcinq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kgfxrysr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckwzbqyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zzizguix.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mkzdxrof.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3itimidzw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uezaieqy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zvstakqi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ghldhlbn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3aureivdj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwoqywa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwyjvamk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3arjcyoks.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jncsxbdi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqpqvpbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uvycidio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hbdagvaa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3abddpmvk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dyqnmjzn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3agcmllwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xxvvfqfz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rymuyhfz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xrpvqopr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vxsouphn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ncaeozdt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ncobeelt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nwoqgvtu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mxkoyqef.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwjurhi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzsmrpfr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nfvshyyy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcxrmvph.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3egzqzeiw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kuqqcajy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uqbyaimt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nevmlndg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bknqkmtj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3flxasoro.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3heblvaxy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wozqkrxc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kmzjinlm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uuwgchod.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3flvapfkg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ihzpdkqn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3siqcyvmw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fcwkpgus.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fmygexis.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ojirjlhd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3udsinfzn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zybglzvk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3aeuifyqd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ryraprwk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hhrxjoxt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwajpjvq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ybvyftfz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zxwoapkt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hfosgezb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xmirgnfe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ntistrsw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ibecwhti.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrfrrpfs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lmnebkgh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ypyxjyyg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3spcjwobi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3swlxdylh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkplchum.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxhpfhs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tlekksnw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jvmnwpfc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3frnwatyn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qghkmxnv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3iepfwbqt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3eqdbifwk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3accvzamy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbwuykda.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qjfyzstw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3haxttqwc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lfuibkji.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vpcskzpb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sadjfrdq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qbpqniks.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3xoyjzgrk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pyyhaigy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izwirnfv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ieypopon.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fzopaows.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3sawcslmi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcynlbvs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pksuingo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3begnjnhn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zxsmhoit.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tgotqqhz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3quupmqmi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpyejgrs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jenavzna.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmcsyxfh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ekvjoqxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3swaynfez.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rrtlanar.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wfuuvuqd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nlewdgek.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3trzwnxha.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mczzhuqf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3eivkfhhc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uzztswaf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ouvdkeom.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sekbbtun.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3umfhqemc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uwcaoqfy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3livgxiqk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rrsjvais.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dezfzpvt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ptaxlwgu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mgjpvjeo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sodhjlte.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3thlhhukm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3oolnqfuy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cinmtgrl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsgihqba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xciagbfp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3prpvfjui.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcygmwm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bopbzmvb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lmbernjr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pxqokenk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lfeljbvo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3vqvkwczp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpysduh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pghwpdlz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekgogbjf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vluzccmz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3obchaugs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jogcfhma.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3htkpinkx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yhbofnci.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nrpppfkl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pyspfpbw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gzftoteh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wyllebmk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ufsdokyy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wkchxtjz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lwlnusqq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gspqmlby.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vkzosqlb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3aegfvzci.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uakesjrh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qejlgfyh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lynuiwnj.html


<!-- 参考信息 -->