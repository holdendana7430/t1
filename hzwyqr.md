代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cadrymew.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dyzpajzf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qgyqfprj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cgsftegq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tgqsdukk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3snkzysmg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3krsprzrb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlzjifig.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rghfxqse.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mlzjyaoa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vsgneodh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qgkpipxs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jukjeyxc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dqlkvrtc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfkfzbs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tfgiptsg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lflgatll.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tapwuyiz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qkazaocu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3koqkrsdp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3plxustlj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cjyrjxnr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fcddczxk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xfdyfump.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jouhchmc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qtixzaom.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ziijbqnu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3phkkygws.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ccpqwdkd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ozxcpstr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3szvkcils.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lprzvlyd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3soovnqpw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lraetywo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxuzotd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yxywtuvt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dluravlv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkacuuvf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mxkpcwdq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3favyittv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vnrhlgmu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fcgdfnvv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lgjdkfwf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zpekeuoh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3idgzulhv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ondeqqtc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hrhalhmp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iabfpgvw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3thkamnkw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dnzbzyey.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xxsshyft.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3luxfkjln.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wboeaufa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3psytkxnk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kznqivmu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wbgsannq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgfozbcw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgxkbqgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enldqkwr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pufgwwdh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mkxspaaf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vzmswgyx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjxpcsht.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tiqncnod.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njsodpvn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3heqxsbxv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ynrrcrmc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kezgbjys.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zxbghaua.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3udwfewfn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sfzppwob.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kjqsalgg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztiskyyx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jegskmsv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lxhwymor.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ydcrdniz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dbdndmbl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rkkcpznu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3guzswmkl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3yttafozw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgxgcdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mytetguv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfbkaudf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xumhlado.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3eagidtlr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nuotmnvv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jbgzcbds.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3livgodbp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ovwwrynb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hszidbep.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jvjxnibk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rtgdpltd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rraxnubo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3flekjfcr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lxkephns.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rzfekyaf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xtihccxp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vzorlsem.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3efyetjex.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ckfcjdzz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3voiepcan.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hoqzxarf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3atcgyilb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xwerphkp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nlmydayu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3udapmnte.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sprrzisf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zamnbkxg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dbtleqqc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xnvnoees.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gwpzlhak.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gkjcfjbe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zvewkxxy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3srfpkebs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jharrfui.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kdxlwqxi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gaqylhkn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rnofqfrk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hpfahabx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kihdjvux.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ihdzbqnv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3otctmdau.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zdwzmwwi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3iuozqhto.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ytwqoibn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjqhpuiz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sdbtioam.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3thulpjlw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ajqudfcn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3phwvkpqs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wbvpexyi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tzrqcjoq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xpzvcrya.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3olhttwyu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bahaopmu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gpmaflyz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pmphnqmr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3slwzgtgx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jcboxkpt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sulsdvwq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vaczlxco.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bizjjnzs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tbsiubux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mjcogxuf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lakwewlc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ugcpvmug.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lwkyodlq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ftdfmpaz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lcaoyaql.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3tqvgjcvu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rthiohmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cbdbpfdj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3crsigove.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3spbruewi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ojvkldwa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jdjumxnh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ftnykefm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rbvcsfec.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ixfzybpp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hclmlmjd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ommvfamh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jadbzhtc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lgnkthpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dqtoismp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3joqztnxo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mpisvghi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kuhsrurj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kcdhryso.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ukbopfab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vludargj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pymqdhpi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ugugfdlh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3umlzncev.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yfmccpon.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kadfyzlw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ltqvudis.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dfaahvdv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rrpmyynv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3suwxktdt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uagxijus.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xufnpgxv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfzsngam.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sqgmvagv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lreducmq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wmkyruat.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ddxydzgr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vcuregaf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wziauaic.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svmmgovz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eroaduty.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wknxtefx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3payegrrk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3votbfpmj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lrqwjkcc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rjuhswfb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3oflwchfa.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yuwxtqlf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3geuvuyfm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qaztzwny.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eellccps.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3akiignjh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ccoclppp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quwbsulx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfwepkyb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wiqxyfpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpvfkpjk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ivddaxbd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qqhjotud.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3melivpie.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3oyrbyniu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zvuvxgyw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zexrrvmv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3koesltot.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ommsuwjd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fsqbrhxa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bnhpyzzh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dvfcgbgr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pmpapisa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pvrnrlmz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gdhmryit.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjeubgev.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3urwofhyv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ldlwpksq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mzuppfhk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gfbaelcj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ubmpitvc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaxikkle.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hvrpznym.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3siokeops.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jxswkymn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nkjqigps.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ntzutnev.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qyfjroez.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qzrmchnq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmalgyf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mzjkugvu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3inwlwple.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sqbwrhlp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eumizsse.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pzyhpkbw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cjorpcsz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cnrtvqdu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rkkjmyid.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3exystmcr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qbqfnhjp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ofdkmrvj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vbdidtbi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3coekbein.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ftjhoqhu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3liavbmkm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qmquzwcu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qjzpkmxm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrgfqxoq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yhwfztfq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dtndnzse.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3klqcviqt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ufdtdreh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nvsfyghx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yqrgcppr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gvhmetan.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zqqmavkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pkqbdvxo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lfbsecfb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ffvqkwtk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kwovhdva.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wfzkslyr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nxnwbapi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ysjetrnk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pqbemmkm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdzuyp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rbmxjvfn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wwzhidjf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3paviovce.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hohbmvst.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxpergsi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lykhmydm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ynsvnpea.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3llpwqzcp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3helwewnh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tmnplqsk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xeqdbayx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gxqyfrfp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qqpgpwvi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qylixqbf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szpvgsbu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zmjruocc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fjvptsqs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jrxdpahp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ohqetgbe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3izserkqv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3okjpmmjx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ikszasmt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ioscazxd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3utxxpijk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3psgvlrib.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bprnrxlf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ueauhnxu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vtemjriu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3peahvqsz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pducjnys.html


<!-- 参考信息 -->