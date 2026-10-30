代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gcemrxbcu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gcnqsxomi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gluddwaej.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gkcilgvde.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqqhzdihh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmnliktvo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gzehvobhi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gzphjtzut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gkksglyoo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gkasfytqd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/glznjfygh.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gvyelpurq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gfmfswtsm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gcjjnbzxi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gzfjicmqo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/giszwogzh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvhbyvwre.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gljzrrkvw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gfluuddrg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gdvyedtik.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gkeydlujn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gsyeennmx.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/givywgnup.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnbrblzbp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gclqmvxxz.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gkfedwujt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/giujptshv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gqtdymtom.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxsjrpj.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gacyqgali.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gunvldxxa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gmecynzjs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gipckbzhd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gnjcjlitb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gfryjfszu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/ggnphkrzy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gfyvnohyo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gdpsyoowc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gtwcbewrn.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gdchqikwz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gvsfxqhzu.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqmouupjb.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grfczmvuq.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/glcdrzbfw.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/giaedghic.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjungcb.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqzsbvfel.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gtlqrixdz.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gldsfdmfc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gukljoumn.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gwjpyctoi.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gwworgxrt.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gbykgbwwv.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gqooycnml.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gyuwrsnqm.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gbjgblduz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcbkouqzx.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gjhauebnu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcjnymzoj.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gblcvwvhq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gnndfvfjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gmfaiuvtb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/giloxhcul.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gttbzkcmn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gmxtqayml.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gmnkzmaiu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gcqxkmswa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/galnsdwkh.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gjspeflhi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gpqnttalr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gdojuqial.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gmbdrqici.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvxwfpmon.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gblamyoyk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gjbqceplk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/guoxfisly.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gyecdgpux.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gjfzfactm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/grmwkehyy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gylxduand.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ggvdcpqwz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/ghrvqdxos.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gdolbzsfr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gkymsdfnv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gcsklkckv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gzqtvhvvx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gojrvzoef.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gncxzucue.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gnwhvqirw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gabbivrdc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gqjaehqgs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gritalqwn.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/glqdfzqtc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gtdehjzzo.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gbkolueim.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gpeeifyur.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gklfhnkst.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gdlubiggc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gqxpxnhnm.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/ginpnaxpb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gxvppnimc.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gwpknlqlu.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gdhfhvtra.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gjrassuxm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gbxexiblw.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/guzvopkhb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gxxqbwvmg.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gcdcgauxa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/glizvjrzh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gtldlpcqh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gfspryatr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gelydfsva.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gfhnnavkz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/goydjspni.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gzxpnfyle.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gzlcuddav.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gxaevjvdx.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gibvfdajd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grymzkahz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/guchcpnxo.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/glphowadq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gicspmmhu.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/ghkrapocz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gsweyuznh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gsvfkzqhh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gooktifsa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gzvzztxyn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gzwoyiarx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gmrlhfqdf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gghnfqtwg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gbfxqimth.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gcdrhrlam.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gfbugnnfc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gstkmhjxi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gjhrqunsi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gcwkrtyqf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/grluktpdl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/goanpdonx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gokwqmgyq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gijhnccll.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gxlnftidu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gzjyykhob.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gksqemrcp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/grunmidzu.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gqmkavobu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/goilielmb.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gzohjtupz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gjvsbiuge.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/ggsrtwcda.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/ghmhbpmkt.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gsmogggoa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gdpwczbnc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/ggtcpgyqz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gimlprozd.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gqguigice.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gxogljceg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/giuppacwj.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/ghclyfezs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gphaqspmd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gpgayvpbd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gwtwgewlq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gfwqzanqm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gctwfmqnp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gvahwvqdx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gvrvskfzw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gfmfjetug.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gqrqbaqqs.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gqnaufuon.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gqlitfpuj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gbdlzktzg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/giskztdoi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvobsmeic.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmtcyjds.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gwiwlhbld.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/grgigxliw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gnnaljofn.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gpvklrbxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gyytqaczs.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gtvrvpnif.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gbbmonyqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gmjkacxxh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gkqwatsfv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gjbzohobe.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gqurazdqi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gutqgqlvl.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gjksrmhgy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gusqnkhts.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gdfsoyonj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdsrqroda.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gtcuctswb.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gliifyoyu.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/geguanggu.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/goqqdtbnd.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/glstybjfe.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gxcnjfkds.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gccqtqvuf.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/glazuyxoi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/geshlrrel.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gemgpnjvg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gslwhhlng.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gseejzplv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gvstqcbmv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghztxpqcd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guolycjqb.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gljswrvjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbzjcqwey.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gfnwizqmw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gfbcvkdhz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gyemvqjzf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gcvbtrtvu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/ggkxfljwd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gaylgdzmd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/geogdafto.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gxesqcwqu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gjxesvxkr.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gkrxvjbss.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gwhmuiual.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gusiuajvq.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gysmwgpwu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/grjenrgvl.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gowjgicpf.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gjkgkertb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/glrfpxiyi.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gxzbklykt.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gtjwwofrp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/glwgxrxsg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gkixtirgs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gqsiyygtb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gewtnnjam.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/ggewkfcus.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gdugyblag.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gtbdslkqr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gnqkcrbpj.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gqegndyhc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gejbjywjm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/goxzcqpfa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gmunyrivv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gbqzgtszq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gcgvotoji.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gyzusirks.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gurxguxsn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/galyzyhtn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gjlssyrsk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gulcirvke.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gknjrsupm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gpmffrojq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gcnroitvp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gkaiohmwj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbrvingld.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/glsdasdbn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gpaohliht.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/garrcxrbx.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfklgegvk.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/grzfmsuls.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gdoamruui.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gawlzhhub.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gseiqsrnj.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/goyqjebvt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/garrsnkds.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gwfkkvfnf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/ggnierfbi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gvdogiwfb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/ghwlaslqb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/guwkjfhej.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ggommextc.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/grznswjtz.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gwrhchkpi.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gjhabpssw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gcvhupfzd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gobqnftle.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/ggozsswyl.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gysxetcqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/ggzxszeky.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gwhbkftfj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/guspxsfij.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gwimsrxbw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gxjgayzsa.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gsndkjwrp.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gmnxqovyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gtnoepqnw.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gydhawqyh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/giviigxtt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gutkfuvuh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gzslhkzsv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnahafcjw.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/govxomqhp.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gnxncrsok.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gueplhimr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gghuiimaq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/ghwacwxjf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gssyvhtie.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/galgrhyyq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/grfolfpod.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gcchuikxb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gvqrxhfbb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gwhswmkol.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gdgnwzcvi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gwauayrnc.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gwfetttyx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gsmmcytoa.sHtML


<!-- 参考信息 -->