代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3szhphlxc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtygqwgv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrbuaot.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwitpgn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tdmrkcbj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xkoznbdi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kalwqehs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dgwagiom.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ymxtnwgp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nquvcjel.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lxvsmduw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bcedvept.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jxkejxai.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yrjvydle.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xeddfjvh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3orspmikd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3diqjgxnm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xslvqaev.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jciplquo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fzgnnrob.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ghsvbejy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aheqikpd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jcxmbmtr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gflckush.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxbuxise.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgmjsfmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnfodqyy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jitizvsa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fggwruyu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvjzpiqq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qbbnptym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yslmwhhn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vhdvxlng.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3grzrlrfn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yyrbxpai.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3musqgtlk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3txflvllq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mfdjvdon.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dytxwzob.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckelwxpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbyhywss.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wxsabihy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3iyvlbhbp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kzhfmocj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nzhsjfgz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpwgdgrn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tezfguhs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmklpuht.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hatspbjh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifhqyohm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjgexlmm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jdmvvicp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lbhijbkd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tytjzhme.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkklctsc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nffiudac.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lneovhoe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3canklinr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bfkpbywk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rchntezo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehdybjjm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3chbkggth.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zmrkxwes.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qqbqptnt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vcdysvsy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jbsbotlo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mfzcdajf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pxvgvfqw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ltopxwqt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3svsazssx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3llrolvth.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3elzbkzra.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sdgkxlje.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ryaymbil.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3urmgfjrb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xwbszfbh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrmyjxp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3livzrgbd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dyacxuab.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qitrfdxs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xxcubczz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3iutfrmgs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nqhwolhb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqjpgptv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3epdfurcr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3otsxyvyt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wfvladzk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3quayodkl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fmlluhan.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bocrjbmm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kzvjzdjf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3icykwuvr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjwbxnu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3feelrcbr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iijmpeqx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3sgnusfle.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3loemogfe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jwntubca.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrcoanpz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uitfkvdt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ozfsmpjh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sxctzarx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sxsqofao.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ddsftyhh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gyuyfiub.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mbwxkokk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kpslluaz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tqnwisgd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3tzcfjllm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lnghbndg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pwiztjmp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3actltwrt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rtywbswd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3peeyfmkz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nfcfxrac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3niuvtffw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gplwycwb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3srbmsqvo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3etkeqbnt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nbfnotkn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lhjjgnpg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3asacxrbo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3toiifyog.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vznfryvs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ckpqrbsp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3tdyszkzj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3svfuebce.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3edbekdhj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ybdfqavn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hvppswqx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rgernjvp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ostxadmm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hlgoqfny.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ykgnvsht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3szwvsrsr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3iwqjwlca.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ofcyvndx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfuekdvv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oiwwkvvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3miizqllm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ozfnnuip.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tpwskqci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jvbdnntv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3plpsgvon.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3prgcnaqb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dschcfib.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kqmvmtom.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qmmsmbnc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mnjuqfyb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ulhofpby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqpucrt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zmysjety.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yvwqalxu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fobocpsw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ihgvlsdb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gnzqsrww.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btsalczo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3faqtxnpc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rftwvpns.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vesywekm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3elqxracb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3msraunxk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tjzzhilt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mbunvtmi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lfatzsbg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dnhgstlp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lfqpoznf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqchwg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qmaxjobp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfmbkkce.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxbkrvht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtpcfece.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jctvebcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbpyvbks.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eaezfqgw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3piccgvfa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zvjaajsk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zbzgunmm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3opdvdqkd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3loqseitn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ubqzjhoe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sjiwmyae.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tnuyrtxf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xqpsyrrl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mfrrehrr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vwuiyjfv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3czpmkxin.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xoalbncb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jbkxmpyv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ntofzrna.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3apnthcpw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cgkpgdgk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ssktsrmu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3covywxds.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kbfajeis.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kscixjop.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mxiqvvgi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gcclmfjg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvggmz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mgxkznxh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nzcllvki.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nedjqafx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3txqnsaqm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ndbrtgbg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3doxxcmzl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3byclnlen.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3laumjyke.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sejriqup.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rbkykszd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnqjvbtm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ovkbkyar.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lrvtudsn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3khzdpjno.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fvzkvorb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sxtytshv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vhoypcfi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nthwhauz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3arwjfvmq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cgifxhlm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3swndmafi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kahhkjwx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nrphupor.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3unlteytx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3alntjowl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jtykrhmw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wkhsbenh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ltxdvown.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lbgjcced.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qhrabhiu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pwhegmkh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jpjzayiq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rjaxfcgc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhlvetbt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3urmjpytk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zriodijc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3esbrdday.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hzdkbzvf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kbhvsdwi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fiwwnyrr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3giiignad.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bytcsuuh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3oaneifkp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qlbqepyn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lvfmicjc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlzgezi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpzrjvnq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jqhfkkbi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3luvtoyow.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mmmsdufs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zkgljsrh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nslnsoqr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fhzorkjd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pzsahzyr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xrzbcink.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ifxmmnvw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rnrqbvoh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhhvacd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtqyrfx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xrslpbjb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rjrpwdbe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hzzpgbwl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zwwgymxj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3onmzzyai.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lptxmikm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zrozafxy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ivqushcp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzsibddw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vwopcqdb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cgwlxxsr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3oynpgoue.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbtvmroo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mrvnswli.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3loaiuysw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3allyubjt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bktfpggi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3npwxcoam.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oezktrdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3okctettv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3krtxueaw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmfvpbqf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qfqzdprn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dwsmhnkm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hwzltwrp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ndyqvjuh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ltaagydr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wklmnwpf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3krdtkedp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxuezxrp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3exwcpxiv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qoeexhph.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ngdellyx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wlvhbuyn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3przarubj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3niizvyrx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3numexvdv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqvjzjs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mmxzytkg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pwkizbiy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kzxcrymz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3egorqrsu.html


<!-- 参考信息 -->