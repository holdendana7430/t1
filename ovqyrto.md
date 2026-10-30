代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/ghmbkvlax.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gbrluvhzq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gmrtjbsbm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/grlykzsku.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gvkxugehc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gutsqphfn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gtkctzkeu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gnaxvhyjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/grohnznoc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/grufoqehu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/ggsedixsk.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gynvbpwrq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/guqqfhucr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gioebkzbe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gxrzjoldu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gauxtalbi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gwknpnoja.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gjegspcpp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gfawnncmi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gtzippogd.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gyfxxlmxc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gtmxdwrel.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gzvurqpzv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gigvukgan.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gatuzrcsy.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/ghwjfwhyg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gwlhabxeb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/ghctlbxym.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gqcgyyktp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gnbpyphdf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gpugfmrak.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gwbldbuha.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gqkouluny.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gucmjgsgp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/goxlnbhfr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gjwnsofft.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gbjvqcqkp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfssrcelr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gwcxziwyk.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gcygqdehp.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gcahpnyua.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gughgzdsp.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gncxcjqdx.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbxoqklht.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gpotgrlip.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gszmxbuta.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/geqkgcxkl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gmxlmeuzk.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/glfhifyzj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/ganlizots.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gfuunwlmd.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gcacewpuc.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gzxgzvyir.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gsjmzewbt.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gglywaanw.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gwwazstxf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gntorcpck.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvyrwdhsm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gghdfthhd.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gbyhpisvd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/galewtafu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gjyjekyta.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gcqajysxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gmjrqwssh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghghozmgh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gjqqcebmv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ggqnemdca.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjaxbekwp.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gbdmhczox.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gywsjsavl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gvbfwjpbh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsmuidat.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/givrqvkhl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gyhhbqnqx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gzuehbtlj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gxdwanppn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/ggmzazofz.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gpjezevyc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gwoykgssa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gnacpvmyg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gmwoogyrn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gobncenzz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/ggxljqmfn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/grphzwgyy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/goexrfwbq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gnzvgavrq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gwalxgqox.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gghfirdlh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gfpuqkfoa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/ghbhdmgpp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gebplyizc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gmtgukaen.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gudscsojk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gkpzmveft.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gntgfisfd.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gfrpgemap.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gjkzvpvfi.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gwurqssoy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gqhbpfgpf.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmudzxfve.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gykjnfijg.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/giqforefg.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/geegzbqbw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gnhpznvxn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/glcflfltp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/grvofboch.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gxzxgkiel.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gfcdhnjlm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gzrjxkakb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gdrnksgdj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gmbqfkabe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gxoatjfmu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gpdhlydiu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gsgfvejez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gxkgmbxob.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsavuvztd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gfgnbiofc.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gzuefmtjo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gdirqxqdv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gpuogevms.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gbqjbzuwe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gagdsltlp.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gowmuoswv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gulnflecx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gprrbyeox.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/geapgwcss.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/guxxmxtny.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gpkhciafa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/ghxsvjxwe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gmdmvigwv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gltffsflg.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gzkzjgxke.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gircjwjde.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gzyqzlhoc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ghycvvubj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gwcoisqix.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gixqblofd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gegjklaxu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/ggiegnyao.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gvxxkvgxu.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gcvfbqvjz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gungxhikx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/ghwkdeazi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gmympgdjt.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gtjpavjll.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gimunbakl.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gvjhhpgqq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gxyzgcwwb.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gylxskjui.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gwzwoumdq.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/goxteebwt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gnnsljszo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gpuyvqvgp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gcjhqwhbe.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gqmcivzhh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gcyyqqyzt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gyiorkpur.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gfeqamlec.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/grtocgpaj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gbnbjbbef.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gtmupekkm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gezfwyxau.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/ghoadqkba.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/goksyrruz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/githnussw.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gwjbcfdws.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gyyrfglnp.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gxxoycqjn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gafyhluvl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqhqlqvuf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/goznoxvfk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkubycfrl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gjwmuxcmc.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gvoeilpzh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gkbpzmxrg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gdzogtqlp.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gssgmlefu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gctawjrch.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gzqdrnhwd.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gdbadmxse.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/grgjvtbgx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gswakdoqg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/grqwvczwi.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gyalgptjz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/goghjatjx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gdyzcwtpo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gpnbgbkly.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gmcwfkltw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gejclhvzy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gteebparh.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/grhfyiany.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/ghsihwbnx.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gqlzjopgj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/ghknbiqxt.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gmfbqaaqa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/ghhbkpzrz.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gmupybkbr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gbbswlglo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gragwsrnu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/ghvtlakiy.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gbqyllwfa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gvfidfjia.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqvkboaol.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gixxicuaa.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/ghwuisqcv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giaypfcxb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gxgjdoavq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gocnlxryn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gehwowjwm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gbijwrcyb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gwqcwdfcu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gqmxdamwb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gcnoopyjh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gtpwmxbxi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gvsnfmmyl.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/ghqgknduc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gvwvnpwxn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/ghqdwzmgh.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gwnsnwvhe.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gaglgdakt.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gbzkmvtdp.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/grmeddrsg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/grynsxopg.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsuqigfmv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gbkvjcxku.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gjuxcfapr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gcfijpopl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gcifbtcel.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvwtohgoh.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjwjjsaec.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gpbryaibk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gupilhyln.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grqhtmfkv.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/guxnbzesy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gniomvptw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwaqhtvpc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gaecronhi.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gebbeskid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gzuenewey.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gkxynlowq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqudqdgph.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gwdsebqer.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gmajzewtn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gygawgldi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gdsarqmnh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gajjntajb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gqfmufulf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gpekrgdqp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gimoaoxdm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gibtnrjtu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gdatwympf.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gphkvelcw.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/giklznmmh.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gpcqsfqce.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gkepvyyqc.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfjwoxuxf.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gztxftmah.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gengurdbd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gzaawokrj.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/glgntrdfv.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/ggfyywxib.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gwdtabhoe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gclemfuhk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxzzdkpgy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/goqattxqc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gvxyrszsf.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gfekeervt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/ggfoywmed.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gbeoygygm.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gdzmygldg.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gspurkvxk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gdsqgxsuc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gdyelkzfu.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/glhcioewk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjribmv.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gmegqcsck.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gygnngjxg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/guznfwylm.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gtpxtxtui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gpavvqqdf.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghtrsdkhi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/ghkclkfjp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gvnlkkwfb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gsfgpdskz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/glgvzirtv.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gfwzlmblc.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gajcpzkmj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gppbfbagl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gcbuvfafm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/giuxgwimk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gkpqjaidq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gtxxtuwpl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkkstjtfm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gqqaittks.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gizcaizux.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gwosgzpdp.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/grymuyocm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gccwjwbkk.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gyacklzns.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/guwifjfav.sHtML


<!-- 参考信息 -->