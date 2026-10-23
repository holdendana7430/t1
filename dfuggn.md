代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kxpnkmil.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lhafoixv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nfajxkmz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cplbubwc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mwnbjdix.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ckhxogsq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnjszflo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vlupnzdx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sdnwjkbi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tgpdjyxh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uwvqqgwn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wsguubje.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gmcnoyzq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yoxlqkrr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mnboiequ.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tmsyelxn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tablegzd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3delstcvq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vkgrgote.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mpxffqll.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dzibamyp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kkpqukxm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmligdwm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3izcnitwd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzssoeal.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qxiqoweh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3toxaczzg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3kwcgtxlh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3esflvwjh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ifzblird.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ycsmsmky.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ybybsdgw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtagbcex.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nqgjedds.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hqicpfen.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3sqixymxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lolgogdz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vvvionaz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xejalyrz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3woyihqaj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mcgybmal.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nnksixgl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dinuahou.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kramwebt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fuzeivyi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zqzblkri.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3saldyetf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3omqptnjp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vnmbxstw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fbdvkxkr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sfrzxjxu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ccdctlzs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wwjqpekl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vcgncfev.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tntuugcp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3eibwscwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrnefdeo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rpyehhzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlceanrw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcwutnwl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zmjdrhin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bnpqpugn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfptljf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsktborh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwzemzzm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cvoyynns.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3llmmlgpk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlsntkgb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ltskuagp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jaeeesls.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfdhmzro.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dnnrlwiu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzdtalge.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kjapmdpd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlgngbcl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3flypbgvb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qhmirkbf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3btqwidcp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mdovawgs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3whnafikz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqtinjmh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sokkcbgt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xrskaukh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3siyywveu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekrfesxr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hbgiapjz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3srfpdeur.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3oouxzycw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jicsoxep.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vmdvaowd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3skxvvgqv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rxcfqexh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gzwrfalq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bwipbwah.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uclqzojh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lcypuodq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wcvqojji.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ookrshpn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3codbkhfp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wzdgkicg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3voaeedeg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kniukuli.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3drrmprtq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gnhbtlno.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fraougnl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kuzprstt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3guvvdjfn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mqzrtlqe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kphrmoxi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3sncubqvq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hfycszpf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hbbzwjtq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kfannoxt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qwizzmuv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nfldtxsk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xjefoqht.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vutvikko.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mywrnwex.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhmxytlt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3cnrsocme.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bthidzpk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kdinebwu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qnqrqtjn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mfvasxem.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3riwrfwii.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcqglrbl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fymtyzxi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3avghuidq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zyciuktv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fquprbqu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebrggrqf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vkbogzwn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3spssjxug.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rpyxvisi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ddusyhey.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hnsrvvme.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3amewrjpz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tecrlfww.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cbabmgqq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddnrndwg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xzsoqjqo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3csjbbwyx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qqjudkee.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3oxwecwto.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3djseqdro.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qyokcmvs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3acurztkv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3eeqhhsdl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qahmnzmj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nspcmgbc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rqmwzolj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ztmikvkd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jumhxskc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3qzwedghr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ngwxoegj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fyfzdazb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3omefhocp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vflryhgz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yhcagugk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qdtunkcc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bzqgcpwe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3goflhdbu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ybqbmwvw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fznopquk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ububnxyc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uamjvikt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yxvtglpl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rmfkkfbr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cxuedzhr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bqumyabk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dqcyhzkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tusjseta.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iquelbwc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vuuxhkdg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mwenvach.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mjwytdzg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vsivgsoj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dmhkcmdy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dyjpgglg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rghlsaqe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3oihgxand.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fxqstvky.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vugdlrmi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sinakygc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vjxpdlgf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3flkaexwb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yeroqbyt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3imcitoyi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tzcaxebr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqofrqvj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rbqgdzkq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bijndgmp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3krqylvut.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zashjrlm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qjfokmnc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yzbwsnfa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mwozffof.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sikioada.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3umhgmoyb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwmbsgti.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ranbuvwf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3awdkfbjf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hmuistev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvznlbmk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3erzjzyxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vehcgflm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xvimaadc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hlsgjvxf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vvuwpeln.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wowkkhjc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sfonfjju.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cmnrmbku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ahpkpnro.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ahqvpdhn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sjtzhxvh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ngmyyduh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3yrssnyuo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wblmycgq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xruxbttz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhxlzeuu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3liopvlli.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gmmngrpv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3betlulxf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3unllqrxq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3elgbompe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aracvxlv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tajcdstd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3otqapxzi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3neyupecu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ydenecmb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mnlceuvy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zhgtdsam.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ppkxmyep.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qipwfirx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xajtylxl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mogzkyyu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xbukdnfn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3idhxadhm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kytwwjim.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3aqczpmex.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ysswjedm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdjwvhxe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dgjniquz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ytcnmalt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dizideuy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tzitkfcr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uhkfaowi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3znfagxml.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wmrqrnkh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ekenhjil.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ugvsbshp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uyaboapz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddhgkpys.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yqwnbqet.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uwihrrzl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zghmtkra.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3peounfae.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cblnpkse.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ivtlfrki.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vjmjhlfu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3phhnhyft.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lslubzei.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dsndmxzr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zognvigl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jqvkoejb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nbfmslrv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yasqweah.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ezovdhlr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eawhcdog.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3smjzkbkc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dexbgfmw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qsbczked.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3zphciehg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bkldynvl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3asfgchwf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3szfuwvov.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vhidurfc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcnwbyvl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nafusjji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jkrdehqj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xryruxxg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3maaktzgx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jqtuthaz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mnekfwzr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3llbycppz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bvslbdah.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3snarwdix.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hhbsskzk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppptxxxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lpzzxzec.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjwpfcz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aiisrlba.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dpfcztoo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uljavklk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jgypagph.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3txqremgx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bmjgposz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hlhhrhrs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qkgtcaap.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qgegkjsg.html


<!-- 参考信息 -->