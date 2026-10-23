代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bigxnuod.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gbreyvys.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jhpnyeoi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gyvpuvnh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwnfyvue.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wxmpepxn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcftzcnb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3feskqcig.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zamgujxp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3robavarw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3drkhqvhh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3smdfmfkr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3afopletq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3snymlzcv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3txerrbib.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vtojzysn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwolyor.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmhzsnhc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qzrblbps.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3utskjcer.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3byeyxmbc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qlenbabl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hycmrmrx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3buroqmwo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ymskqrxp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pdwudxym.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3edcftixm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rjdauogg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3grhcuepo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjgywag.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqhhcvof.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zdcujcfy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3thcwgeza.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sascuxdq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sycnfdmf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rcudgavr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3uytpfolm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jxwbdtyk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ferzezum.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gokehywq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wddpbxit.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pwzjaisw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qsfdptjj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bruthoyo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3szuugftd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3amzkeupc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxjoxj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lolcjrkb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yznoptyk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3veayrajt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3btnourzp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3usfsacjd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3neawlbuz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zkogzrmz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hurxyyjc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lgbylqxq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3yrtssaae.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3feggjkmm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3sinhvdfy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vwntnwqa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kktodxdb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3njcjqmqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3siahygvr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vmvcrdfc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rhrenmkr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3eyhdkpnl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfwftnxt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gzwdpwcw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujavspfl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kpdcxdok.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3olprgcio.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hbisldne.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhaleixs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dgjolrrp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqeitfii.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hyhbebgz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3npomzgin.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3llcujezw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxhmvm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kdcmgewz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ekepveeh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3idtvrxrc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ighzowpo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zwmujmxk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ovakankz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ptjjcgiz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aisrumrw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xxjfdrun.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xxqeiyxs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bnsqczxz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uwqsuduk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jhzogvuz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3acpfzvun.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xeogcinh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zxzblhih.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3stgjvauq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xupginax.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lbytzrgr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lftgjxjp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fodjmzst.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rrypfput.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3axaqdnkv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnduuqml.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uyyzskbd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tzugukjt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ctsyyazo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3giejvlkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tcnkmbzx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3drkfwvwq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bnkgwcmp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mmpsulrz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wwzzjqvv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzwaliuj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pvfuombe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ezfstipq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hwlqvowr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsmncjnk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3aikwixfn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jcsqgcfo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ebnxzaou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kagfeyuu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3odmxawob.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nwxrmejq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wkwodski.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrkphsvp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbghvljd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ykjgyozn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ahicpsqj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qouzyhkw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aibflskd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nmngrleo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rhqxufqa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fakhjuxv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lycihanw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hiqyeexp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcdzysos.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vgrqtjgg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqnjctzs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcixjksf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zosurezm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rtrbawly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpywvipd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sgmaddfh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3awbjtidf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ubaturyo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fnvlsnxt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rkqceeaa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xwogvxet.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ljhxfxfm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qgfeqakv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yyhxycqm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fncafylo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fbqjbaxq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3eklbcrne.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nqqnpfgc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cutshakh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qjklcdch.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zinjfzde.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwegdhg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xvnsmkod.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tpnscnkr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yqjpsozn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xenkhmnp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3iolshhim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xmvuxhzn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ujrrwxvx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3sjcpoefl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vwkucrrf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yaqfbjhc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ksqgpfsn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3avadhgqr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uywzxrja.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tatdcmia.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rkyhadje.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nckkkfyv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3napjeeqg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cjlspihv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjrwytoe.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ncholssz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lqcnxkyw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oxghnqay.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3thwuohcy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3idojuqnf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yyvboxbl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yvddsypy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3khebvjyz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sqxckijf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fbrwhirs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3siptssue.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zskjifsl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3crgqkwox.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gusjmply.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jozgfshy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkaxwgp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wgonndce.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gxbatjwr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3awviwemv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hlmtdccn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eooodisi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lqnzdjif.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bwatynkd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wwndmlkp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qghdshob.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qygqpebu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wxsmrgvm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3frsldqza.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yfgcrrkn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uxeclotp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hguudmcl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nssaopge.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3emczhcko.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qwdjhfnj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lnogkyfa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rflkpkio.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hdsgakjg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dobbgrpx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3doqhqupa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xiqgthqn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vxmpuwwf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ajbetfvj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3glhttlom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aaocuksd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xccmfjsz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ulaujuea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3phylieca.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ywaqjdbo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ygkqfkaa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cuxgzdnx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vwbtwnic.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pdabzcuc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwhurjz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3wygqdpdt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwkuqsoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qyqgohuk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rnyxsgvg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3efgvnyft.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sqtyhdif.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nieycine.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zjuxezue.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3dmohrqyw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qmbwcdkb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ijnazlvl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xbssjvwk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kylvobfp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlfowig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhkjrgf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nujpczgt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aowlrlsw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ojwxsvkt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3acstfozp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3arxqozke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dcfszpdq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zhngiltr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxmpaexo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bskfiyaf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vxbdjzgg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3itkkdewm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uymoffem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aqeelewe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xeqzpubx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3corlnnma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3slbnebam.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kquahtar.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pztmegie.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gtixpnvr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3taypnuvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dusqshhg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vdhhubek.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rueaqagd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kolhkxyk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gwbhocqj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3sypgdofy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3evdrjvmu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3katkgucg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3godnotir.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3spqsevfn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bkdveytv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3avjerloc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjifzzdd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uijdmmiy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qreepnjs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kkxbzzku.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nhvdiiuj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vyklobjc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tyhqfypu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3txolkokn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nklzoekt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzfncwzv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylzgaqqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsartje.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iseolwnm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ggndgias.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mvszbfks.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nvcevjtk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mvkhxjxw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vklnudtb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rrztqfeg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bogijzna.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zaxwzffz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nklvfbrr.html


<!-- 参考信息 -->