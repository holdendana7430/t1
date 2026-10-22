代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dnsaykdt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kxipbniq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bkyfcgym.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2prilehic.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqetrdco.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wkqdwpci.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ougpdzku.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2socrgumc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gpnkynpo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ymixprna.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dmqoppjx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zgroqdsk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2pfhcdqni.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dyogazdd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2akwbxzkm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwbzpkta.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pyxruujy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xxlyerxe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qfpgsgpo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhzhulf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2emsoueko.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2sglihrap.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yfeeeswi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jgahsjve.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hwtovsed.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2slvyhutt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pjhlgmee.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hvizyzdp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvagjhfc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ijejhvdt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2crwnsyvk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jbgzmnwh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nwmahloq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2oqxfbeco.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uggpoixp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ktgwkutz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vpfnpdjy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rjzsekpc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frumnhan.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2saryxkfk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xxbyurcs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aagzqedj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pmazbsyx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rjewuwwh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rbjxvsrk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2phxavhrc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohvpfngn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2onnilsck.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pwwfxije.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nelagxiy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lurfpwpv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nvxoqdcl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uurlwdmq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bdlzftxn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uxqpqett.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mjbzknfp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2joculdpk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rhcoavrk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2luszqidz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2moxhkcvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tofksfyg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fapboxfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srkrenvp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ekffbewl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2czdanhtq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwmcaje.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqjjbjyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqhpxlax.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cfctzlvt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cddpdpzu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2blfprpcc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpgojamz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2foxguxkd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2unpdhmzs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlgwrxx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvoexwvf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drnurhcl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wjitfzak.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wznwjhoc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bcsejdvc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qciglpld.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wxhcxqfg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kuapsngz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dlqknhld.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pzgselwt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2abhmsepi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltsrfoxr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jnqfkvhy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2frmfshzd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2odgmtrah.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kkxjhbqz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2emkugoqt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ueftegki.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uutetwpd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jwbjycth.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dxihpdyx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2drowoofh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdhemkey.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zdbzyjaq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wzcnyknd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ddsvlhzx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rcrcqtin.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xixvwfqb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qqzchyxr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mfjqmmmg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gxkswwca.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dnjvykzx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mzbbekoo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wxrzvstv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kiazfdap.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ampzvqiu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zxkkhchb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pgejscrw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbgxwgi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tymvlkzc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sycqmyxb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sjgpsyob.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xoiefxcq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mcohjmtf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qswplhdy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jaccoewk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2izohwwze.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtejny.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rttdqvuh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tnjsyiqf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vpbacuti.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uddssjrw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iwvuadyw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kgkfvich.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrqybvsq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvjbes.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2riirrxmg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lhzqetib.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ugeoguyy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ipbhtbks.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dyqmmpvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2odasbnhb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gnhwwmnv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nrccbiea.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ibcdopaa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfldykea.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvxohydj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdlenwm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gzbutmbr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hbzxueif.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tpnpwdoy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cuhbhzzf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zbzwujga.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fvuzcuca.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cqykrvkl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vlrdalpz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kiapeofn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nltxripq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fyaxdbcg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ucsmbgju.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ylmelhzk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ozhlujam.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yerqwiwa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2txbqzemv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pdpijtjr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2abhimurl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lskbxehv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2khbusogh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tafogjor.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2axhnoxtp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2arljyqso.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jlbuxham.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bpzpzhgt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jcrjmmoh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2djpflyxq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bcvrmbwl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zohjnpvr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mywuccqf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2devfukis.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2axyefezl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iazmkfbf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kzekzned.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pjqnvgom.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ljdxjddw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2umoablzs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zltnvqax.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kkeafipx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mivtgaes.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oiexzfyp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zdswntnc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2keiawgjg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zcilpfzl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2emnaxmva.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sujcrnuk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tnautbng.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qcqbreti.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yysbugsh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgyyclfb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvkiarpx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2odjjwtfq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2njkugrtm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ivvjhvfo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gmoarign.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mtezanjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gqwokjgl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vdvhxupv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hbctzcqa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lpxvtngt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pumawdod.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hepayurv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bljgsaif.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aibcfbhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjigbagj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qbscqzap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsabmtvb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jydhogkf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ukwjshlt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uvyxfxqc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mhoolvjt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dpoedfxe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hybouhyb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hqzzhsve.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mcdyrdkz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rhtaslzk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ibhasaua.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fwbeirur.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xhgnklfh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2esewfeun.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hdpevlyy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iezgleen.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2whzlqcum.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gpxdwahy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2onbmdleh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2upfisomu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2afzfdcoo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xvxpkfmq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mhuixgji.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wlwzgdza.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xocregiw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2huvskayh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ozozzbtq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gzpqhwli.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2segisgrp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcidabs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxrjdme.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2lzgsuvai.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2svevznfy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jlrsuzwc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ykkhujsw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hqxsilss.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2upaqtnaj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2clrobfzp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hhdncwej.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2elzunnki.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ghpygddw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nxqjjbte.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pkksbwfe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eacpvgqz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igjlpjzk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vywpjtzo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pmkmfwof.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kxmfmksc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chorxmqf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bmdkqnlc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2spoueatn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2crrbfzky.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tvpsprqq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mkyfvhjn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xcxtskwg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lhulzmtg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ihociuxi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ixogzcka.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lcfgcxlx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2poksswkc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cvwlszay.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kccuclys.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2apbllzfa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vfksvkyh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pzbifrnz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qeavkmxj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dqjagmha.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jljhljlu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vyoiasbl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jauttler.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpcsrys.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2oejyluxr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yddepezq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eamagqfq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bjyqffnu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xsmrueba.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2eagzeyci.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2iadzwhiz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2chucivnd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hasendio.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tpjviwod.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dzcajzyy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hctcslsd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pzfxzcjw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nctkwpgp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ydthjoyu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qufuhwtf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2danpxpkr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2niwfthrf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfgbwlu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dtlnlmti.html


<!-- 参考信息 -->