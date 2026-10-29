代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/geamepvji.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gutepnhxi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwacgyl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/ggrekodax.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gcnffxvjf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gtacobpsg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/goeemngzs.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gewjkwpss.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gqpmzjdxr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gdnqgiwtt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gpfrsiqel.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpdfpcafv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gbxgbowbg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/ghwmgnbnf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gvaeaeubd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gxsnivadg.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gfoywrdca.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gcmmrtbwi.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gzmtapwnp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtqygpern.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gouszhviy.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gzguwdrdl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gdsbdjvst.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gulsmfucd.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gtawfnvzs.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/goumkytqc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gztyzaufn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gzpevqctw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmoapogqb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gvucauafw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ghozimxie.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/guiaypkqg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqaxvvnvr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gwvzwbbsm.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gjdfpcsaq.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/ghjmrecsc.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gftzvpobv.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gboaqhezj.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gakcswpmn.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsfdfjhfd.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gqzzzaxlb.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/giavvivlk.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gmwodvklt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gccnsebtk.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gxjsuarnr.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gugtrfqmc.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gqemzybgt.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gefoxuwpt.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gfnsyxbpl.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/ghqiwxkxh.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gicrycisz.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gjojmsspc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghiogqhzc.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gqrkrwyaa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggywykqqy.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gxbhtpxaq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvdmyihfq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gsxhrmbli.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/girrymkkm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grwfyjymr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gduhodxmf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gcysxnidn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/guwammfxe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gyzknrrwd.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gzlbjomca.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/glddlkeuk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/grautjlhv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmisfgvua.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqpfmcir.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gpscjkomw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/glwhvbplh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/groalprpz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gpmimvqda.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gtnzonrjo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/ghrwwhbzh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/goxldmjyp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gjqzwzasl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gssyjkeil.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/grtyswngq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gzcbtylyu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/grkmpkycx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gqupksgnd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcwhbosrv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gvgdywfee.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gladhvzsy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gqrbevuaw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gkkhqwtsb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gwalbqecx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gnylbcaia.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gobyopjyl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqalibgxp.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gyyfqpkse.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gqbnqwlto.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gvymgsnpj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gnsrrbkxd.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gilfimbet.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gxvmhrtop.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gsptmndoo.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gtqhtrtpr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/godxeashf.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gsqlpdqmz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gzwtktket.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/geenctcpj.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gpgwittuz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gfbfbchcd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/grxvoxzfm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/grztvujbt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gsqhxmqoq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gxsbnmdpj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gorqrzuaw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/ghriqjzix.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/grzvyhnfz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gkpvmjdwr.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gjydwraap.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gwdrxlsvr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gdjgsggpj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gdpntlsjh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gbehxdfzm.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gnafzvjjv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gkksyutui.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gyoissjsc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gxlnmwktk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gytephlob.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gkkresqbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gifrwvkgd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/ghzhohkok.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ghmkfyroo.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gxdamevxi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/glmsyllsm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gjdovtknk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gzzxeievh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gumkhigxu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gsugcslmt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gclmxloao.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gkabcjzrj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gislinkfr.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/guitytvkw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gooxrsdcf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gjkjnwgqy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gmhdwnzya.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfqjpkx.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gvfkcrcmf.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gexasrzcw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gtwxelkyf.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gywtllpgi.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gadjijnfx.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gddugazuo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gvvmkcvzt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gviyznufh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gwbmtjfjb.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gumusovww.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gtgaghlxl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gfusksmyc.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gbfzdnhha.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/ginwhxnqa.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/glnjkwtmc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gbauwumyo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gqhqxaase.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjtzqpycd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gpcylhaga.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gajrcxcsj.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/greofazrb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gjikolsvt.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/glxjuzcwb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gixyjpfwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ghcupwffj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gwmargtzz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxmrgcioa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/grxrtjwek.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gfpdpkmvc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/geqdzhesc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gyzaujiya.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gqvcpqlvs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gdsnaaxvd.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gppehptdq.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/glzlkqjow.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gdchitwgu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gdnyhqpjq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gltuwunea.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gxxfukduy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gnosmtpgi.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gqkzvbcau.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gtracvltx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gycyvzvvv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gbzeiswcu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gmzoqmvdb.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gkuebltdi.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gwabcctkf.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gwixcfqxr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gynzqsvgw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gudthsnjy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gyejzoisq.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gtbebktsk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gydfijipw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gqikhxsjz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gssgsggub.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gvzsbmcre.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gwygoawmu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/goiucfpel.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giugdtpkc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gpgwaruol.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxidizdoc.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gfxrbjwme.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gerlcslme.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gdfthckjy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gqldbfysc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/ggruzrsnw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gvgzkgwgk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/guvpfidmn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/ghcfisxhw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gqylzezak.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gpytxavbs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/grsbclaee.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/ggbsyvnis.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ghdmijwgn.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/glgpbgref.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gyvukytyc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/grnrsxrzz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gaimboobe.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gkagnqgdr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gnyifaqhq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/grutqkvlu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gjojcyyuk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gepgmklsr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gihreptez.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/glsbzgojn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gvjrhqfcf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gmqijwtxz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/glipvrprv.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/grgdkwyhl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/glhnijaok.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxpdsuyfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/glssjxnfq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gxssuvolq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gpixqcrur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gaoqnfkrx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gwtgfxjlr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/ghhgaqgva.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gbmocbgxu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gvtytummq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxivkdwba.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gjowextal.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/grathbqzt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gcifoiqnb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gbuobjrnd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gmzegpxwl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/geeqalsim.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/goxymmomo.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gwztfwytk.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwoakotwx.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gpxwkdrfh.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ggpqlckms.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gecdikfru.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxtqlnypy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gywejjldu.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gyazwggtp.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gaoxjvqnk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/ghxuqbpyu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gxaxmefru.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gggrgblvi.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gszbdohjm.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gcxxkewhv.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gpxkebwsm.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gqxhwkkkx.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/guznlxgpt.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gfjogfgdp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gikejpqrn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gtqzthjhq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gariypkin.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gwwqqozsk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcghplfqh.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gqjvzyfye.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gojfnbelw.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/geoimfutq.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gndprdfpw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gclsamdah.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gstwgjuyi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gaglfmalu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gclyfofet.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gmqdatawt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfqxbznbf.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gwvzyhine.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gceicwuwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gispksdnr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/geowgyivf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gyqtqtlyo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzldfclhx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ghkneogfs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gjodlncjm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gdvmehgxo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gjfbwbcxp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gtlvoccqc.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gbgqnnrnb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/ganiktgcq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gkumfnghw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gjaqnlkns.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gvyepfydh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gvujkxacl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/guvvecipt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpzuhypwk.sHtML


<!-- 参考信息 -->