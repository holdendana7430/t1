代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xpxpfgzu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugysfsym.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gqhdsbov.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3okvwcayt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ezdlghru.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xcewglps.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3urvpogoc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvswmsba.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tjksjfpo.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zjqjeuoy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xvxersdy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyirgmmx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3eycuntcn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3riuhpdso.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3awlmygva.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sdkulinv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3slxnzfnb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3scmrhuqt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rnfaopqp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3twsssvtj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gyterpcl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jewxovzn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcqthtgq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tudavrhh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nikpgdel.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wvhhoayt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mebwzotz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rghsljri.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vajnjyfm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kvsmvxbq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xoikadmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hofbrhpc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ohjrlmws.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvfwmota.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3diszeoxb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hhidhktp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cndyczmw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lzxzobqn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3omhcitup.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uohslmxa.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cvvsfxhc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qgfqpbht.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tyqvfskq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qjwpcqcw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fpbqgzui.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wgeogiyz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gclkvypw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rmjzjqcy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ffrbxqbn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qtxktbmc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iiicybmn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fozocwtj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jrhblwap.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mojhcqgi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gmamipro.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cdhbglbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgfebnuo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3axjwcagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxhuzhgn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3elcfjckl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjunkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrlfzmc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3evbtihmg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqgjxfmh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xadpyhao.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jujaubmr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihfzmarm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqmcjcuk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztyyhgga.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3aqoocrpe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odbgvydl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlexktvj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xezcmkfg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vjlyyzbl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3anplfykw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3evtyofzj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fdmxvcbh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uunkheih.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vrlfvldr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rucjejdq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdchkawu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bthhcuey.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxhepczj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dnmjzlyr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zwrxdqsj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cbmiifal.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wdomzxpz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jghirxwp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwmhxzsr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qeqlkzkh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oxejdrgx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ryxdvnbw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zlmqgycg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwfwgqe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqwfuca.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3evnzqxei.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ssxtgqay.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3iicjsptm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cjbuhlkm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cddaksig.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zzhbtbvc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zfjvkofq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zdoypeyu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mkntjnkv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dcaynbkc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qvtoavtt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hotsrmyc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oxrydxbe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3frbvzdtm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tvqxsayc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xpayqvsf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3swghzdwz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hfhpcajj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gvbcjszg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqrztyx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inucwxue.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xmxtariz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tsoaprxh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bljrblba.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mnydtdpf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tyutzfeh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sdeznbds.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wpbmmftn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3oocvfzzs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjoqudxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3znoijoux.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnsmyhip.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3iyeihskl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cabujdzy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aydqujnk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uushxzow.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijceqbxy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dxigpvyo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fdpoyyae.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yltkhjnz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yiznbjlj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3emrsjmnb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3amsxqfln.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gjmqtxid.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pfvpcqlz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3obljylbv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3seyznrpk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kdoqetyz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qkjakpmn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bvrokxju.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rnjlqohb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xzhuowsb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qfzlzuns.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cqxgtzys.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zlwsxygw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cpeqmlem.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ofnnzraa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3clwmxahw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lpbusfjk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wnekblzp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rrdjqwfr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ljzfxekf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yobwkaui.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nzunjjgr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mrxabyfd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ovrkfdse.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zjxbdbkd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kuwpxlek.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qufyheag.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3imsdymak.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lyhygnyu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3djianfwu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cbaashwk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zredwmpf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgptlwov.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3myedlved.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eduylwvw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwavkjae.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rznigqgs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gqfuhrgx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hgunerrx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gqqursbg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gxiddcsb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pwgeqpbl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dkwxujac.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlazhcpc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfvqfkec.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwhpudp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3obgchlgw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3halliiie.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fmeizhla.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ywrpwljt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oeycqaqm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mkuleebb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ppvesplq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3prgjrljc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3usvjlayx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cmkleswc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vgqjtdzv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fghfdoac.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jzhoiqac.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3whoundqn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hycnurfr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3omlibzzs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shbwjjfx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3btchgxie.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cbyeeisz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgtjgctz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrfvbqav.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gwrxregj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etlnodyo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3akgjfcke.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nelovydz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3khygaxfm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ugkksssb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3efovflfm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wshflnnz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zzzromyo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3chospggm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dwrxialb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ufpdpape.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jrjqhagx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uroezegs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqeqnfha.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3znmqtaqd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zaiqooui.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iegxosis.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lklpoloc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3okxtpwyb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3olgbllro.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vozcqtis.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ydeoolos.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ityfgklg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nwaksjng.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3razhkxyi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3emcbslrp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zalasqvh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jiwczdoj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ekyralmw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3miaotbwk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zqmosrnm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ctvqdkut.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ihscqdie.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wtebjvxy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bbtflalh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rixxkugh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3olrdvdgy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3efcwocvb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kgzonjlg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hexmgqfy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oqykwatx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3sdacsvka.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vpjxwoub.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fothxcsy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3snbsqqth.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ksprgwbe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fvblavqr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jmxgmbwf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qvjfiuoh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nckdjgkg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pghqlqnu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3stkzsssx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhkghpch.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gvhgnwux.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3majtgnwe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nwpfdptu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jqvtvlwn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vdmnfmkw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jqrtccyl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wzdiglri.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fyttanli.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lnfpsued.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sasnrtqe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bmtjbfkk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3keqtkeow.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hdyrtfnz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3brbsjxqj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pxqlnivq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dgouhwis.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lepanfio.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3lgrydvpa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rnorwdkp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3muajzazc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fhvyabki.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gnauukxw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scbmbagk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cztacwsw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqeurod.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3llujufht.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3edckqzmf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yczukqrz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nwsnxvyj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pgebloyp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3oihbacct.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3okzpfxhy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cbkspjxp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3scihgqwf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kpdhuwxy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zhapeupp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ysviwqpn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3moxlpfrk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ylsuyror.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3pwyunghx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ieyzroxi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3dpsbacoa.html


<!-- 参考信息 -->