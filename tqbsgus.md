代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gtpcznptw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gcrfbxdli.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gmkhrlnnh.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gvhtghizf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gzrirbzfg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gzktgalnp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gwhwsiabz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gjrxaxpdc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gjplsqmmp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gpacxtalw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gysqpagko.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gzwoqplct.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/geeyiifea.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gidcosgnf.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gakvcujfy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gowpccnqp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gikskyfeg.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gcsgopufn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/ggfkxxvmo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gzsstidsh.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gnqlxohwf.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gneoeczeq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gdztqshwp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhfajazy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gfwiruoig.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gjeynzctv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gonyozxcu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gmmiwlxly.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gkewykttu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggsyziriy.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gwammxwvt.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gldmqroga.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/grklntckk.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glalymvop.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gooxhxqbv.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqqwiipqv.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxwrngmrd.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtuzlcoli.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gujjeiklx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gfkesnpon.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gmzwrpfpm.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gbagpijku.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gsmnfbknn.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gliofqdua.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/ggbggpojg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gqqbfmtxl.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gtasvltbj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyftvikv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gijwxwvoy.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gnzxdcdyd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkghutquc.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gwbzrktgq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gnvqrlplo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmtieyaxu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/govamzndp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gthopbzya.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gbpnnziks.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gksoezfld.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gfypwquiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glaqtvzrh.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gtecupbew.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gysifppim.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gesjcinsx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gadstpmyh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gxorywmax.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gfymdplok.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/grarnfnch.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gajuotiqp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gtuuqcuzb.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gquwcptfp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gpawouuii.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gquvpgdsm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gpgpdrpgs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gywlvkyhe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/glnabfsvl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmuvadsk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gkkkrqtai.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gpbkliolj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/guytzamoi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/grnssevyv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/ggrdefprk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/garcygqca.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gcptutxix.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gfbmexdfu.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gmpifmliv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gojocretb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gwibqkybl.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gmtuweaxp.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gywddctzy.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gxvfhmvgk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gxroqaqce.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gsvyaqkba.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/glsbevxrz.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvjhbcoln.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gqetlnisa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gxpxuzbae.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/grkcshalj.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/grwecefew.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/guzddchyf.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gfeudeghn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/glfjytrqb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gxwfmortn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gwokvcbhm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gtojimcta.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqpovvzko.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gxrweoerv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/ghxzqejox.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gepugxhsn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gcetryvqm.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gassfydcq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcuzfaupw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gwlmbdeak.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/ghrfvpmqb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gmakxytaq.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gtoowzkkm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gmoiuqclq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gsalgwlll.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gxjdvpoey.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gfqdacekw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gfclmflsr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gbntygcxi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/grqnsrwaj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfpphgmgr.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gcepxsfvl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gfmpqleka.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gzkypzzxg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gfqpnqelj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/glzdwbexf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ghkenoatm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gyflwlgzv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/getqxhitk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gwsuvwzgp.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gsmdutalk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/ghgvmlpgz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gjaobwbbz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gwncxmpyp.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gbzeqkqiz.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqopeqdhm.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gyaggniwm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/glzzndckc.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gctziiaym.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gocigsrfr.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gnajhztbj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gmrmfvcmt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gxdshwafj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gffrxxcws.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gqegjwtyi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gmpxoumbo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gbqtkbipc.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/grspgjoiq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/glpbhrpdf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/grmtsmlac.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gomekxfaj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gmobcijqg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gjffsvcnk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gzmhyazuy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gzqkoqhov.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gahxaeoqk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwzdwstnu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gsynlpppy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gmbtfalmm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grlogllxu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gqtspawqd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/goygoqzgw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gmwpsgznk.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gatmnusku.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gskwdpdhe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gxpaxeukp.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gcmtqpxeh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gbkzrwxbw.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gpkjmdvhy.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gtmmspbnt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/geqowaogr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gexlqdazu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gwacrsmlt.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gtjkypcke.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gwvqqughy.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gqufjqgfy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gjklwxxeh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gdqyezlfx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gdlwwocsf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gmgcptrmi.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gwmyyvvua.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gxuqjypre.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gvyyqstmg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gevvhxxlf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/ghafbdbrz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/ghqcstdbk.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gowwgxnps.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gpcopwezx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/grszwjisx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gvpcqukiq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gldhijfru.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gtxmghitw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gbwgfmkxe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guxhsqxhq.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/ghipynbru.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glgxkicky.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gtohfksqy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gnxcjtskd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gdvgpmqlt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ghtplvvye.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gjdaeriai.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gsbhclxkv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gjpdhdnip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/guqtrrbtx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gwmrnfcyd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gskrirfqf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gaftwjhms.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gzjxpketx.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gtokdzakd.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gihpslnwe.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/glmufbtml.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/giztuvniu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gvrydvzeg.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gxtrxuqek.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbepbpaia.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzbjdktog.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/ghxedekax.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gabpsssga.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtfzagsax.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gqwzqnrvb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gnijjcemo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gzlenczyb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/guqczutqa.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gcylsiouc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/glrocnvft.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gryuyhiks.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gbyjfkels.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/grbkdgedk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/ghmbybbxo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gztatithw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/grwyeuvra.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gzqdmomqj.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gtuofixhb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtbwuukhy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfsxynivx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gbnubidxq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gmqrrcthd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/glhlisbjm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gofurfkrs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gefpuirnt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxxfklrgs.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/geyyunspo.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gvdqiodzm.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gccrjwkxg.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gylwzgywz.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gffcvpnhw.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gtyykhubn.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbjzmtgro.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gpmlypita.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gvbvepagm.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gdaedczpo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gwrebjeyt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gaxezowhy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/giipyvgln.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/geexdtewr.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gpuekwhoy.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/govosgwft.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gicanlgai.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjobcpwsc.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gewrzigko.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gssxapwua.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gxsckgzfr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gtrixqicz.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gymsyakpw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grdwaydhy.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcwyaeqx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gpytdclzg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gsrrzenor.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gxlzsdfsu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gttufocyh.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gizgmamlf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/ghhubrbwe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gezikdqpx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gdkapvsao.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwiktykbd.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gwbmiaqtg.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gcuyphbwy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gerngnmwn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gllcqjgjn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gjelauhcd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gccbxayie.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/guksroxap.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/glorxyfht.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gutfmwiip.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gwfvrbsbe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gmxnztpgm.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gfnhmyntr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gsdbfraqn.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gviekqdjo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gqdcptudr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gaktcohek.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgtngcz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gafofpbzb.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/ggdrmxstd.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gneikbpha.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gwvxguqtf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/ghfdelxny.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gxbfyahms.sHtML


<!-- 参考信息 -->