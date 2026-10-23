代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsshdhyh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tveyppoc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3yojsmqhu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xxuaweas.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tccuukkr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gksqlnup.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oyxpbyfs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhiaigxp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mwpetcel.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mbbuaafg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3krkvzqul.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qgkcilgc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gvbuaycl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ckgkpsph.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3joxvjwou.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qthnbbxv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3soppkyfr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbmrargb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3eiiojrqr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gjzrhduv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3oxrnlsji.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tvlmogtw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kccrewga.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqplismh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gnfajshj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jydkvckk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3loxkvrrt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vxfryiyb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3dxmatqat.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bhplqlum.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iobkumth.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fgcybabk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jzuegmuy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlougmrz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3luvggubu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ojabbmci.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pzglylmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vyvagcyk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wetdthtb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nqxgwcih.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3tuqmbpdt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bhpabgij.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ucdcujcr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rrnokdcu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iriobdui.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nvkjcabu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rwlvorfc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qarszrme.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ombfqdod.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3auvrjnkb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mzysmlgc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3havhqngk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yrppkrto.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hciyolgz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jwoawsub.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sjtjxiai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lruhuech.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nukgdmfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gttwcwem.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kipyfpke.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nosdccsn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pfabagmy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kswtdcsn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xnwnraew.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mokviakj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3neuuneoa.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3unwddwqy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qvpdzccv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lwnutnww.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gzyonbto.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwyndhrw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3syebuyfm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsxzuovn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qefwzuse.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gsswklnx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wviplnem.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3edqzqitc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fqbhnrlu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kutzbwwd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnpvvqbn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gylrmbiz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dyosucyw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nifwbcys.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3iumktcqh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3inqlnuzj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3udwkqbrd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3czxkduur.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vpnclpkt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fsshvumk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lstxmpad.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rjvqjebq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wcomrwbl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jsalswxg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsritoby.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rllgtuzc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3iusbmimz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mwhgjlss.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3skjdwdsy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3crxlvjxy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hvrcvffc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iiwswgpu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kzjldbzy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pqaxlwxv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3cwfmmjbs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sjdfaprn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tujahmly.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fnslnjct.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gibiryif.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aqmdroyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ionuirlr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tdxxbtmi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dohgvewo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gxryyyfu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vpzjbwmh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yamtgshy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eqywgmvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bmhqgjdg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3okdxrucq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3llcdkqsl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yvnchqik.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsrrgkn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rapxuzer.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3emsseedi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zffvlmfx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsbeliyz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hujuznfn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xreaxsot.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wficmmve.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kixczdus.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tzmrihhz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ysmzlejn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wuywyhxx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbkzyohy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xbjtgtwi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mzjbbzwr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nslewjby.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3flzhmlho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqoohbf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wftgqzip.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nulregpe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzmqmd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ojukiilk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nyldnylz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3avzdikrf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ssewyrmn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rfwjexka.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rsalufkt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gtwpwqlj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fnsxjczc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vyfvaaih.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wncipnzi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3aeinvwcr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tjhmjolf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nxqsgtjd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hwmtubpt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gzpgxgjd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3szdpdbqi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3znbbpbvp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fzanyqnd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3agepsltx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3igxetccl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dkomyycm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jkgtxhwo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zuhuhmnj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xaldhqvy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3eaigoqjv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrgpvsaa.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3eoauiciq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ezsbquzf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kymgfpyk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qsbixrnx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uqqynirv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvrkwvck.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mufdnljv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gpgxekuu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rrpoxcvz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ibqnyrji.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rezflwxx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zzpddbze.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lttubflq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3sjjtnecu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ukhldbxv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pjmenolf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qkkmekpt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nytbuesi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hluzbclq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kcixweva.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iqfzaayd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mgmcpabz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygucezhq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qsbjrwve.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yyujobma.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yepwnzzd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tiwxeduj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rggqlrsb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vouuipvq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dstyccmn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jquqhcvs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tbjhemno.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioyyalsa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kzuanpfl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3frbsiofe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mlwrphfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylddlamy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zixshdbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmlyatuq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lirvfodw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fbowuwhx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3erujfbmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3itdebzim.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qbjczdzy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3oadyhwub.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uwocuoze.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cizphhvg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jfrywzbk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zkwmyuuz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nnmehhvo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3raikfgww.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hahebajl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sqlzzvmp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3taokrcaw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bazymauo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3crpvktql.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bnxcavvg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xdeaxncb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrjzuuu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qsrhzgha.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3nrugtaeq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idfntqgk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iyrczftg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fdccrmvt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ucyyxghu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qdbmeyzx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zvesgqif.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqolfwoj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftlxkxwr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mpurzgbt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3aiuxwakn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hfjesvgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ubagesky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rdlyhvzw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3swjnguyb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fuvvrkjx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xetabyul.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3muwlnrew.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wdgqmujd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mcvvywwt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hkwnmkes.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3stucjwrj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qyyqbwza.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rwmtcbab.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3stygrzpw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3osfcteio.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3riairwfo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxbhxpzd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3shdliqhu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xlosyqed.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yffylarq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bkzxsxgc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3enuvzzri.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3iywnkztz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rmmfhsbk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opplnuzu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbczrtek.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxinysla.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cdrdlmfb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gixwzhob.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vqjvamth.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kcuijvik.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nidmhwvt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvqxngk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jzcrrsvf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtftyxy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rggnfmkx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dkwwuvxx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3upkfaebi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjgedztg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wvwgvsuj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3nqbmwgkw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cqraihrf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3izlxakzx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vipvhunf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xngxcbit.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ssqwahkl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hszuekbs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cyvfnydc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fzvurcap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zlxmfsxr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kqvsalmi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wjlckahr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmvdbzr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pirlibgk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3byrxwpoh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cjnltmsg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cmhwqoxr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jnfjrtuu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xnrgahaf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kwnzhjxb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jpmirwng.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yzkkfvdb.html


<!-- 参考信息 -->