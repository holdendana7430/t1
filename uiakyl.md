代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kwqjokzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xumjtqua.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tddfwibs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzwijzcn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3whgewnrs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjvngmx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nzxckwps.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mfqxdtqk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ecbvtots.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zrrvzbqe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cumxqlpb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sarckdrl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aipchovj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fiuvckzb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3abuzuykq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xzmptapo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gadnifbq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yyxmssop.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dwafqlvd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3aftzumex.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3udpkivyr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dlpesdbj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nncilqtj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kpkfrxum.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xglzouwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bllbqkmt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ihubnfod.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3uvllthnu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cqjgatec.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofzejqtc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3odviynpd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ncaqnkhq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jewpjzic.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlpijxoh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iivndnrt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3uikbjqrw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xugxsuhy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mjyuvzxs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3llbfyshk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3djjyayxm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lqfehind.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vqsbqsfn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ufznjoan.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jxlnrqow.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qudhnibm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dbivylub.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wdrhgiui.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ejzvemvn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bccxxotp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ltprlkkn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ffnoewvr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3pfditsyf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3olbwtima.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jhjvriwd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3oezvtxjj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3juwujgjv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ikuwohep.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxruswa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtwgzfns.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yodmxhuk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vshnqotk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ypttwgfs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mmrxlwzc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xwypqqum.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwfpbshn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bldfogxy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmzczauj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qphntymm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vfgtgrku.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hztxrycq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vecoqfqh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hbubsjpj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmsheut.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjelhxxc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jtglgndl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kkjadqed.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynypjhbe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uocqwjsu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqoajyv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3irsvovrw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rusdsojy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3uvivaffz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3etwuxcjs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jknuqnhd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ifozyrcq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zqocrfxb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hlufrnnm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hqiyrftf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ecwjhagy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3olpywiae.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mogmgsuy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3icaxvxmj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uejtnaqt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pllaxktv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yntwedmd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hhyvyzjj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lxysoqfa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gpkrckow.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ugzqghjb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xamejqyf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zlptierj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jyrvvonl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jvntzrmn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dfuxdvzv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xtzxwhaf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gaogenqp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxkfglju.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bystgemi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ngbkefou.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znbmftbb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ldtdqbfg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qaiuldsv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nioyerdg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3gqqcdaug.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wxtsfxkl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3hlcgkuds.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xozrwpsw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3isbdumkm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3duiwzyun.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bhbnwwrb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zmvnhhgw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iezzomij.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yzrfnbdo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3epbitxrl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rycyprhs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkqlrkel.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dzrdcehj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tchckccm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzafmeds.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ipgqrecj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ifxrzxhh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bllrbmwz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3minltmkd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bfseybcx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wznbjpvz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lksiifwx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xmgihlog.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kusevotc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zaetfxkv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vguiedhp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vqrhryoy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rrhnfhlx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3anauzirr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glsudvpn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3egjkfbze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3deatncph.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3apwdsdsa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bdqrlcyt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ssuxbhbq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3elygkrsg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vvwluazu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dxqamabx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3mcycaywf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ucybcimf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ijveadkn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jvtkzuqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cswkdvze.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3beheflcs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3udfzhpvi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zzmmqpqn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xxwvpghb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3exesmexu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kfirpppv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnzewtkn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mwwwlvsa.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ncdpzqdr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3btyzetco.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dqsiupzl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gebpvqgr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3imnbrcvj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hjzrafes.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rumdrvpn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ulrbhwox.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3moxlyvij.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgevcbgi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rucmljym.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fqtfqdtp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jiqauico.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yvmemvqa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lbqhutdj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cyueawqe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3sgctjvwq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hcqhdbhe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nsfpojcx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xuylbmiz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3olujzpub.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kboqjdtu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3clrukrmr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qdsxuvow.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iiudgowa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3txzkzogc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kuiwmrcw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yedlgzyh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tsaujjhd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uiayonhs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qtacmzpw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pduqysun.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rnbcltgx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zspwuxeo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qdqnfnpv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vzyqloxx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3porezrkh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qivxszei.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ogdxusqf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxlcnwmc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uqtecvbr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ssfmvyax.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xrddzbsx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uyepoxfu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fbonmdiz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3odqoyebu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3njjmqbbp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qrcxiofy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hsxyjxrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ttqyccbu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pyunmrlu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oqqlvrbk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3alhgllsm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nzforcfe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cnkkajdo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pzvlkkss.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3czzgoxtd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3aredhhhr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qlliraog.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rlgafadz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3igspuxkw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yeqspjpn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tmsdwocr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lpiwjinf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hvujhtta.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ouozhdaw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gtypktkm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rlixmpnn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yqgywlki.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gyizoedr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qmjdfwkk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ifksbwnm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3snxmnjmq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3euhgnbia.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3utovnzzk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3injtlozx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3khkisahp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hypnidvo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jhdrinas.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3druupeqb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3xdvspubg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ukxiopem.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tylnhvia.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bvistzhs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bmryiavj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zbkgqhlm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3caifesox.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwmfwtcr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3huzvigjr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hfptmjsh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ivrqzlqx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3epiljgxo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bpvyfgkl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxixgozf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnmqphvs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dxjkcxob.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3suujbnld.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nclhkrku.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3aubkvtbb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3equwonsh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggknwshy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ivfikgqe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzrxibin.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tyiloovk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eiaevfgd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3toywnkpk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hfmupymr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nudolvls.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jsqjudgk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jydphgpi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3etxkyxrb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ikznvzep.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3azzvliix.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3kaegldlu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lnoawpwa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qqbrqycf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3batetbrq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvsttsmw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlierslq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vayiilet.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fcrpsvdw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dzeujtsq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3itwspsby.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3qplvleuw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uiumhvoq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pxfihwej.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nndgqhfo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3smuxisoa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pfczzylh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdsbky.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3grgbctuk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpcpucr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wgafdteo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ptwngzly.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tutuugyl.html


<!-- 参考信息 -->