代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ehkvmwpw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jvxikcua.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2flixbpmk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gylmpksv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oznthizs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jkekkamg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2txzjzwfr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xkzpeqep.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2duoxywyd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2neydqhvf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jvalebse.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tlajibzv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kjyiqbcm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lrcismjs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hxeqyeob.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gryekipr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rwkbftyh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pseorynv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mixnwefv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rjzoyoog.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pcvewnhj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aggmsasl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gebprqjv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yyhgeivm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxetkqkr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2obkvuwod.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kegjgrpt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2csgrgmfh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rfqcwuae.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vdhebgsg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ibdaiuix.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebquvypc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwywsrsr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ysvzqadl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lxtvjgtq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dsexodav.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2weadfbvk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2sllvhoej.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yryqofby.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hkgbbolv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2htthfueq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dmlcyxdc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2quwhlczw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkamvzmp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipeprvip.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2drrzpisi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rvkuczct.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qgmbhdim.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2skppbmrh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wkggcvfx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fgqprwln.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jptrxxcw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tfbkwjmt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xbbfvxqe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tqvmjjgp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xpbutcga.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2spynmipg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qqrabtiv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ytvvauqb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fboughoo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yimhzfmj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzlcvyt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2esxpddqr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yzffssrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emuhauop.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sqbeacqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbwduhzr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fnjbaqez.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2odpijwga.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qmmfxuyf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ogjhsnat.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cfsimqrs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oqybujwx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2srxvamto.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2etjrdreb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nytlihtl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ryhpaipk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ymyvtsru.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xvqoxust.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iemwkjhs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpnlyny.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tztilwio.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxqojznp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2igbjrcvr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jepsldwv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rbosbhgw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mpuzryez.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kdzvmbgd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjassmw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iivaqrgb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wvwpjhxp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cbsfmpys.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cwpzgpnq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kqpygyoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zaoqiaoy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2poyefdjf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2taenwawq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fohyohkx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qwrrkwsw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2aeyuybnj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2szykqonq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dhfdjzuy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekbfkztd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fekdtphq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nomvpyjw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2punxwmhm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rhsxchyc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kcwavvkk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xujsgdwx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2waojwqye.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2paikqyvp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bjdzbdle.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2holvmlny.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2slkuqmbj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2olwuzmku.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dmefzhhy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ublmjiel.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ncqonmjw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2tbtkeoev.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dxkknvoh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2riqiaufw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jhjprdrl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2gkbqtcyh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vavjxbqa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nujbeqlo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yleumwhy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lxzwanxt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2txyusdrw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lqfzrzgh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2fbdetogd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zagvkszq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2merzcuow.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2clkkxuuu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyvhmzqw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2acsbheez.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2uebfhobk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dkngnsdl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jutfnwxs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcxthufk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lkaboapj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2taxxxoik.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfhuxvls.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2doqajnop.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oesybyoy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgchihf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qwhglefs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iogzuuxk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2atunoaiv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tjvkuesm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iwkgmcya.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sjuxqbbh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bgkugogr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pxuytork.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2psxrdlci.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uynpqyhs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2getzeexg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fcafuwrs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2allpoevf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ebovypzb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2mraoofcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2olivpxnk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dpbfgswk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lujrvuua.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tngrbpuz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nqeekcsx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2prwhmugs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uzgsmoop.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2unyvgolh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2eujbjnmy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2scgyedkv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hxidgvvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wowntekk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ohrewelg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2itwuhzwg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xgoibrzp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hvirywnt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mbfwxgrb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2piylwohq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mcljpnfg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ubwhesrx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nntnmzgs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pkbefpxs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mogvvbcy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jdhdzfuy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxptkoig.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uyrzoxze.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vdyslugt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aupxiaml.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tffkzfqb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhbpdjh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hrjtmoyx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xitorzut.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gmxhzbdp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jgxielie.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zarcjxax.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ueqkrefy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzsnbjor.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xligtkas.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nekabvyh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wupssowv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xzifjcti.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkauob.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zrsnuioj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fyerjyrn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kglzxdge.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dbfaaiwv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oshumege.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjmpzklf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bvstopbp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtyotb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmyotfod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dujxrrii.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2czxgiymp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obmohzih.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lboyttsr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nnwaajgs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gimqfglo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gqdahxby.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sjfeoqyb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rzcwawng.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yayjkddt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oyywgmlu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xfkpgzqf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2zbthonro.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2eyewkafn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wwefvxuk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2miaucggp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jfhexoqv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2osvfixkk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wzucqrgq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uxknrzxe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uykththa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjxpcyrj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ktdujqcx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2aforenuq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sivucmhd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uomnadli.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mlkugbqj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wgyvawrf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ncntzqvi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2btwigojq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2knupogjh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rihkuuyp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2plkisisk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yeatswxb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ignmohax.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jqudphlf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2daukfdif.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpopgsng.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvdpmnjn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gqldpauk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qgwobuja.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nyvafnqu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrjljvi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pvpzsnes.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tgeaziqz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2spwfdrss.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2adhftgiw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ueltqrhk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jfoeghve.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmljhuiq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hayyvwdp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dicmfrsv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2elavbjso.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2etfhjiyf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwkafbq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ftrrfpiw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2acocnyrv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2oqtwfods.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ezgahgbl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rydhiwws.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hrhtwghx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wfmqxsye.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmpntqmg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yqcisfkx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xhixdysy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rbykuyyn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2scvnlrbf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzadogg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ptwgzwzd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2feofjllj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dfmbmbyg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2utapeulj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnlxinc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjovckfc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2teaikiav.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bplvgqpi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kbangcoh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjulmgof.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vqtkviao.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nvzljsnj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jnqsnusd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vnenrarj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2czlhjjrb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yylziukk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2smixqbtj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zqffkvgn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qqxmtarc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fxizofti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nixrlriu.html


<!-- 参考信息 -->