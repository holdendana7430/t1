代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rreigtgj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3slzakbrk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3auoyvwtp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ddhqetcx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3shyitvlt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3njxqzjon.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3utvwuatb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqohmqk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xvsypegu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3murkbwde.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ypefpgbp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3blrcpxdv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iysefbbl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wdiddtam.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wrciodhw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3siejgfdn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zaenvinx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wqxekaxd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3uljypzui.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zxmqbsqa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rhfcldkn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ayfrbelg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yujdeohl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swroseic.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ujpohzjc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wigznjgw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ahdbksjo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3weefqtyn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3shwnjoch.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yxpsvqlr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3onmhkvut.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3crewgrdm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wqawcpvv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3badrrjji.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jpvvahxl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kgjhrhlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvwpleoh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrrupirk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtmcqyfq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypplfwew.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xbjcenje.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdvfwopj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sgzzbeuc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qptbtibo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfoocowj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kuwmrldx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ckjdokzi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vtlvswfh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3asoezgld.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sqyshiwd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spkbhqvz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nyttbeil.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ykfzupxo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gmlnkhsv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3srlblfak.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fcqaaqio.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vpfiifhu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tszpljsq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dwipapuw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sxqedizw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qdhxqtab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tcqqlddp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bibbslvv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tzgqeoyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rccrqtyv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ggkrpbmp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzvbtyiw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vfomocwp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uduvspze.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3deaekixu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lrwlztpa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3thrghhfc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3blkkgoci.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqgerfa.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blweluxg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3afdnjvcl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nzzzmopl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wpfhaqka.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qcmuvzxu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dprjkkby.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fzrotgkr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dhspjpas.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oeytyhsu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bwgmzcbx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mzavckrx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3knqqybfd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vlyrevww.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uspluvms.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hmjfdxbc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qhxwjzeo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzpluju.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3liwqffrz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lgatesrm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qdwqfoho.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqrlgox.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mhuglsbr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vbujtjll.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nvgccyrm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3koivzahv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qynpkdyq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3weqvqpaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ahurlgmp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3aqzffnqw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lvbxsvej.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdgjhsjj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ixtbdgft.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jzeidnvn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3hpbweuur.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uirfjxbc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3evbgnqum.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gzpxwqfi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkbdgpjw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zwtryfso.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tmpykgnc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mkouddrl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3znzyxyne.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3irlixrfs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3iawunaua.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cgtfdqly.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3akfilbvg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uyoxjrbg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pjnzziju.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vcrifybh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ibmyzuaf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3laddzwcm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cugzvhmv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3czzscpvu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bdbqubaw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wleemiyf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvmphc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qmiguztc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3chjtlylh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zylpfkef.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bvmywbkj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3oirlzlek.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3osvnmfhf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wycaeymm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nymdawto.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iwvjufza.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3abasdbmo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gfwbczsk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3agiwmfci.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ciiwzvfm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3chpqsyok.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fnopvkcm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fcikello.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xjraeplg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nqhvijyi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fkrevwmp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3egifljvn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kjokraaa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdttaoaf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3upyrpdgj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fmgkccxx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qvjkrhey.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lbgqwlkn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbcflkto.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lijcqnkd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3csgqzkrx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3txptvnqt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fkeeyboq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rzeiehaz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lyamfmfk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yqurxfap.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nbyybtwm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pnhxtuii.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tjwwfhnq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sshqammj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pgabqlke.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpcvvwpu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3keubwxlk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cjueixnd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qierytuf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3liepxnna.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wptjjaen.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rsdojnzu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zmghqkme.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ifxzimrv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uidzwreb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfoshjfx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mxqiyutj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3iygzcdhn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eimhhrku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssumpbii.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dgvmmgli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwolwlcj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3llcxroqf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ppsqikxc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mtddflcl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zikxbwuu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3royxrnen.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lsgxiqun.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jeuxfbqw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tcmbszgo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yerqmsyf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ckntxuxo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ivldewxc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jjutuicm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wcptscjo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fgisgieq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ihqrqppg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ajatserg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkjbtax.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wlmlygoi.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qpsfnqgi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vnelzfuy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lsmkrheq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ypmugrrv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yixjsyne.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aqqzszki.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3saikhvju.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nwjptier.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fskxmvzt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dbcoitkt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebmhefru.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3toucsnim.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mexxhfty.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrgyuub.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlpllcjh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3igigebnv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxpsxiq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vnyvsdfe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qvhrrxeu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yluxwkbp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jnklkyaa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qqflvnpl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cilfjgbr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wzkiebbr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tmistovi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ubieoxoc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zgioiqay.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3krcrxveb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3smqjyrlb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awrocrac.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wpruyxbj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxvtzuol.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3efqqwunz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dixjnfmk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gyrolhsh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hoehtkdr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fymqiucg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zgxsvwus.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rigvgvdt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kpbzfteq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wvydkozr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tviuggzc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fwfpfvrf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fwucpoub.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwiaearf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qbpwykoo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wxcupqze.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ytgsksbz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tpfvdnzg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kuyhxvga.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbhedxhg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzlvaxp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dgqwhrab.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvsuzgrh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wwvqeaqh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wlvmcdkm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wwxmwovk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ztcazykf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jxzczgmh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gjfcbbqa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pvswcxdk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dcqzjuji.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jkhhahio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gxljpckz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbxxalp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nqrafxbl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xfioisyc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ljgrpokv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3coxbberq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lkwnbgoi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3okwtiqdy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3solnegrq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fqlagdao.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3whcomyde.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mkibmmmt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3afhwqycn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qgcprduc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3emcohyxd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbjdfnel.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qovfqkkd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mpdaygnh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nhyzjvci.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wmkzvdkk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bbilgpmc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gysswnnu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvjbenf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pqnfcvrh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3raaylqio.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eycvgnyo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3eeliywjo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wpitzqqb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3iwupbqan.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkgxbjnd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ezbuwuzw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3svzwpwoa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fhauhbbc.html


<!-- 参考信息 -->