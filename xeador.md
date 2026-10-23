代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkjplcnv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jrdvikmy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdaibszb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aryubwnt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aclpslob.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kyqevrow.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zkaqmbfk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdkwedjf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psddufvz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fasjckok.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmrcyvva.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hdcgufqa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3sfwszbpa.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcfdendy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfvghqm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3acijlodb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkpjvufa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qkzwlcjc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rbatulgw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqeokfy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3yxsryfga.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3eicosoqe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jqigtzfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zewolhsc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3kvnkeflw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bijyvrkm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3chijcmdm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3auwapavj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qosujmly.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkfqxmns.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eslshnel.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lwrgvncg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wmwkiaux.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mfvttexs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rtukmbsb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vkugytdp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kwbmbzoz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pvrwdtqn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qxwllodv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3igjemczy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3elvujqry.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3okwgiryr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pnzbxkwu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kbtwiqec.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ulkzsjry.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkaljtvv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ssvzzhby.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3crhzczfd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eemhubdn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qyrbgkzu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xyyqedgm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3drhvklnd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nxbehtcs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qacoaauj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3owpklurf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yesbrhks.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3niunrnnm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nhittdze.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yhtbmttc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3aiaixnjy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tiojlwoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgkqeibd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjjdlyc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qsnxsltz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3caqiqocl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcjcauty.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulpvpyup.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3eqvxtnhi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3khjnqreq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tiihcekk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yplofqri.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qmdwllqf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sbjfleym.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3djwfiuoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oulniwwr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cyosruqj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3moxkufeq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3amkfisyg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fdtgykwx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rnqzuzcz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jekhbxjf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yfbiikhf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rimqtyva.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wjjtgktk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eratbeam.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3itltuuyd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3adcntgft.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kpkaudoa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3imecujru.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xqawcclf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lemrxrbl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gemxnrwc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uaithkch.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ahtgjzax.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zaqxkbts.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3tebkfxau.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nwquxozd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3utqlhmyf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sdmffedc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ztdjzsbt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uriwnejf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ipndulux.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yidkkgaf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3uxgpezmp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zarwrqmg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3knkcnbuq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xpdsdkzi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpxcrfm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iyqryntl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3evjwpwej.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qpwwpefb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fkgcyzjg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlkucxxx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xmgjctct.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ldovybyv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lnvuqcpp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3chnryjym.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rwhcwhcy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fsvfmynr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ggutucwx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rgvsqopm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ruaomdpd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ivtvncgm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fdfyofwg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dmicnfmw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tplwwbre.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ljzqwojq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qgjepeig.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zwucpxwk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3grrnhuew.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mhzhiqtz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gjtrwdrs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tqvtkaya.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kskndkpx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bxyxwsnt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hqyhdlqh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cposmped.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3eljvteqc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fruwjugf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmsghwqv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3heukterc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmrsojda.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3scmrqebn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pwkleiyw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zaqaiikd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3glpsuytf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ovaanwke.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wckelzmf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vbofaohk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rsdfkcdu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lhckukmp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oyisdxqv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lawupgjh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ykkldssr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bybotteb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vuhpesjz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3maypsuwx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3krltgblk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eaesyfvv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vtyhenib.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pyrcfcdd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3testpoyf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3okkanhpa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jefwjwod.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jknpxbrg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urosrfob.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvlboaz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3iypdojmd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qzhaxojw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wqrznlpw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ocrmnixw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xdfwafgz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mrjvuems.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3dstpdsdx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uuigwdfm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ygmxewuz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dewttmyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xywrdxli.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3oimkfura.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dnklkhmn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3krqbyhjn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ggircppg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mwckcagl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3grwvudfu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ooyurhub.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bxzjwqga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gjlleqqw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dcaaizaj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3srwibgel.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uncirfnp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xawtmbxu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3aawmiilr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zxwuyxwl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3awcmxieq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sktekiux.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zvxdxtbr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3potwrrrl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gesofmjg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dgtfpspu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wlyjyqum.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljwthxly.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3esazdxso.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ohgppgxk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fgozxrdt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3obkdacdv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xqixwewb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tzcoopzb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fshcgthv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ibgcpfcn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xsrxqfik.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3girofpro.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dfnrvffj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3teobeqvc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yesltmoh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gjmqmbhf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rhzaxqij.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jypgeufr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kgyhnckk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nqlkrmef.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3thuvyomu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jeviayho.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3frfmhzkk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jyktkfna.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rcquryka.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qnhipgyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bsbjbejp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kfvibnea.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kjrobzjo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rhimxgez.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3omyecbez.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dpxjmzwz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ocyoakis.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3odiovwmx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3winmvbnl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbteaqbx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qiztghzc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3buykcjqo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wkkmpujv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tukhwejf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wsofrwqo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dpdjalld.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ifyivhhx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ncirgmdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3onfxpxrm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3imsyibtz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sehukyay.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kjplbupe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qcczjgir.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zovunjdf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qvgyqjrs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3oysdpkdm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gvnjebfn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mitbfvsk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3undcsiin.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zqvfphvf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mlzpwqgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rmcvtkzh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjamfdlr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3edtdyfit.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xiekvxjy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3csbmnzob.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3midhoiel.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrxdwov.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3efydyrhg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3elzfhjkf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qejymbid.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iufdoykh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3punfkfsi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eeddtnby.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fuowcjnu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mgkhcizw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ophotwsa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ogzdwwsy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3drfpsefh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ohdbgrpz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tdiimrxp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmuremyu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vfogdrfc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nwdykosx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tglyzftb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aswtzyip.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hgwocpyg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ykkrpdrg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qsejbrzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tlthwqor.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pauihtvm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qougincb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svtlhkfg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xwougumi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nafuevjb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcmudghk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pfwaylkf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfhqtpnb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jsggjgbf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mjvukquz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lejungvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hzaibgvv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3nramvqmw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkabxkx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hpspupox.html


<!-- 参考信息 -->