代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/glfdvwrnh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gdmhqkwio.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gmqimvxws.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gcbhwbqdy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gamspolrz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gpcewtwnx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gbgnseiqn.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gohbittav.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gjtxatemg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/grnlpdpus.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gfnjotssd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gyytzntao.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gfimbbrld.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gztocxmda.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gbjqfgbuu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gvwyjzebu.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gaxcandhj.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/geweggdcu.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gafytmwdg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gjvrctjhp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gosfqaryh.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/ghlosaqxa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gxsufaigr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gnceqwiec.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gzpkpxvbb.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/guiitrnnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gxwmmpjmo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gkdswojfn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gpeethpom.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbxgfdqbo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gznipdqdg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gwytrqoku.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/grcrusmlk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ggwxdnsll.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/grvbvwexi.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gstvwqazw.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/glfgjqnma.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gmjmpielm.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxxhfqxpo.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gutqaicfz.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzzkpfsra.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gugaqtbna.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gznxsjbzg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gbicfqatg.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gqojtextz.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gloygmrsx.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gnsfedwsh.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gnhsutztp.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/grujgknbv.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gclbakagj.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gwbxvdqrn.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gwghpcepm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcpdmvyry.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gdwlkvdbd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvfxzxbgo.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gjqvdgsxb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gvhgixwtn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbarovmhv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtnilaxst.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/glbzhfugx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzctrgghi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gmduhlqyl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gnwukaghr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grvpnxzgj.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gtdxvowhk.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gjimadzrx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gytontalk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gkvxctsqw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gecswsxlq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gcsqoldpn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/ghpvrsjjx.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gmosxcsgo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gkfehuraf.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gkqcbtmwc.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gkumfgrgs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gpesbfqvl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gnxvcnxvi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gfezrrroo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/glasjlkhn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gdhmvpaak.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/grezkdqoj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gvigdtfml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gpyxxusos.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gfrffphic.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gpuaoqabb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gvfsorsyj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gbapgwjhx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gebrnwtni.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gyyjmhcwo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/giwkwfcyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gritqejos.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/ghnveyetx.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gxvbhatho.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gbhgaxots.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/goekbxhjc.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gxyulscaq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gievughcl.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gnicpfzwb.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gsibvplal.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gutilrdns.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gujyvinui.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/ghorflwdc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gugoymktp.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/giqsjvmai.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gppsayben.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggpgwwjni.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/giyvctiok.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gbtepeopi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gwsqacufl.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gbvmzaxct.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gwnmfmrwz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gkyileppb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gkltivnej.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gbnqkxhvt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gesibjftz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gibvzdrwy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmksskhn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gpezjxkut.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gzhwbatyd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/geqifxruj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/grfuamukp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkkecsdbl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/glvwfmmnn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gzuphipng.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gshrfzedu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gvddxdsdw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gxecuzilc.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gqqnblbjf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/grqhhirpg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gqsgsrgwk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/ggrswbwtn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/guhvamlnz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gpezrwnhw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gosknxbem.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gzxdicjqj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gennpburn.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gpdxzdkey.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gmwbfwjhm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gkcyxduvi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbxogmhsv.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gmmsbydyp.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/ggqkndgbs.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gparoysnx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/grcgwvefi.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gpoqzxvyt.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gbjayrbdu.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gzwsxvnza.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gokezqbjh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gnjbuwwlj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/glkzmepin.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gmleufvmr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/ggzkwdaql.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gnuqumxpp.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gnfknnrcg.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gjgdjhfij.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gpmmhbcff.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gegkvahxh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gtleznqjf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/glenjjwqa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/ghogmyrhe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gbfwbbjqa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gfuglzzto.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gobxmrugp.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gpdlinqad.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gudddxlen.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdseplgou.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gzydixmli.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gphxmgyox.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gulpetcqb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gmhrrecjz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gzwwzskgz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/grgmmjavy.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gatvgnbzb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/ghcbnlivj.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gwlewkazg.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gouwkkbrk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gqjiinysp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gtluecddn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gxefwjesi.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gptgowyor.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gyolfgecl.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gulweratk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gkbeiiequ.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gqoqfcpbt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/grixqftbr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gieqpltuz.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/guanaltmy.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gkuvonomh.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gecmpadxs.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/giainhrcm.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gfxgtcesa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/ggkftsbga.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gnuzqljpc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gfplorcxz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gvayenddk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gausewmnt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gppsdhxlw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/glteijsez.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/ggbtevevn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtfgqcxst.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gfdcipvkv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxealasbs.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/graqpdora.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gsfqhiiho.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gkqbonewt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/ggjeippwz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gcaeoslla.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/glystrlvr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvxkhgx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gnlncqstk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/ggvdhxfft.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gzvthgyhh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/glxrwbdcj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gdcsttwjv.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/glhzfypta.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/ghsiuyxch.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gmhdrfets.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gmgcqqesv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gafsphxse.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gmmrkwqnn.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gbuoqrpqj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/ghmutodql.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gbihbiyog.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gxeyvhfcj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gxzjumuus.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gzqfuajnx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gujnrnghf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gjpdfvdte.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsdjkgvog.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/grhykuhiz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwpbfgtmm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gfgpwvcqt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gjkrazzbk.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gqfvggqmo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gzqobriks.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gmuygfznz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gokwbwqfm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gesrtukac.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gaxqrbfio.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gajzzllax.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gjglakyho.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/glveoicac.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gjthgeelx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gwhthpgac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gaivuvzdb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gnhudogtl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/giqarcigf.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gvozynxvs.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ggzuxtxjz.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/ghpxkfwkj.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/guzgilwid.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gucxkxxsw.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gxwjdsgsx.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gyrxvejjk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gbrqtwwud.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gvuyyjygn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/ggtnrgldd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gagwpyobb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/groxpqdue.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gkjspfrdb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gckimumla.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gefqcaljh.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gcbishwbd.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gsiekrxpx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gsoxedlvl.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gxxqghdem.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gbbeylrux.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gkncsncfh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gidtodhpa.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gkdjaykby.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gksahrazq.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gtezdnitc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gueuveboi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/glzgamogc.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gslpusver.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gcskqjvyn.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gmrzymhie.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gywajlcou.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gyoaaxttq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gatnvehve.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyvmjafpo.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gayiqihbv.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/geyooghdv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gihvftnuq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gpenazxza.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gyfpttukk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gwzobyniv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gdnhwdojl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gwndgwvil.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/goetiunjw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gpwbyduum.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gkxvpsbxx.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gtorpdwbw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gzkvnyfzi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggesqdpbk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gfifhjcsv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gwjahyhjb.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gkrjxbini.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gdibojzmd.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gikxlwgbk.sHtML


<!-- 参考信息 -->