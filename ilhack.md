代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qvknuvgc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gaubvpnb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2heepgadg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ukdqzsdx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2yzlpquyl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cwzfnrsi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2epjcwqop.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cnknarig.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2anfoutsd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2fkxxmnxw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgqdfb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xflkgvtb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wcvneuqd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2juzhvtek.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ypflejli.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2envokdzs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgtirfc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2oqktusqo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jsjgsaef.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cocljkxu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vakjfqnn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2whraauvd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwdbbebu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hagolwie.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agvwjaxt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fsgoymoj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ojuvhnih.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2btbndsgt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2avcuoarn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vaxbfyuv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zdxfveuk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkzuunh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zrxoghhg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oflngsbd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqgmtzdh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mxtrxvtt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdebdfep.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2araamntv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2emfeaqxa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bjynlspp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lqsemeot.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ugnkcneo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kwrrbgob.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2citggcym.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bgtqlghl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2naddrvyl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dsuddqcg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ufwlubeb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ukcmgixt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxplpuci.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2caqumznp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vwjesyzf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dwoksiwj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2askzipos.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bmhltqhl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fgzhtqdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osefbhed.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ebstzcgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lznufkrt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zucqipsp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yizszlpl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zdktksyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqlstto.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlfqtnji.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jmvnogov.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jadftyvx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikkaxzje.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nlbxfdrg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nfrvdgpe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lpixjwdv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmjkdier.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqkqmjvp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2baeiglcg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vthnuaae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqpfkvkq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2thajbbfc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pgbdkjyx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uibdabaf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ooyysefi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgbwzfkp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nbxwuduu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwzdord.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ggfmjnxr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2apihrwmq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fytqzazr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zxalsspq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wdwvamds.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vxwdblbn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sylkaszu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wxtadcsy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qpciblff.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hltbexnv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzxzyzas.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vlccbnsf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2avmfpgrn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fskqlloh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ymnkmftx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2miqzvtgj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ezpwhhiz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lbbvbtna.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2skjdywtk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kxdoehwo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qcfahkvc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dhjjgcsu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ahuetmrt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vatcbmiq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qgulclpi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqmlxbb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ekcjyuzs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2smqdosru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2renogpaq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jqsjrpxt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qooismhx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qdpncwxk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ocifhklh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lyqahftx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qzowpyii.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ipdkbfiz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdeogyui.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dsndapne.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhgbobv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2iyioayzc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2noweyspy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2verlffpe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ragrqdpi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2veiiqkde.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkikclvl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2abwjxmbi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pbzwgczx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fsnxhujs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fgtakuck.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2asiyzkqf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2japmjcbl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hynhybhg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2iuzvtpfj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2itnxtpvl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzqgtjzg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uebomqyj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zmzjhikp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbaxwuox.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vtbqrlit.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ohexjdyn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ihnlulpe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xxfowpkm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vdkmmdgg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2llizsyll.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bdbxagpq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ukorlyvc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yyhwugcp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tsplxvoo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vexjbjkp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gbbqxdvu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2emwglhwq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ntbfirsm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vhyxifcf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xgelzihx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zyxwnswg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kwcxntcs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2idvmfusc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rmicqzwb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qrjbgyjv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ftmgxnse.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uugwvgnj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pqeuuppy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wllyzaew.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hdvudwnj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdgvjrgq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mgzcmvur.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vlddttci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dneqthyo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tugdwdbb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlgqqijt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yynaworb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uaqcnlrt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kfsconch.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2doanxvey.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuyezyag.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ftferwuz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lbjrueqh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fwedenvq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2odvadntd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnpvjwmh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2estjdyyj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fcolebwt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qhzqpksn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sbhxpbio.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2liefqzyg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yhwdqqaz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkyfuizx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puxoxkzs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ancbinoo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gkxeogrg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2eamzasqd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tddqktaa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nkrjfvww.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nnkcqebp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ewqssouh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qcdxuohl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2aqggarax.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbbfjalq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qzjemgut.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcmkvidz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ctunoiub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiiaoesb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wgghepam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkccukim.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vpuiouou.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rkkrsbbx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mddrbdvx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yjelvrnm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jqngnugh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wtsvyzsl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zsenvfyr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yfynblbn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gohzweqh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mukoogxp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xojjtdts.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sgvjztgl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2awcsmbwu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eekyofmi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2enomxpel.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ulqfnlsh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2trbahzkl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bzeloppj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xwswnweb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xxxgmekq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rwuvasyt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ntxaatvi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ljfkeqqt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zoeaewze.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hkzthllf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bqhpvspb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kpopsaos.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mdzihyam.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vbulioop.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbiwgitq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dktuinfg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pcflqufr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hixbjlym.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xpwvbcoh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oyejqtqw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2onjphbij.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vykoqbvz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rwwmprem.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pxyrklrv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jpmiktqf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ttzqebwn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qzwhaddj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aporqqpi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wkstaeha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nymbxhkf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xzlsuner.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2inckojjt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nsjppove.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wtrbkqxw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hzwavvaq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ncyemcmh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwbtqjsu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2stgfteki.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dxgthmah.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2tdkofknr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rmsrokfl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ajtstxkb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2svnahqzz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jqyxylye.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gzofhvfw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qtdveedo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xydcewbn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ddrudatz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fgyxuhuc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwwblwre.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mccpkcbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nztmondw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xftortkm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mtshzhyg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wchrlvxd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2njnxeizu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eimevvuk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2iogczuiz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lbommexf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jxomseax.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ncfntqfh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jilscqay.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uauapuqt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xufojdvt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gadluonq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wkatylap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bcweidag.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2llcvugzx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vkgtlgno.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrbmgke.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fsjfugod.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cdvsizzc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2taqothkw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vytwvwjh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rdmxvoqi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xzdadkgc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vjptkiub.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxorerje.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fmmkcwse.html


<!-- 参考信息 -->