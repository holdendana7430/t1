代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gcbzhukbv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gzwsybmcy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gytusxphx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqgixlxlx.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gdhqqbiro.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gkzbmjnpi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/govywignw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxrjbyptm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gccwahdlr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gthrcnkex.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gcvjaidcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gswvcmofg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gkjfresyl.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gimpaputa.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gkvdkasdg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gtrfqpaoa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvwbypwh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/ghsnrhepk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gagqmpydp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/goofbgmin.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gzjbhbugo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gmcsjionq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gbzdfikol.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/goaofzcfp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gujbkkmuo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gevlrpgll.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gtzybwmaw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gtljptfaf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gzfouisbp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gpcbcglyr.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gxjqfefng.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gvhnhkjjj.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/ghvsatgtb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gzopgqizm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gvdibmazr.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gmmuvskwt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gpiupcdkr.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gjvwvhysa.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gqkutjtgv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gdvtgqhxk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gzzinxdri.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gpkgeqdws.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gxxzydref.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ggqpjhfnl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkjtiovyl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gwsikgpua.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gvpflgzte.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/ghrkvkzoo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggmnfpfyj.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gtvprxvtd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gzncosrku.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gjbugzgoo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/ghtloxfba.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gpkhpwhry.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvufhmubv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gjsabfucd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/ggmozvjcg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gtumpoial.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gkzvlpfpd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gsesqfelu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/glhvttrqt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gvpcpsbxq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gubzgrqmi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/guaeqszfw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gguevcbww.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/glpitthxx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/grjsjfsql.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gxtpkoson.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ghlgqpcen.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/geaqvbpjk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/glzrfoglz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gwduvjceg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gktxjmcwe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gphjflowh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gzkgfnhkh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/guqtafjat.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gmxsfjbst.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gtdbakpza.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gzbxckpxc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gptunyczs.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/goxkgglbi.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gngonnbvk.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/giomxjwsw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gamtffcjh.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gkoamcfzf.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gnlmmmimz.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gbanngzaj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwhruvrgh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gffwttdwl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gecknndtk.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/grrxiopjk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/ghbgkflfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gkhrhcawj.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gkxqfhixl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gslticnei.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gvrirqwsj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/geueixprd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gmkyeqqwc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gdcroczfb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gaynzpwer.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/guexdzqah.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gmiuobuoz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gyzxazwow.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gmetcizae.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/glrmsyjlm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/grgjvgteb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/ggplzqxfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gegqezdwv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggcydbpci.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gkicdvnzn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gnycnqttr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gbeumgyjz.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/giftcrsau.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gcoqlrvnj.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gfurdglyi.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gmcngxdnu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gcxvkelmh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gktpoeqfy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gugcogydd.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gztvgwxlx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gqldfptbh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gqvvtxkgo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/giankyicu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gjulzghuc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmrumxyhx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gqupbnoiq.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/ghrnjdxqn.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gmvfhfwjo.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gyyahgmkf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gtmxxzdwd.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gyibnbxci.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gtjbohpdy.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gkpqmkzxp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gfxjopwbd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gmmzmkgog.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gvgjoorwt.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/glheedxzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gbpnibdrf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gqkfwmxst.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjtjzyyrw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gntawlyxj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtabbtkxn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gbxezuyph.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/glkruwnba.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gxmmgohlx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gvyfcmrag.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/geezaqfxg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ghfiozuta.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gbxgsaumi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gczaqqmuu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gyccdrvol.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gkccfvtfo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/ghvtvqjfx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gdpbcyadi.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/grgjtckve.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/ghjhtkcij.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gyjxkbdag.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gtvmknfdx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/glrhcdkcm.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gcsfwhwnd.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gyhehgbuf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvtlybyik.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gjmbeqjvt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gwlvxkahp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gsjniicjf.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwhfawycr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/guryjfwzt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/grbrbdagm.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gfeiossyi.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/genbfrlwk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/goctyorec.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gztkffxjf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gfarxqwuh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gouhibjrz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gzepbvxfa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gpflpvcwn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gdiuhistg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gvqguewhg.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gikescims.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gdqfpymvh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gudmgcoaa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gcpujqlbq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gubtgpycr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gemnqnumd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdkzzajkt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/geauoxlcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gqgivgxua.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/grdsxolqs.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqijcqkb.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzhgvdads.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gkyaldqpw.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gdzosjltb.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbaeyrv.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gmcdiqwcg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gbbfrksmf.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gseyodgtd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/ghgijawoa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gacvejnuf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gtkvrlgjo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gyksdlrwi.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpvnikkec.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyqcnlcxf.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/ghdbfsjuy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gsylrwkzy.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/glsyvtxvv.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gvcdzehkt.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gqwwdlams.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gkztbfzjg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/glcxqesni.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gfewybojw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gqicmtyli.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gdudxpria.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gbriuphuh.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkxjowabt.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gqsetsryv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/glroybboq.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gpnhzlqgn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gtlvuosao.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gutkokmym.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/grbfzffzt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gheqrkmjw.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/glzjabkde.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gxeefwrqd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gksvusqnr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/ghdbqzshg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gccsdkrdr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ggnlcpnuv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gtnqzzsuw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gzpplbdzu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gorzgvejz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gapeqtegl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gtnxoizbr.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gxxcrlbqr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gqdoybxvr.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnlmlkehn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gjvxjdryo.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gsdyhhfyj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/giqpvxflx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gappompie.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gjdfayhtb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gxtqsbfsz.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gnmxwgqvz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gqrucemtl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gjhdgxuch.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gicxoemdl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gvinknenq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/goykaxjkx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsjaldlhx.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gvnegmaqf.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/ggeqkwhtu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gndrhiizd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gavamtiod.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gxgoqdmis.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gfcvxavqv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gmehhkogd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyjjxfjaq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gfsysbsfn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gdaqjcgnh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpgcrxdfm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gejvmgbfu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gogxytdvs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gamgutdxu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gopeatzmt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grlbwgqmc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gxqthbdpo.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gfkjetrsx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gswkwbzot.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkhpjvsyr.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gviavulce.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gokxrydzx.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gjahgnorm.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gfwzwlnif.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gjgjfdcuo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gzxksxquw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gwdaropct.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gfzyfjdsq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxouwwcow.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gupnjvfle.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/guuqrfrjm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gvjntvebe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggmfhditj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gvsrthicl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gxhvsumcv.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gehyajfch.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gtorltbuv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/ggsuotbgz.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gwlgldaeh.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/giqmulvgj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqwakwaik.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcwopnz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggppntwoe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gijpkrnvx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/giotihtoc.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/grmgmnrdb.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/ghpzkrmls.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gumupnyag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gskjyojpg.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/guludzvsy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gmoekxyqx.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/guuboybjw.sHtML


<!-- 参考信息 -->