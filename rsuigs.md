代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rdocaaaj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vuxjjiit.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nzjldqxg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pztfkwvj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cmydpxjc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqcjlbyz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3djefylqo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yrvqmjop.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qncjlqhb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dcsjjdjq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fdmfythw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vpsjkmfk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sctlpfyl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jbnhymfd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvxywlcc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wdskclit.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xuggzlmh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tolgplug.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hwhdfgrp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hkgxysnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hdjvsgeh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kdabhrwm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pmuwwhal.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3froeavgd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qjakiazk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3uajkqkbq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rapifnnu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jbenhttc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tupskqfj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xaswmlru.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3teqcpxrm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wqstjhga.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nsivpbge.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wkogkzjl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3nieoujjk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zilgwcfu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xiqcudcw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecupsfdx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aaagprru.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsmavevk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmeiddf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gobxrphb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sukevtaj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fbpxzvmn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3juteyivf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xlnerjea.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nioyhpgr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gzgzvztl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3voytpkmy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gzypxqhj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tzecdmim.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3itgflymf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bpwnhbja.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gctmspcx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3clcxqodb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mgljhunu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kduyrxcr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kuylezqh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dmqowlfh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ytrdzacy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsltloao.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3imwzcayg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwdgenkx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fnctmzgj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zzyqdjcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icrbpxth.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ztestgoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ypideagw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rtiuwbao.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uvscqwda.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mnyucbfd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3unyryoha.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3woxbzwaw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cmetjytu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bftvfxde.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3woemubzk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gfwwhkss.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bhruiiml.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yetcdlaz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dnqprxlo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wpwtenfz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwuhqqdz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vjwtxgve.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyikcbhr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnafeqvn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3phtiygcv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lmfyoauw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3srgzmjek.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jciuxvgl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pqwralzy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3omawialx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cnxhctts.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jgotiwok.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3efesrkjd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3isdnxokp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ahuewqxe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3emooexfj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mgayaeqx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvbbschm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mcckkbrz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jwjnphrn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cfqplfpn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3urpcanrm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3shjxdlko.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cthfkgwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3azkpitmk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lfvyxnrp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vdnnkfbc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3avxbjhsc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3efrtbmgn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3thkwhyof.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gdwkofzj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ueugdnag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jrvlfxsx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3evhdqwjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kmpncsqm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lfuozfny.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3speusexy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3saxibhur.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nlirinku.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ltgxgerm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ykbvxvxe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3epmjnuir.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gihokeka.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3oepeoxmu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3emyqjeqq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3makqqxhe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sbzaaiwx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dqaplfmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eibpkfcp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3upfjklcs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ykxdumbl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3phehbgrs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mhnxvcog.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsizcpkc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwamecdx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmfxpsh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3euoxoxif.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3etpipyrp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3czbyvidv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgjazxop.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qxypwmel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnypamo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3orybmrad.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pxuoyvwm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3eksthkjp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wqawnxrg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tnwcjdgp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rgrijtxu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lslijuvo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ewgpfgjp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zjljzjin.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3unkuiwbw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ekgklzfy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqykah.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3eqqiofwm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kbgxtnfv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yuqdjvfa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xqsuojel.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zsjiwdxg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kvgqbzwf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3huwfjszf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tmufkijt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3zibovrgp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vtjgimsc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fevqyixk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3seqjqkmw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hmyjujsf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3iopuaxzm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zfmcssqo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yunvkowb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fxgcjwym.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tfrdojse.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3njrvfrxm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rvjqrfet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bdbassrv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgqmxend.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rtvqejge.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xjomamjy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vkmatbnx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wwetowyk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dyzimjzh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mvlvfbfw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jcrqxakp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3osvcyjtk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bziwophj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3droogelh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3atgkzkmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jgmryyzh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yiswzosa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xcyyohnj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rdslzepg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3khghmrvq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paoeggct.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nlruiwdp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3maswavel.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kgnizgzz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wiudokcq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lenlxarw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mjwicyka.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mqadlpxf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3igfjyspk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uzfplajs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3htymzvhq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wafrpxwk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ifbgerwh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrwnrtym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtwanijs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vudzrcnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyusuzvd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qzwzqoft.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pwppmdig.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eukpjtuk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zdtjbgvz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3iyiwxael.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vdoqsjor.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pntftygw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hgxrgszq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lcuwqgoh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jxwtwyxk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zvssyerh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bpvyeypc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3erltszsm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tssaylml.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kefevpvc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3imsmzdhg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hemqnsct.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3krwzyvsj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3bykffktv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jtgrjset.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vywhwepd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3epojioft.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fckqsiqf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfzzrir.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jtyoyrca.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrobael.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vgufwgof.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ahnscvya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3peutnzik.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zmmjovkh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3heneiuuv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bmaojlqm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fortvndi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnjxkum.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3abrcguto.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qsrvdbbt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3stjpetyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qchnbuhr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3djpnxhhr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mafajrgu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3crwfaibb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mekodziv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mwoaffum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zotazwgu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3apmwsosz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gnkfudvg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xapcteyl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysgdetku.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mabehxmt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sdhmyvmj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ecdrauca.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvdjjkdj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aspohxxh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yiumfzqv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tqqhapmh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lhtotftp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3egubghim.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zmewcnfc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3niyrbjyn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xnfgjyoj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3orfmabfu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sbtehuoe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ysnusvrt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qupctnfa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3huzypdtq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mchiengg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3oekhefij.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qfessxjq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcxlvjhe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3twwjarwc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jgtwxodg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pqhlzvvy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3kgtpfsyp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3arokelhw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dqxythze.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gtblmofc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iytikxvp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3enfnlpoj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdnhdvr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lwnhjpka.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3brcjonih.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3zhihclqf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uwdpimkm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fhehzpji.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xttgfouh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ziqfknwj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zgnvtwnr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qkbvmccx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcyvjot.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kxjswatq.html


<!-- 参考信息 -->