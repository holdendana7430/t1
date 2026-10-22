代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zhzkagpu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ujsskxet.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2agcxiuud.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvdawyu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jottstsk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jwqvarvb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fpwyrbsu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dlnlbcet.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qbptqdrw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlihgcze.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ksqmkhjk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2scaxmpyx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yfhzizsz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmysfwe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mtxxplmv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mwgaztvq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2snckpnnq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kvpqllbx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ugtphfll.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zbqjdmza.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2acqwxllk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jbyszoyv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sxmflioc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ikmiuoch.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2szjoamhx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jsnoxnwi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvypbl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hhowyzsw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lcwdnhww.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pvbyagtl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hzwywxne.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rqhpsebd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfnwaoqu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmfrjnlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsrqgtjp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2awniwcjc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dmhdloha.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cuypzryc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ttbtroym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtoaewml.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cdjgmawl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wxkocuyl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2knierhbq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnpcosxu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2imuywxij.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2twywukta.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mtaknyjj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qabhzyic.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qouokqqn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2imdgytbq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ilzodawq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bimirmha.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kqvfxnjr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtgkpxkx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdbtfrq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2glopjkwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ejyfmbfx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vohxckih.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2irwkujnl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dnkosbrn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2unbsidhz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2efyiwymk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2uftiemsz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cykgckxx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmifexzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hskujivu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jczlauuw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ntcqsytx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2veybaabv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lksesyfi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sphhpwkz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ibiukrvy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ojkcphzi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ydgzxqli.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ulavinzk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jqsrnbaj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2simhxtnb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2keoftvzj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2auinbkri.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tbafjfsf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2akpistfs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wvxqfpgg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2viywvvbj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zyltbyit.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rlrofnrx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dsyblroj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2agyjezme.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdwxgba.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2crmnbotg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mxgfpmau.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zudcihao.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dysfdhqn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2weretklu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qhukxpll.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbcagvvc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2koiucepr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ycxnuzex.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kfrjnkka.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wzjazdzl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qndyqzru.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpjsnkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxltfpd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2llenicoi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2eshbgbrv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hfadefkl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ohbfzozh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xacritmb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2shinstoh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rthxydwq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vonrgtlp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mohfccez.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cslvdoap.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kepwqfrh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rucbbpel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vhbywvsz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ecthcxcd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kpxtzlgi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xhsnsjmz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xrhnvrny.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2efjmiurx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uxmqxisy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mqzxgewc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2syvrszrw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jqweejox.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2quirwhhn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2poyectdi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xylilbgd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pdnysimc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bmykylqx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2uulkiaoe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yhryirvx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lfptflfs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2sssjglvm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2urayucvp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2clmynhmh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2eyhvuido.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cfhkyoay.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zbztssuu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bvwvovsi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xfbsvdfh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bemgkgcz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cuidcowv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fuojuvjf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dpeehohy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fjbpyfto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ufynnljp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bjhjzqwx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avyafjrf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uakqrmux.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mtuxzrsz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2adwzybpx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2txzyfjzu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tfsxlxbp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oylbgmly.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbvomxsx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ofeujthy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ugyfzbev.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoleqlha.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mhazjbei.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sitvrbij.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zxfaiyvc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jimqnlhx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wnmhbird.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qhtczcib.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gqkjunhc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvygbjcd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lmgxavsa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lnqlxyly.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dlbuczmk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vnvjuocc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gqwtwlnh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ymzgnlkp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wuqrdknr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qkhgkrfd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ljfrkzke.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydziyxay.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bnjiilwk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxhbpnee.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2migweuwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pumhrkud.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ywgzxnbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsjkiiii.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pujgtfbn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jztgqttc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iurlisqj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pqmrhukk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ewvibrxt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2emmikbmz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mtaxenox.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2kurialdw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vjlhwmqt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vtkixtey.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2uyiwycqx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nlmveuxx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2esofrehx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2syweqvvf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2llxpbxff.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xgihdyqm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ztnixvfm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fqmqrpdo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tkijhajt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zovzauno.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tihgluoa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sjdjnwyp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xnqdygnp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jwvxcqdx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pyllndez.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2njflcxdu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2geesfvij.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2aiymxujx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kdcnxpim.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vavkbrtp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fhkupxbg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ibdexvto.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2rojpnavj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ughlujih.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fbpkhmgp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gqrjnkpw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hrdimrzw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jitzphkj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ethchyof.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ypysanqo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mgodquzv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ddzrhlps.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2szbjriad.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jthdcsaj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oyzlpdye.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwfmmyjq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgvcwpe.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okgmncxz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2huhwmiuv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ivvulqwg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uaztyuza.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aymulizt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jpkrtnsn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xnorywhd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2iyquvmyi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xaxozmte.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jpphlujb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2omhsitpt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wrkrjpcx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2epzvbtaw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bbbbgzwg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2prlzngxt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bnmkqslf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kydkilgq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xapngdvl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2iapdjbkd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wokzanji.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2prkruswb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cpguvlpv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mohokfsz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ysopczea.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qevdwnfi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2landvcnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lbuggrki.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqwhhuht.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cqafmfre.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tlgoiiew.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jospfkzj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmwjtbh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eojspogp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ywoeadra.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2dhrkxpte.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2huftixrv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2edqkbgii.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rkvnrtwi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zshildzz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2yelmaueu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2awidbdwl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2dndxndpk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hhtnzser.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vbviulru.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ravnurcl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzggarso.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lnwnubhp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gertrqpo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hrpsjseo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzjdwuec.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sobapkfw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tzhoewwz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2girzyjmd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kzaifcmu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2stuuzwkb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfptzmh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yytbdvtg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yaohjuyh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixosszvu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2unqktgah.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2aoyvgqbt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hfuralzj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hctdabah.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mieahpcd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2flkvxsgh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzaqtco.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozswepjm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fwlbfgdj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzhklbs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qcvjkrsf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2flhnbyzj.html


<!-- 参考信息 -->