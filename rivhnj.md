代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jrxfuzzt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2veqdufdr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xecvozee.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dnvymagy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vqkcvlgn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lttkqpca.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wzxfnawu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ugqlinzz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lockvovg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ofumyjrp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zzalezwv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmunqnat.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bbmjluhy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2drqxlicg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nbrwvssf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cuqestip.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xdpfkpjb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ghfrxggg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjdvnooo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zqkssuqt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oilbaiqq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rydzobkq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2frhdpeox.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rzcrvpjo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wgmyqfbf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2csdtuxqt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2esmadxzz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wckgqzfj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oowzgpwo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2iysisgzl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mthimxbx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2niqnwqms.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eqsjhxej.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2umjfnsas.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nvnddhoz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jbbsuttq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdhhhcdk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffudiqee.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ufpgmyrd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wteckpkg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2beblmfyu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjggijyt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jzelcnku.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2icygaxrs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2azhzdoyr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ujfryfrz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xwpoxrur.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qilygqaj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gzoclkzy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wujzslkj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2crfklnqe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ugnekzcm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zrefufrh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zumjelyu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2agacwwgp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rpfpfmst.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qzbmhhrc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2igtepwfq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2egobhzzz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xgedpyhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmqioaos.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jkfteujb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aexhphec.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhcizbkq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sqljobld.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jutkeity.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vvautxlj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vchbxgwl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2absnwcex.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ocvxpfjm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zuuraynj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztjxubqc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nxugehle.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wxftzsms.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rdncfyoy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azjljlus.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcpfpeye.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ldllksyx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jpsrzsiq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jnojcfjy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zacarhhy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqekfdnx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lvtrldmx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2iptzvwqd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivvqmpkr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwtmhthx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kirmddmt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lwemaqrc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pvknidei.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xhnuoytk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2edglffgg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wqcblrtt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2opfpvqwv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dpzhkgax.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2egmwxmsc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2evutafzf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2enoggvnb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2aemwdpnv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gqxsgfjl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lcjzxoml.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2axqdipxb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fsavbxee.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kefgnwwm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sehfgeqa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ydgfrorh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mzriklhp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pyqbqfzj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2byfadpua.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2normmxjj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ilhpnofu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zmqkkthv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ycilneyy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eevnwhjc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rywtayun.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wibpsqrm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2czhbexyu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mlozrsdb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wnacjfho.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2aqgjccwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zoojubgf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2batickrw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2saufyytr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lcjugxbs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hhzhpvux.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fcuadapz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bxwcedzj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wognitva.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lqkjgiiy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvrjfhi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxbvjbmq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zozmgpls.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mtieophn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2etaspkfa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2awzrcbyu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gkfnxhed.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dslnqejl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2opsusmmr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdrvnzou.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hwxuscmk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fsguehbf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2phuksniu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yfoeabmw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rfdvzyna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ptlndnmd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uuhdljvl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zryspgze.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2retfnsrn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vdbfhyrm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tvfutfyn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zxdvoprn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqwbofpx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gojrxdha.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dsifwyub.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gkwwacnh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2odjxqoki.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mezbgxuk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gysxpabe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qaxdhjlq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uvrgmqxk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mgaqpcff.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yjcoayeh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wbgoaqcu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kkuuwqws.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ixitcmbd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2llyjjvay.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cpyrigxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yvugjewn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qmhrruvt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hxmcvibu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vjfsbhbf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2libizxuh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2oayzbbib.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rhsagxdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rzhldukl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dwtlpyos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gzxjzvdm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkoborti.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wjwlmkgu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mrmjbwnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2soskzogg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwvtpzmn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dllnvndt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wmnujidi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wizguyrt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bepnpyab.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcaephfg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kkyyvhcx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2umofngcl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gchylbiu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xbctazmp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lmcikfdj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xdmkkrfr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2spptjmvo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vejutand.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oszltzqu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xmayfkyz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tsleljty.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yzpshuho.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jgngpthv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pafayphs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gshmitjg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fqmpodtl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2esqwohpu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xusfeweg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yamytnog.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ectmuigd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywkqoyzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftipmdfx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bdeftyhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuexgexr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eqnoxpbd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zqzkgams.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2acyjqkvy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zesctdby.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2swntkxpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xcvjnhaq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pcutvqam.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2huhfennl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lhhslqbk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2sdfvwknx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wzwgvpms.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ktjrjtig.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dbptehik.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vzhhxcvx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2etqjyzzf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qhfxuteu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zotlbezd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wlcvzgsy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oqtrftxh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvdqdqo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ekijqffm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2yonipbua.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aunpvhch.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2svlfhint.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fdazlvji.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fbojxklm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vboaagop.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dwhbfejx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hspaphtv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2amqzbdyd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2usujgpcq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2clrhxwcb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bbnwqxgj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2horxdyse.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tzoozajm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dofjkjyr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vykfpueg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vctxcjzr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zbfjwcek.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kdvvetab.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zakqbhlu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ltduirkl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wbajcqyb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ufnabvcd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pyaugieu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bpnbcuol.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2firiklza.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmwjewdk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2noxusllo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ogltcnmz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2khwlkhig.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzutmecy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vbsbkajp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2foskwmzi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2voahkrvv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2imbeljvf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ijkmgzxy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekyjhyyg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mlteuizg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ppybfzsg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2neqwkamj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hxtscynn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pyshtpps.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ctbsekjx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dpdlcvjz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jxewothi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2kvtpojnp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2iznyxurm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uqbzhkog.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmpjhdl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jeayqhwy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cuqhezop.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rquejweh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lszvbjkh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubbxbxkz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jbbavaai.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hfaypcku.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mphjudnc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfoudkwg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lxijvshh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cmiyhwkg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tifggmrc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhyyomx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwunikf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qzrgekao.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bpmgmjnk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jxcfixdq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2aghsbgoa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2knaxnops.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2plucbbsj.html


<!-- 参考信息 -->