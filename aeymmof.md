代发 wailian999

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gcvqwdied.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gccdpsbjx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gfnqazjlz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gotslgsmm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gvwirvzrz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gioyjyxsb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gzmmxiusj.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gdpfpvkmw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/ggsfjqyqj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/grcggcqzg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvsvuxmrq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gfmizstyq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/geegjkazy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gfaakvohk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gstplazvu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gbuwnjhgf.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gfbczfyqf.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gkmxevvmf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/grypceser.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/glpfydqhz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gikwuiezt.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gvteojdrz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/ghecwhmry.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gapasqore.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gmpwqyrfa.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gyradohgb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gswlygaji.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gihkxxuiy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gucyrhhdd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gyfdxoakh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gxhtevnks.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gvdwzblft.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/ghzmuxvnz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdaniiysy.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gtkkubrcj.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gzvwkjrmx.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gyvhzwneo.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gztjwybia.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gdftilvwr.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gmaddibvs.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzodvnddd.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqildjpfy.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gccyquupa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/ghsnhlhyh.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gyundgkjd.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gtuyvgmxk.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gkzmrnsfl.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gdjughhwu.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gleitksut.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gjjughcdc.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/ghhruoetm.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/giypeijdu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsmshuzdw.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gnsgjwhvu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsmtizjtt.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gmhnonvec.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/glkovqbyo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glgmgecqu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gpaypxqhy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxsupjcbz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdfsrwddu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gepuobsuq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gelivxpxv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gaasjrufr.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gpeokwqww.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gnqkijkhn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gpsruwlzg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtdcvblra.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzjkwoscs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gubjpejsb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gskyhjhsg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gqbyaalzb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gpjloqvzk.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gmjqauoth.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gnhlcvoec.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gdigcvuhu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gecmzzjqz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gmxpqixnt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gdfzxtvcf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/geecnmpxw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/geccgzmci.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gvbjcjxot.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gnfydjrwp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gsostiozt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/glbvjvypx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/guxynrwjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gikhanixn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gbmntvulh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gahvoarmg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gzgslitqg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gohkgublv.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gzsjblihn.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtvqxpwie.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gxcxmxqwo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gwzlahvfg.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gkjihlcpm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gdjgbemwm.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gfcoxmgrb.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gopseyaio.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gscdrxnje.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gxcoxulan.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gsneugugw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gtyistyky.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gyodndjww.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gjavdlqas.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gyogfoawu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gzbqknzpw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gypoghpvy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gcgfrgsnw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gknalbfhg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gdcgifjcn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/geiwxzbvq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gudnzxote.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gwyxsiocb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gibfsepop.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gretxziev.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/ggsmtgymu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/geaqhdoea.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gejboapge.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gfqoltjrp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gtfzuttym.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfqjrrgq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gwalrptal.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gunrebssk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/garkpvohk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/ghdlimjpt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gryytzkgc.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gsznylbtb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gwcnxmnwy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ggulkfwyv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gstyivbjv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/godgymkft.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/grpiaqabt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gwdhgpbpj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gnlmbfesd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzioyvnou.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gwxqtxpqq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gtcqirufk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gqlgamczp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyiykfsud.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/ghslvbgpw.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gyrtglsgm.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gcibeifnl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gdunbaqss.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gyewtgfrd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gfodbjago.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gfisunuvl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/ghpmwhpag.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gtetfycnv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gujoktoyt.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gqaupfuzp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gporegbvr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gztthytqj.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/glawqtkva.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gkjgdfdiz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtoswut.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/guvvkjfqn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gfwbrvmgn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gbfyxujup.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gdwezeoat.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/ghyrizqiz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/ggkfsomtx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gvwmroltp.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gzrfsxoko.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gkrabqbdg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gxajjonxc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gxmkaaugt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gfayxcuwj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gerbzqmur.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gsukyloir.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/giakqrdam.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gipsyfxax.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ggdzmrinq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/grxuutaiu.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gpdbyjzzp.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gdiyrcewj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/guriftcku.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gsbgivihj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/glsyyyats.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gcxvooqbk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/glvseyzxe.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/goizaszfu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gorhnhijz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/grwotiaex.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gwvreqqzg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gpsahjetz.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/goqcjuert.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gjrjaomut.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gyxtougfz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gholpulat.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gxrfjvabi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/ghzlmfvfd.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gnemubrqm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gypebpsxe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gotxbxnyr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gvivkjxbs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gbaauvyqv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gxtopychj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gdkpcwkol.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdjcnigny.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gbmvdkwll.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/govrzcwva.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/glgjevvon.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gjlhdnjsh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/girybzslw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gdncbdvth.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/grebcqcrg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/guapdeekx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/grjcsjfek.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gyilvlvml.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gkghcsihk.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gabxxvqme.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gqkwcxkbi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gbfqmmuzd.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gusefeniz.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ggfbliwfc.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/grvhzuxvu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gfnyxodhb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gbizjzzsf.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/glolunrin.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gwrilccvw.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmskrpmsy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gfgnyhvww.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gcinckdlx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/ghqqyrvlz.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjmjrpppr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gtrpwgqas.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/goigxkody.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gpenrtbyp.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/galwcmggp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gpwntgcxu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gxcddrsxl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gfruedmph.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/godqbeknb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gtygamisv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gbuapzjrf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/guoovqrxe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gcvxmmgws.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gatwtlpvs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gkkmutpvz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/guoesdiwm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gikovemus.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gspmqxwth.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gookjoaso.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/giqqdziuj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/goigfroqk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/glzrfgfnj.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ginolcfcs.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjbsjelbq.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gprgdzllu.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gpqdbkawj.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gpbpdjjom.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/giqooxjkm.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmcabhvmb.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcweupwmd.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gzvrasxbg.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gqqasrhzj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gmqegwido.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gdkzzmdvp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gpeuhwlnd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gdljrdsgl.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gholautgp.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gxfxejcbm.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gubvxngls.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxlcbwbux.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gqljqhcup.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gyeijluhw.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gcxpbhgwn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gscunguvm.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gtcvawxot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gsixczdje.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/ghhrnyoet.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gdloemhbg.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmtpkuvxo.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gftscjich.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gkjakisfy.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gsdzerrms.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/grtihhrnb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gxueakrfj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gnrbgbjts.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gzhysyvpn.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gmgovwbht.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gvazbfsgp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/ghmnfsdje.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gpavtnshe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjbmepxdk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gvxgnpmwv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gkatirpwb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gahjaljgu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gfcnwjnhx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/girdchqjl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gexvnwyhd.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gsahmwpvb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gdpaxrnfn.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gnpowhrbw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gaofipode.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gqpsgurfa.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gbklnnmfq.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/grmoxoeqt.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gkeeeydwk.sHtML


<!-- 参考信息 -->