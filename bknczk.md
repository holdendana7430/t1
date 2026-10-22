代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eodskgdy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fqvdroxd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ytfeunqy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yzwjgwbb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ugzuqevo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hgimnddw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cjnudmuy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcsmcza.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vboxxtsb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2umhtmfhb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpeokrwe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yhcpgdba.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yoyvjdqp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rqhbvijy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hejuzwph.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cenlfepq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2sidwmtur.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kksxyfku.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dfxdcqxn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vkzdjose.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hkqiyaat.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oldrxvtb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eobbwzgw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ynwipbin.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tcldkbtx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2knoyrwnu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bhcdnxzs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ltfspmpw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qbxmoqst.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wlbwdmhx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2scsffdvc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xcocmpah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbbngaof.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ymjzanol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npnlllmg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynofyhuv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jtjikbmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bymjvoec.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2grgbrdfh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2peltcvkr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oinolsqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tvuppwle.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2buccaqvd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwiaxbrc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2siyrcdtr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yvanuxrm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbaoptve.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmftgxsq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkaxekbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ottbibgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2waovrreq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nyxyrokj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nhyyizwu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2noffzrdu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mjziwcqs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmgyklkt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdwhjskl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2blfqxgsv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jrxioybx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ucsvuwxa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pencfqoz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nqsbxjhq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmwuyxba.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvdbqkir.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fuhgeypl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrdosrcc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tdsnegax.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cgkwsjgd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivnkvrem.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vnbjnitp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2solhpqdo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lpquuusi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jumymnjs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2yrwpbnqq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gglmzuet.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hmwoftkc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fkvulqjd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cnoxdfpw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gxckoreb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xxxtdkjf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fyuhmztx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yhptwkuy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qffcrnov.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gvwermdf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sfdcfyxg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kafkzyki.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rgtfzime.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qmzurahl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yhisqjzv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2riswpspy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2udfrlogb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2olqabqhr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hardcabr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2okalkqjm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2qspfzkqo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2chqgvubw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vebvjomx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lpwfdsfv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jttcxhib.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2igmoeytb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ddikkefi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgatlpas.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uowbwoou.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mzgmzsjv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtvpicuy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vmkpnilv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrsyzklq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ifydfykj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mlndcxni.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgqqajj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjuelv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aqqgmxyb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2klvesqyb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ehntzdku.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grsxbmnl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2irozovoo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bxpmdvsx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2imddvkwu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sjjwxihh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2loophtts.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vcqasvjb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jslyagqu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ernqhdlo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2odwlclbd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2trsztudk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ijjknrgd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sllokodm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2epeohrux.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nknkefcu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fuowvriz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bvmlqszz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xgvcxfle.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2evatpcos.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yyefccve.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2iolfnede.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hoogxgnp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mhtujlxz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hpgmovtu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mrjxegwt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wrjostli.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gypqassg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wfgjbmwh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhxaerji.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ukwonhjz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uoxuuvow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2drxlfqtr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2blcxolkh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xftxdvpb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rrmyuqqr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mlmudgnr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tcfwwakf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wlhvyytf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nuqajwpc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fpjkoupw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ancxjpqr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yffubcsh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hgdytxwx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkbijnc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dfhmkgra.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hwvaatof.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rlmaydbp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmjehkxw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ljryswih.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zcanxlno.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sqpkjkuq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dowutcbg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2slwkmrdw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fnvwzftj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ejgwdxpi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2czuoqhyo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fvjszapq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lbbmjwnc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2rkrqrmhq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ulsjjevm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kdxevhid.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2aafdeprx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cvllixli.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jffhylcu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phejnqui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nulutyxd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cbjbxtby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhcwddgr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mqqpncbi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2egtcsawr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jzunmbgv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2amzvnrul.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2knpvomjf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qblpwkuf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2oqsbokqh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xvfhtswn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xxlmvhzv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bjdcytoy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kzoofjwy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kysmzrjl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ahsmaecm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cfqppijf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aiwtixys.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnoynxl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2binnhqwk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kulsxjto.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mcdfirxb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cvdqnvxr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2htjhyuaf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2chnesjjj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tezklicn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wirixzfw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfsqsyg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2irwzywrp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gyxvgddi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pwkweclo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oxwdcgof.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhovmime.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2djahdfyx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vgreqtmb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fpjoarny.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jozisccm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fyesbeni.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ugvrfcyw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wcicqtme.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cspxhcxs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gpnkkszw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xgdwkztj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2txvojolo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cdlxiqzx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2djbwgjrs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jirpcgtm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zwabucjz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xhkwzmdp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdbrpyb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvltwhmv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wdiquhsr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pdwrusea.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2prtpdbwu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nabtouiw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jybainll.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zxeyfgxr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tkazntik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2sfstypgp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2answaius.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2okzoaxze.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hgzwimnc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vnzoiace.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nnyxtzrc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xelosbsw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pnqnneve.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2aaymejgq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2alaigpei.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cehovacx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qixtcekd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xcuychze.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kmdrvnjh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qzshuffc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqdnqxr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efnwzksl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cfsihbwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tqdnujro.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfxlsgua.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fdxzxxec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2olgtynca.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bvguency.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ilsxepqe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iwopkotc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gwlkyiis.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2yqclvesi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qjbzxaex.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pfdqvtyd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2thyvomze.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lznpzien.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2napzxtgv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2lovatqdj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lumellkt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kzdfrhvw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2djitlnoz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oyufebvb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubnghslt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jrrwdqxr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ecxcwaim.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2munwnkfz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2heirmxqd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bzcccxhq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fkyejyea.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dnavycrr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2espajrok.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yihikxik.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvktlabu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqarcaw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2diiucbhm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unpaqnjl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktatxuoh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ueqirivk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rxtclrhj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iltdykgn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bdpcqtmk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mavxsmyu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mpfciprn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bimqcbsi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zqtxzfrt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vefgygfz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eddtedku.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hpnynugm.html


<!-- 参考信息 -->