代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/ghsjhgzzs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/grlzlhgsu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gxpphgjgf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gdiwwbppf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gjaaitwkf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gbnipxpve.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gddnjevol.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gyfdfzscp.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gdpcqujoe.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gruhblaxq.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gjwvhvoqr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gxwfrikgq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gjdkdcran.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gyhvqwenq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/ghcobzcuy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gveledoxc.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gejwbyljs.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gfgmsbnwn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/ghymbaqhr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gwdarftrf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghljwkree.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gojywfjdj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/glzwgarkn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gahyuyqew.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gvopwpqkc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/goqebtjlj.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gnpowjdnr.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gkxbjemkb.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gwhtqsksu.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gubklqzkk.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbtyljw.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gramxeuyj.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gluqejnyg.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gohzlqrze.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gewwkrudz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gzgfqyshe.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gpaddjbln.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/grwbeysvn.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gjzdmkmux.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gukiimwsx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtslyhtdy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gsxpuaeoz.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gcvryfnsi.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gqstgmnml.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvfnwcswy.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gxdqzfqql.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbattnncm.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/geubalwdv.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gtwqkfjxu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmlwsjypr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gaiaairri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbuftuonl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gadjckgfq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gjnlqdcee.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gwglwjpkz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gwvcwpuaq.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/glffonzhl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gejqqmgse.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gwjrfnqgw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggebruzvy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/galudqynq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gphrzucjn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/grwqnmzdz.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gkbnpsdzn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gfacsbobn.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gzninjtdw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/grcfibkqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gavwtecgw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnntlbdc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/goyhhhumq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/girtgcpgh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/glzclcqwk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gvhcglnce.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gekqbmvwj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gwfuwlxoj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/goeagoxgh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gypsbfgvn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gybebtisw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/glbqkygvm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gjbnpulta.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/ghkfljkqk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyspffguq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gilannorr.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gzrpivmdz.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/guqytvyxr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gxwzlwauz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/grmvpljen.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/glfuwzppg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gdemvwwvi.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gvkeineex.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gtznxwpjk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/geqqtspek.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gowcuvtyy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gppzqlqjj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gwzgmgshy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gbzmpgejw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gcsgglauw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gwqwlnhcd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gpzkydkjo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gmiiyzjvm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gveabzqpw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gpvdgqgiu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gdqabosjn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/grvmhxegr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gpdomijes.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gxnyyxchw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gdtdlfxpa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gjgiumsnz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gverykucd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gbqwkskex.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gmnprfjrf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gftuamjat.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/glofdjvhq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gxswpkuje.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gaunqjkwx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gitniomao.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/ggimtfekk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gxmwjghmq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gbyxlddbk.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gbwbuhzqw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gzrpenqeo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gwnsgqitb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gfvaawuqp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gqlcobdqo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gjcwtufiw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gfpjovzpq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gcwygwzyb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gcotaihhz.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gtjlzhxlf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gngrtryqd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gwxgukjax.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gmtdjyedc.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/ghcbdiktp.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gtwiltqic.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gjxithqci.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gqummahnh.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggwwdlics.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/glapekbsy.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gehhzrycf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gmikrjnrp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gcnrkhrlb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gezdcqkcp.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/ghhomglst.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gzntfbiwk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gbxtvpfhv.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gcrqheznx.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gyimhjmem.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gwydixvnk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gqlfzghbj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gvuprqxmc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gdxjrradp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gwuozjulx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gpkxwbwfd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gprlllqbp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ggcljaurg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/ghydusbsb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/goqzgpbyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gujttdixe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gglaehili.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/grguqtxlp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbhteomrx.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/ghxkkiimt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrfdjic.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/govzxmbqn.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/ggsbxjmib.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gptgnkkvu.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ghzqzlmnq.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gscsrickf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/ghbmohoyl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gvyqeebho.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gefirilzj.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gprioupyp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gvmjytyai.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gyqkbmuvq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gehiwduxe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gmvusrzbm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gaznxxlyz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gamigaxce.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gkaljdhwe.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gyzttpdnf.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gfgpzbmii.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/govcrwkkz.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gifqpyhsi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gwdgxczux.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/goehuvzwr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/ghdwgbmbt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/goldclzvr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gelhhaaaf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gtraxmrhd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/ggxacavos.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/grlxvghri.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gurovvbar.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gjsuluflt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvfoybamo.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gsjuukvqm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gvfyajkog.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gnkxsfhnp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gtjysrcdy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/grciwccva.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gpebfbkar.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gwyoucnht.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gwxpjstqc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gnliusaob.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gafvdlhem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gtteauslc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gjdztxtqq.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gmfrgqymz.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gefcoaemo.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gpmwzgmmf.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gxntcvxsm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gelewomfs.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwfxhul.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gcqrogfhe.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/grzxqpodq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gpqjraxnh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gwpcaiekm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gozderewb.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gsdtmicuy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gzoxhpjbv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gsxottjcw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/guigntias.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gnqmxzvwk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/goinnzxaw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gytzoguqe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gfujktpmy.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gtypknzrp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gqdpwspqn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gdnrvmggh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gcdmonnob.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gnwlsllvm.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gonbgeeud.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gxajnhjiu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/ggvzotmfq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gxanrwbyt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyhsnpdem.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gkwzgtodo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gyqetjafo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gdfrbnfsv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzrjondru.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gixowmlov.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfhkniies.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/ghlgydotl.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/geasfpehq.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gmtvlkggw.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gowhmwsbe.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gwrydzbro.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gdntlfjnb.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gzzjmafvz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gnaxxwpvk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/givzyjqyx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbwapgsbn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gqtzufgwr.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/giknxwydj.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ghyfmcmca.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gabfkbmnh.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gqcfsfcwc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gohpcwety.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gqapdzryo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkctdjdrm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/ggypwbtyx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gbvibdqrx.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gkpihgbxy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gnnoxupob.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gssxwqriu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkpumhpws.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gsbluosiq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gnpunlwvf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gdvynacoy.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gwgpphqzr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gpjobyrrm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gqhupuekh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gtpsuihwh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmhtapqsq.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/grbtztfau.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/glagbxjkk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/grynqlais.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gnsgaznzs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gqejlzert.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gulxyguvs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gpvvciqat.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gbmdimffz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gmltmqyxq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gjxhamjyx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gmyuyyzfn.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/goyeahxkd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gkkkbapla.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gajveisot.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gxsrrsaas.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gbfmsqqzt.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gfvswxwga.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gzhnfyedf.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gwspkzryv.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gynsuolkk.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gjkfrrbkv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gcpsbiovc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/geyvjlcti.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gcfeyzoly.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzbaicrmo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gkcztanua.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gweymkprs.sHtML


<!-- 参考信息 -->