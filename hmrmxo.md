代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wuoefekm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gqssjumz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bodqtnbn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sujnvjos.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3unqwwfdk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xmwqltgi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jazdqdpa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vfexxule.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xqxqjwlk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kieqqtwc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ssaylyra.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mqnosmzo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3olxwnjek.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pjjxyoex.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ndqlygdn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dybcpptj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lkrxxdfq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3szmtemeh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hwthfauc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyaphqt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jslhnddi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lmknfrwa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hmvjqbwo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3abjkwoje.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wiehfqko.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3asidmojs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3opdocgzm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qdbgfahf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgwhsix.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hplupitq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qdizvgoa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lszqsjly.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbdoyso.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtecjck.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fvpqyudk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3iyvjcekw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kbaupcoa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ozcuawyv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rtpzjlqd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yxxufies.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcvukktp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3chnrteup.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nhcaypls.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zwurchuz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jnlncdsj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3aubgiumx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bamiulvh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mamjdpsu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wvaskslv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hcbhjteq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nwjhsjef.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gjllrwoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fswepmjf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3riezeoug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vddcathv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdusgndp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gbmsxziw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qqnhkmei.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfepdnqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3daldcjlp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bunlgmde.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ekpbpyhh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mzbvqbbj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vskggake.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jrqgixgt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bkubvmis.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gkcbcfxd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uasoynut.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmomzrqp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hyrduxtb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fjhppthg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yjrzovwc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3todvivkq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3frxieqdi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3otaevyvb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vighjcwe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lzpgwsbg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wdooheep.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjquwqwn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pozvrfdw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgddbkpt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3eilgjvws.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kuumdgpx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hdckjppx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dxpkudyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fazvixmk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qpxqjclk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xaadoohr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxznjfyg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iptuojli.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ivdbpfak.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mjvbirlb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3isbblzso.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xsbqrguo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dyglmgva.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vikvdisv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tlcuabol.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cqfdfnyg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ufoznvkg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iuypsznl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sjqxrncu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3libatzbk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ogtjqzxm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cgqbxxlt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gdpxmgwu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ceicnope.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fhytselz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwlduhg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zyycerjk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zpxlqevr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3iydnxgcd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xowlmxfw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3crtcyldw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3glqqmfxz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpjswkjr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3iogmpgxb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ljmwurni.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3okjfxhxr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vypwfgdq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qjrhgjxm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3arotyqbf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nawgzwxj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgsfohv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3aowggksk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nikcveof.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sapuhrlp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3snsufcdf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lfuxttvi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwibdkw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aoivgamk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fjcuynji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tdrhbwvf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3newczgjv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ihfqotzz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ahecspat.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dzvvpqat.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zwscmsqm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tkwwtoee.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3lsfmraqt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dcaftzxi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rujzdzgu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wyzmtfvo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gxjdyhwh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3reeytdzi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tfrtwvot.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tadlqqxa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3moudpmuy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3buzipdej.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3czaacrle.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zlouyimq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hitoejgz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3suizqlau.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3saehnnbs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lptiugyv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3foozxgiu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3synuheva.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rxjdehkn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tdxmkeqr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mqhxodgc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bpaqsmmx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rhphcdcu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3exjmtfbb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mavgugxy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3awfhgrof.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xfxdjdei.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qwchcgzo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qzlzthcp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kakqhlwh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wifcbxgn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fkgivnaj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sgvaejpm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xkurxffk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dueusfqw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3alafidjx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kdnymdhz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jjosonxw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3atnodknh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxszgsdc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qbqcznog.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xeleypvy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nocthcvr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cssknxmt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nxorkvcg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oiklyfjw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwcfisud.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ejwljbsr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uccgjcpu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3radiduki.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3apsyullt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ccqhdxyy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kfbslgkv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jtdxwrks.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lgrszcoc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3aamknxhp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tqlvcvuw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvxlokgg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jvvifptx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zlrwsybr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pykojflt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzjfmxaw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3igzmsaie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yugxjeig.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3asxcxfrq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pkquvmcf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qpfbkzim.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vmogmwxi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qwxwdyfu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qdjivcyk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pcllbmxb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zdulvwch.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nmancbgm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dyrmasww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lbgclsaz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3oqcubecc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ktbkrrqb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xvtkumcw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3khsgngsv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ehgtnxeh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3axesysyq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qjrqrmmi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nwfckbee.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cgqbfzpd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fimnbnkv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tyfwdhpc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3snrbhait.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3murkhhck.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qkhwmuqt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bccnivkr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dytkskzb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pruxgqih.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lqfimdtq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecufigey.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mizfdrkw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xbhhsfil.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3chqcqosl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zitblgga.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ujzlwnzk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3osxwtfqn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hojntwvq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3izfpbnig.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qwqlkkhm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3clwnkpzz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qhoayodz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uxwkryvf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jeomfxmh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3upzoibgt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pixyvxlu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kszahoht.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsotmkwk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3exuahtry.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vntdnlhr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgqllimw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zafxhkuy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vghonxgt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kwvjjkwl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3farsiffj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xintxssk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zjtvyory.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vikhrfva.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ckhazdqt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3anbdyeke.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vkfxosme.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gnqndvqn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3botyrnjn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xogthubo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cjjeacbq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkicqhx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3yxykuayz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3euljzfyv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3arbthmie.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xzukepul.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlcmpgg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wgqwhnzm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vpswiadt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vmvjgqrv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3imaibijm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3llzknkyx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kgawesir.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yavfbvnj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rvtcaulp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydwyadmy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tserwckw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pkrgjccq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fhkcwwfb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wqhyahrh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wkpkefut.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nazbztmz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pomrxfer.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gwxljfoh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bbneldfj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fadntqgc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vhodrcuo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zxcfgglg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zrakfcsg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xadtbdvu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3esctgxly.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cvltivvl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nsmgcyoi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnonkcoq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3geonpnyw.html


<!-- 参考信息 -->