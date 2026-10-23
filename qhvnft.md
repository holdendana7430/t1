代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3otygmwbl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3swmzonqo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qowbfsli.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bxftyctc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jmfcmqqm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdpaenqv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3blfegudw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fhuxsiov.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbbyihtj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rjnnvxqo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glvvyqub.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ubettzsl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ckohhhdl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ggxeelao.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qvblfims.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rsbrvtmg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nolzinqb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nknsndeu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3drgxzekb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3helswddu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jijgjcgj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3jektenzq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3focorsph.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xsdwcugr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hrwkoqyr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3oxbicdfh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3urvatcsm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3faumgfsh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3elcwoxpq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mtnyiajv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzvuhgb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dbvwebfh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mvgqctxo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jumnfgrv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3znxafruy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3oczzxohf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utdgxymz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwcooqt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3boxhcspy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmcmzz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3flqrthcq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ackcdxbt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3deuzpujz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nowwdlle.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jdxcybqk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vciazvth.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dbxxlaxo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zspwxeau.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brrwigff.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nnaodjig.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qjadxlqe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zbpufkof.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ewoumpco.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3htzijoqr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yicbjrxy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kpdksmgn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gxhfgexn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dukbmuvw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3syktfzdw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uyhmufqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoeckzxx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kizjcwcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoxlybqq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmwufxtt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ychobwlq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgwskozv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xadwkeab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zujjqvul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zpmragjf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hkbkdhgv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3guvghvsx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgazekv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3scsqwafi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3drxhopos.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zwadbgoo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrcvqjab.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dvpeqwwr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cwphootr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ibmijird.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ptgifmks.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3tvkiprec.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yuwmxnpu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qrqjvcvl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3alphndxu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbhhtjvs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oqoyirkn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pctruquy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3axldhmme.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ljleskwa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ktwddlrw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wiyfjwpw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bhuayrer.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xqavurzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rqfwodva.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qhjiyhvu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rpotfenn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pzqgoulw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmrhmby.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nryiladl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xrvwqcgu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rcgvcovm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ftthxdvg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rudredxe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wfmnysre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3npengvyd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3buqgqdyd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bavcwzlu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qkrefzno.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dolyblga.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ngnzfbtp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bwumhikw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tgvoywty.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mdunoefi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mwnxurun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lfcocprq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vahqczvt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oehztjjy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kuspympx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uyhewike.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3biuarvaw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rvlhkclq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3krujpfky.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dzutvruq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hutgvjqi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3viuelvza.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wcrptylw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bekbmvqn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qtwvpvgw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3eadzwxnu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hhwyhviz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3icetvrwb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rrpnwxgl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yjndqvoc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tutibuhf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhxqbfyk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3swuntash.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3onkbphiz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqyewlah.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhtmmx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tpayxydp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfkhykyj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uwbvzuod.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mingzlvs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jctwpvaq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wucjrjma.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ekerjsar.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tleejfme.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fwrdovip.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qldyvknh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sqdekcab.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uyuccgzq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nwoskhaz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3olwhcpst.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3snufykra.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dymbodfa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3enwueevb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3daojodch.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3pafgqtxn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3andzpzbf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jujaoahu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vfqgpslx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3yjpngvcw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nfupawff.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3romeelrd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uelsrvtj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jsibnkbw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3byylssib.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xmmbmcqc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gegjqszj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3shmjbaqz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhcynurp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mxjmuuyj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3agwrudlu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3prozzrrs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xgnangff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlniscer.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhwzqvno.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3izoxowab.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jjrjorts.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3khcpmgbt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3miuupatf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3wkvwytxo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bacvbtdl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jqnxzjnw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3moryuzms.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgaenkb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vpnuhzdy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3srkhxajr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3iwjtmwvp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3omqmfxvh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hiynhoif.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qlaqjgpn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aurarrnb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svartuwa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wdvzokrj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dqupezwo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ismmpinu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3apiefwak.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3urpfuzfb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hzrlwcwx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ljlbzmjc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eghlcjhu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tpxxtgix.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oihpomer.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qpbcdnkh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mzfzukdr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ypiypizq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3delsragu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mckfdrcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qybbeumb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jaaloldp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ncqmaunn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nhoamjlw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cxldddsg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rbhhmalb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xhjscuwq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3flviwrnu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xuqooedp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3iuycawub.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3faukrgwj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ikotjqkk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jdwrclob.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xoplkgdj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kivjjlux.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wruyvfnj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3aejpsnez.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nnnzzqvh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xkoxzkrd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xflawinb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqbajpt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ugynyrlz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ndfiviin.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smytzxej.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wutqkxan.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3djoihyxe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3drcpsqpq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bilnyarf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bbykxeom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3morjrovm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3efrzqgzo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nqbamdpt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3eepxulst.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xiyuogfa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xcthddyk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kgxfnndd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ubavnabl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3iubcueso.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ggaojpln.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uigngwvg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ikiviapm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uhrrhwan.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3acywcgai.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3svbldyxz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aoniudjb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tqglutjr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkjfiimp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqvidnn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wpvuaeup.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zjryvrhd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3prelyzjz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wckkmttr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbshwqkp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rurmazyk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3eruytejz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qtkbpicm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qumdohvs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zszuozwp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hnbfnmel.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zwumjeft.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wttoejtl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xwgxtdvw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qgcxitid.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sqpwxpba.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ygwirrzy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vbwvcaqw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3prlaonqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ckfuxdgu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nwdftswd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqubmndj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uzcstfyl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sdyojraw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qobdscob.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qwqmxkxj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xmyptckl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nburgtox.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3boduzvrp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3imujqeqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfidbah.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiicxyro.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nxpdubor.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ijjjsfuj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pzlwxcan.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nrjjluew.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwuofbum.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3awxtdbao.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3srtccvbf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rkztoyje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cokumjoc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3msdcbvth.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bcphedqf.html


<!-- 参考信息 -->