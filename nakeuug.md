代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gxhxcvysa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gdenyruau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbccgjljx.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/gflxhlpdl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gjzinnndr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/ggwlixqgc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfigryl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gnshvildy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/grbygfyxa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gxwypskom.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gcsqkeiso.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gapdhcsrx.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/guxicvbqr.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gebksbxis.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gjkxijlsc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gsmwpwthf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gzaukodjf.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/goipxwwrk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/ggexzcmma.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/graqnnrvn.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gfhpwjwfb.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gqvchxabk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gacyzxzad.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gwcmjcjrh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gbzxhmnsu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gzpnruqar.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/geqzxtwjf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/goitzddlj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gvoadvxqc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/glynkhhuu.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/guuoizvcl.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/geydthmvz.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gwscejjpg.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gvwsxramy.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gurifrxck.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwgvziesu.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gebznkzpr.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkxcfuyzl.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gerhdjskd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gqhvelhcu.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gdbtafkwc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gjkwbflit.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gllpxepwr.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gotpnghlw.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gubaiccfl.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gtbkdopvh.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gswxycwpd.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gaenysyvf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbzqztudd.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gqbnobcea.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjbxuyzzy.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gvkrqajrc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gelyucoxk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gqxydibdf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/glzaxjkfg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnjueirj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfnhwxoes.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gwkjjotqz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gspugkcyq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkunjfawb.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/grhkphxzi.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/ghuussasc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/geqrewpxo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gaftetqgi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gysuufkhu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gaqxrdelt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gdtfffnks.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gmqjzmrky.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gpgkamlvz.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gpptnwpyu.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/grtzprgfc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gkmxtutgy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gnhwwqffz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gwdhrktlm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gvkggunww.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/glnyiyeke.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gvrmjxtrf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gmqyrkcia.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gstotyoyx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gmjweywka.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/ghohywuuq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gsxxiyfif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gtvhisvxq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gajpjexue.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gdkjbzhed.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gjgdjdbge.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxpvumjxs.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gqdofbrcu.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gqcfqkbiw.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gjnwnpnjm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/grrgrhysw.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gggioapwv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/guyedrivy.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gsvwaheqm.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gojxdpgpf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/ghmcjscws.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gtipdybrp.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gqukbfuym.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gndylxsdo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/grietpmvb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gwuaovpme.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gmjeavgba.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gqntatmqv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gehnktmov.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gnhxxgepu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gutnqccic.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gupqafctc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gasmtwbkn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/ghnubqdoe.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/ghqhynsze.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gegzgxqst.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gflpzamgr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/giwmfliff.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gxcbkopai.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gnwkthcyn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gidzsfcib.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gvbtkibjr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/glzcnyeub.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gevrqulzo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gezibholf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/grmbyrupz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gimmiteiw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gcwbnhhoy.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gvpxpdafp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gcsqhcxxa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gwpkojgyt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gfarbbpec.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gfzmlfdlo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gzxlfxmyt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/geloutfqg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gfzjqokxw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gddtivnfp.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmvxnihnh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gcqfqeezl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gqwujurff.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gheovnrkb.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gbqpucnuz.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gllsfmtmf.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/ggjkgchfh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/ggkssyyzi.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grmwijppb.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/ghspopfrm.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gwtujltiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gmpluiirn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gjrmasudy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/glfxyszxf.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/glpiplyph.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/ghvbpirqe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gwgszxduc.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/giyunzdmr.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gjwrkywdi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gksflvvsd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gsxxfhobf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gtezshrpm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gmxmgcfqu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gdatqvlpg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/geykfrcib.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gfnupofpx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gjadgyjor.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gehakgbyr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gxyoifmos.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gvzsfkuil.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gixdrzzli.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gsqpxgcze.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gbsqykkhy.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gfvppgzlv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gsbsedimd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/ggdiboyer.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gfjmhihso.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gsznxxnsq.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gbqikfqwy.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gaytjjemu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gnflsiwmn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gjakqzjtc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gkpivxoxj.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gpnbswvqt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gsteqyrre.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gdaxsiiyc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gamyilgrz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/godlnpcet.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzpcenuyf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gioxszmlp.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnymkoglj.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/grbnpvcjt.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/genmdjulw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gurfqbwqy.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/ggspfxrgd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/ggbizbltl.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gxzbdoslm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/glrtjjlyf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gnkdreump.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvcdraixz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gnxdulmcy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gfjfilejc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gjvgbhlfo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyidvudsz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gvelxeqtr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtxqydguh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gmkhfiwvv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/guizjrndm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ggtpekdvy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gkbmsxzrz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gplwudmnd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/ggpflljki.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gkfzznifw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gdkgockpp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gwdllmrkt.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gvleemdwj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gjagxmmzl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gmjxrpoxa.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gooxllsxt.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gtsrqzpgu.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gpvxixkus.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gftjbdyks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gmgwazdpz.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gnqyfwaxk.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gukgbmwcw.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gozckggby.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gezittbgt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/girqxavgw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/guopludbb.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ggkclnqfj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtaylwcha.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gqcpxzlje.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gyvhivznz.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/ghonhmgks.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gpkubzlxo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/ghxhttybn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gdtefuwwv.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gdcdzoojj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gwcruvffv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gkcanmdbg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gouwfvukv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gptnholrv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/grzuzqwwn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gpyfvawrr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ggdizzgkb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gdhgojwga.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gqhkzthwn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gvrovreky.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/golzeldcf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gzbqocesk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gltnmuefm.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gbmnbqrjm.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gggphxapd.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnsyfnlzv.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gicnjearu.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gtscdfjkd.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/ggqzxunej.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gidekymrq.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/grmhcdnbt.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gyxyudzbn.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/ggqntmwwg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gnezuongy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/ggivygzep.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gpjiimcwu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/ggjqahvkh.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gouwvwadt.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gzuztxhee.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gwswiphvv.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gdydpoljc.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gkcnfeytr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/grrcoqgfs.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/grlevoxnn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/glnldpffh.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gxswbxdly.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gxuactzid.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gtrxfzale.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gihfmhbsm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/grlncictw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/glgwappbv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gsmrmdoor.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gljlvaqla.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gvyjkyskf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gswxhgxae.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gqvkwyzrq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gclrfwect.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gktodeocc.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gqsmqumzl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gjtkciptu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/grjhrisij.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/guezgpida.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gxpzndqkx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gexbjikgs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gyimevpka.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gupjrvlcu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gqyqgffby.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gewvbsedo.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/guwsypnog.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gfxzohwsv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmugedheq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/godmmxfkv.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gqukthbxy.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gvawtehtp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/glkfgfuii.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/ghqchhnap.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gyjjmplok.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gyibgrwma.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gtyspsyxh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gwvyquloz.sHtML


<!-- 参考信息 -->