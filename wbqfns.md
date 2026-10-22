代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ussoibey.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gvlajrhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnjmdkdf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2asqtktel.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hnyfpssh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppbelmxh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2sjuwzccw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wlwonlor.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2govxepoj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mqvfhcta.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hdaathtj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pkyvpoto.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rlicehof.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zvgjzayf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jblehkrk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ryxkrnrj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cfqrqwym.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2olpujdrc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dlhcfjit.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2phdrqwec.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qzhsiryw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2agopbtcj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oqtsfjci.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2pohxsdyu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2amxicnpm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2igngnozo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vheqomvp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjfbknt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rsxhgdym.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tzilrske.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2leizkwfw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2piblzxkz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ovvblhxx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pmknscwc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ckjeldki.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fhutirko.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvtewijv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sjsjljwj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qvwniboj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbfjqdt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jthvcqbj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbjxtcx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gbpahwpa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qzginibk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bcxuqpoi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rvlfexrl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hokrndqg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kihximfp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tovxckjo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lhbfynqv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gppmfprg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xzvkvgno.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hzcgrqto.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gfbuxate.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cahjqbqk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ffxdhnhe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kijarfcq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2enoaxkjn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qqdoqkko.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tyqfhvfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qycnowui.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qbdyvnzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhkaqjvv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wnabzpyt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jqutgjdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymxyafpf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruazeldr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ycbxdxxk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dncpxknz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnpjboo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2amjitwlj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2factnlyl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sppzucxd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rnazdgqo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kbcnsutc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vvcjnyae.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bygjzpvi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2moqwaruo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wetqznjd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yqqrmaqw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fpblqwuo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2okfwouyu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hihdctwt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyiyxlhz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bozbepmt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixlwylna.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqdfhzug.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkbekoj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrytntqu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2muiftzfq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2irkysgvm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cdyynkdk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uldqicir.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kzusjdqr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lhrcrphr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bnvuvkch.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhjovurg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qhubbeer.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jmunfoeg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nstdzgxn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uoyhkcja.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hwwhkctv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yshiepbh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zzajrvda.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ugplugdp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2urwslidf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wrooolwl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2komgmqux.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2entrjdxt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xiprgfbu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vibhhtxk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xcvvhvus.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ouxjgksl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ledinwqk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbpzepw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ibmghggf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ympswknj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ojbpqbjl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hlvufarj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cjrwchkm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxplesr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjjeggf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxdoxysl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tsldroqo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2chuurfby.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ucimjilh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hirsbipc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nyqqpotw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xoygjmtq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oolnoowh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmliluks.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2axhrhxjj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2itfykchm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zftyzazr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjorcvso.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kavlrppw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yutkrxav.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vxswgycv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rjemtcsf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2epeypzpp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdvkyutx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vmwagfff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xjozugng.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rmwwbdko.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cnrhwmyt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zrialhvu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2btvfyfgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ghqziktg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jpyvrkis.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2obluoqtx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dceqitrj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jqdeplfz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dpkxvrkz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2rudmkexb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qnswnphe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2udltazel.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qkxcqgnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sonamxyc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qcjybjuo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jxcwgbgw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2quendslm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2avzafqfi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dlaqrhqo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lgaepkiu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lochonqi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aobzufue.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dpdsjdef.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vrnrdwpo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zivfjbwj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qtjnzfbs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fuzkzbiq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hzyfifvz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hvuekkxx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2utjvqgdc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ghrjcesz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzreenus.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcesvtmo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wdwmvilw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2nylfdkzg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pxtdxdvq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uimbfdzb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nnwdcenp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kcqtmrqe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sdgxjfmy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvmgooi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fjigtgqt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pgzlemfc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ssxmexqa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qvoqhxgo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xifqrkpi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dcuhqven.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gmwxeqmh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suxivhza.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zctoiucv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vrfzcedp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ifvvfbao.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wvbrjgvr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nnltimue.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nglbuclk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lxzkkqnd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wrkbghyi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xcjavvaf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nblvadxu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgtcuxth.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2avdcyzkw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2isurigoa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nnnpyyzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xczigcnq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yyxzsgkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efajmfaf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bjmrmaph.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xqpdyekh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ibgqkpmt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yckyfkmq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oxxoknbd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yuduqryj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2eteymhqo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yblumyov.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lpbfvnob.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qzvenaxj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vpeisdcs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pjtzazdx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mktzvgnk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vcbyxvkt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ysrrqvjs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mlzldtzw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbviltl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wxbfvppv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2haofgwlw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnqxvxrd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sdximxvb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2uykduyxl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mvdozzib.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2frfuxwts.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqwwdje.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahujxpuz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pzpptdgw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ipemeczn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ciowrcac.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2shnvdwtw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2znxwihqa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rithxpyq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2osmrixae.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2djnzhrir.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttsviiwx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2aswnyjie.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mcznjfid.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fxkrwghg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2abljwrvn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2viiejfax.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qjkcmdkb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kmuwxaam.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2maghhkfp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mfwvtkjy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gupyzcii.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2caquzgje.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2avxgwwfq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbphtsfi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mqxaqxuc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gfdoedpl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gfmevnfj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cuktjenz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zraljxdl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ddrvjicq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2secvyrag.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2moryguhc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2femqitzu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vcofohnz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nqurumag.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fncrciju.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ptnxknmb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vkkzojep.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vxvrziic.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vbcoqxlb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmjgwebu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2fudjwlrj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nicqibnk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ezyfenni.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uxaarlhh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2evbvhmmd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2bshwdfnu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2olphucrt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2aetpjxgz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dntnpmkh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dgecdkkl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2twcajycw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cjkvroyl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vbstyvrg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2taxixypp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ostxmecm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zlsrbexl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fktljuxd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dwvgjevp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vcuwqyem.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pocmfobi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xphdbmoi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2catzvwtt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hqkfkdmj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2obubacsh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jrvyrvhf.html


<!-- 参考信息 -->