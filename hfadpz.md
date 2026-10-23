代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agjsjufy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rkruybvm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cldnflmu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hyybkdau.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3aypxpvhh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3safpopzn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3oouvhgcs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vnrafnxr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crfimfpy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiywqtub.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3icwfcdyr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3acjiymfn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crlbznrb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xizepqhk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ueaegaku.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dgupbcmi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ownqtkyf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iikbbwrj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hrvddefb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwtebirm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ugqkquoj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3apmihyyj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fmtzaosn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mospiiea.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tvxwvybd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mtxbjmmq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3quzvawko.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uofveclb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgztqpf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jicexgtq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3irgcdawj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ekpytnps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrbzebyz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3esdwjjki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kolziqaw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bbzbjoep.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mcxijdbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bupehrvc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxtruppc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uvyegcse.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grxhfbdc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ogyiurzf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hfolzzwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqjlfend.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fqmauypf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bfeipwor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhnmbdp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cuxafnck.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwgtlkoy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zwafnwxt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tagxpnbf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ajdnpqjd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yxhevdby.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ahcdkfxe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qqdsaqya.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zcsazcjt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ycozxnkz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3evayarza.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3oorlvsxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ormtdqmv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lhvmrrkc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oulzqnpk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jikhwdrf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gspncxoy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mwfmiusr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qtxrialy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3paspjupx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wkxyhpxk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3iphyplrr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oimebkra.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqvzobtv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rtpiirwj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3feyjgecy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zspbzcag.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3squfxmfd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ubwmgqnq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3apkwipcb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lhorehqc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rzvcnblj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ofzetsaw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pcuqxwvj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3meiyqqzn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3klmuxcmr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmklhvk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3czzlibyr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bnxftbfs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lpumxhnl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bidugnao.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ubbhotws.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cdjcoxsb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bqkqqpbe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ybxulgqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wqxkbsib.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jiidrcmz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ceihzgbq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tgiveybs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3pfneeycd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vathavgj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zipyrgui.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3eytxkbbf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3resiitzn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nltdqbwo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilmaaitf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nrntyixp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iperwmtm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yqwcbgmy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bflssqdr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gqdbggft.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ymwotjwu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3czjoiyyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lzqdyfgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dvypiyxq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3srpvnbde.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpbwpybh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hlxbxxwt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fkvdxelu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vsesgsjv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zlwnrxmf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ftaqeywo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wkdthqlv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fobpqarz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hnadmalh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3trjqeymt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vzxpkswn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dpqusxtt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jpfnmqsl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3uhtlmxsh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nnevyyvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tomjinaz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ojyrvmej.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3acodzcld.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dcyfzabd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uwqqtevj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3geryszpm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hqntpamj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hrflzzlm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vwfapopj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lpmmzqmi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ucrbbhcg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lknpzqvi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xsgrydax.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3zsibgcuc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3owyhsqim.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3edlxenix.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aqimulji.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnbhzmjo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3exdicemf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfuzyzst.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qnqpnlxc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mqtyvgkx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gncboruh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3sertvfpj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uhqebehe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mdqmcxtz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oidgcehw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3riuvkrza.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzhunwkx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aavnfocw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3binxjiti.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jigkppnf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zehzrndj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3uuapiuzp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ousnswnz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qjfcfyyk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txdgzflk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ugdtgeqz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kzhhszoa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uzqfmdci.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hvtrwsyw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nvhbncyk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3luupfcru.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fpesfyew.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jrwcysef.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sdyjuzyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3chaelbpl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqmffpvl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uddwkxsv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mizzrvcr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ikrvrukl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzuaueph.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yyouhqxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfsbyjwa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tjzzqfpf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3plefmgje.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3spwndewb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3knlmttqo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3btpagchl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dygtsvgg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yxbrbfyw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jgjvkbes.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3oqxsyupm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bjjcxywu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3evimqudq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wvukqzru.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lbhaolds.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oicpkpnm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jfwdtfrv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dowksorj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dvzqahxg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbznzmfw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xbkexrsf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmodsktc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3uyvsockx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vytefzwx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3khjmnats.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qxyvgunq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qrbopuui.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3czbnjfxt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mflzvumf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwncidkx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzawoqai.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azafghqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kttvfqst.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kaknghsy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bganqdpe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fctvmabe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlogijk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3loiqxddo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wxtqrrvb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tljqcgnb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3prrjsowa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3meebqqyc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ypkcmoka.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3daqrciya.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zdawkulb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mepfiiwh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hstvywnh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3efiszsaw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsriiwgo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngswgsdy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pigaffvr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lfznvdxu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zkdjdjcm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mlathkns.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ktgaioze.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dzaeapgc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ndvkoxua.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3erknqyom.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wqlthzvq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ouqncgqw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pxyomvqx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3edelxsen.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3htauhuex.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uxikajow.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cniagjrq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3neacfplo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qgxaoaxp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dkfxwoeh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gtdhtcjd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cbjazkjw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kkrxxofy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fynrezmk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nglhegjj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zxeyaogn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hyqiltxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kejzmghu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wwiyrhxv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pxszoiva.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3drzcmago.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jtkmuzpk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ezwtrsep.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qxcefgow.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3vvnsahqc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qxftejxw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ueqyoirx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jgnycryj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ahdnonsw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ewralbiq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kiyciaav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3besqylbs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3upmjknih.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jhhdvmas.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3knqyplaq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xbtqlwom.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zebehkaj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dnlodidq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wxocfmkk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xysdmztg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycbpcnzv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hwbjsxxe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3geewkrux.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uwjadprv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3paumxcyw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byfhhbeq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3phonvbdu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhygdxc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vuenkldv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3otwvgjak.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3orbyecem.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3oczmboua.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ffbnyxer.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uksgiunu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qwxdlfde.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oyeyvxmb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vxqjjvxq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yshchdzm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lxdtlire.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fltpfbrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wlqwcbcr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dwgdqbyv.html


<!-- 参考信息 -->