代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mxjutxui.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qkzmrinm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkdmjcxb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3terutezg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fmthnszr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gbsdokyl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rvkmedmq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kwcquggm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cfeyersk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uxwaxvuf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dzulyvya.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vrbwageb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rgghzpam.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yppfciiq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ftooxvbo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxyvzhxa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3stmqkyoc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xamsmplr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmdxflim.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3armgftoz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qcxmdpxk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3sgrgfuwg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zknwgkkm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3itlgrvbx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3nsnafwfi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3glcvxuhc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3slbzthyg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wznahbcc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hljicjzp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kexavifs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xndfdhfi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfsfosg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ttxrfvlb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jzjczlzl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3aqcmlznb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbbessh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjpfkgaq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqqkpjb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhbzsjh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pwlheekw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsocgyky.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xjguilab.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3hbbiaqmj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nvlnurwj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ojezrxyx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gvonotkd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zqxzzrhy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mwcigcgl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tztbreib.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uapchvxw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3udmpzxzt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3panhmdbz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wfyvsgfx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wzxhiaht.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mkdkfmnn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lwwsuvpg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3koylcwtd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kacaknhk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vcctlhrv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pjjunuml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llmiqqnu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lhkpopts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlylgyof.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoppuclu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xgjzxcqq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3osdxnlrn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thbolonk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hsfynrvc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uqinduvu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zemgzpur.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yvvvmjfu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgmlwxnp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tivuamra.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3awhdwhdl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruuanmuy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azrejvaf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cfgkaian.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ufezdklz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qdebgycs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ooolyvqz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dqcydplj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3taockevh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xocnsctd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbbknkl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yexpiddu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3llvpdxuy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gejkqksv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3atkqfyyo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3otxykews.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yqbdpngo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zwxfqdgr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3stmlwsgc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3swnthaqn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrrzqyog.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nugjtfvq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3qtkynupk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwdbob.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhneprro.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxprjipe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3uhnjitpr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wqcclsmn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tcznwdgw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wexhzkap.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rjvwqozy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3skwypgot.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wwfhijvo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3niiuyhwu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kdfaobqs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3emwvhnzi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dvmxiunm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3yxtdksyd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ybxuvwys.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fcfumnyk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3usmsryxk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3akqjfasw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3godpmipp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3drcgjhhl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qlheifyb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bmwqjjyz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kkkekfvk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oukgcixy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cmtykdir.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3efwsaily.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sexjacoj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwkrkif.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ucgmzpzo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ibtrzopc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mzdcikge.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3haqupegg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jlgposit.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tgmvgtdb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mhbhyuir.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ntyrpcwx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3oyfnlxjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gcnqfzbs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gkscimxc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pykomsbd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3widyoipy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lroypauy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zuixuopi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uueybjmo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ztkeuxrk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wkmijfir.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rytptrsj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gynftnsf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zjsmfexy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3erlfwewb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3czicnldp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ahakjviy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gxaleeny.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rxgqhcvb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3eqmxyinu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ilumtzlr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vywnmyxz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mjwwilhe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yknjhbbt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3snbrxdgw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hfnixnge.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cbkurelf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qrkdfrgi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3osxhnmhj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3reyyjdsf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ewaamyyb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yyijsxlw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rudpebeg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pwmdxuyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zjzvnlgm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3umbeqxmm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tpzmxsog.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vcmklwmd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kulvbbyw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hnmknndx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uqsdnjaj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3asbseftc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qwjemhmz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvvheciz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ceoosbiq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rxtuyyem.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3osgzpxcy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xcqjgbry.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3njrrmwic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3enpfgmeu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ayklsszx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ssyozpja.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ylqqnhfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qssjhewr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wnfvlszs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wiuyaayx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hdrhbnsk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mnqozmvj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3agfvrbgs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tolaudbh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpbwezxb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgiopdce.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ohqqcfjt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vxzerdqz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ecsqjpwo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lmeeynbd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cdsuryfn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3iukbbotx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mpfnyuhj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3weyhoysd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ypvornna.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ceunrajf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qdwsmxqz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3elfowklc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ocsyiovj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tczproia.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ugpfumzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbsobrvo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bstqmlfd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3utmmwpit.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bvaowgbx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3izvtiggd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3keulxzqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3frzhwsph.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ziueyujs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oqmpjire.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vyvhtkxg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3gvbcwmuz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kainwtdy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bxzorapo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fmzftldy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3iuqkborw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3agraaxrq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpizlxw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nmsqawjs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jcdyrkll.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cstnwxok.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xvweiwzc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3knywzflc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3oyybkafl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ggmxqmzy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ddjxpfzp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dkkdlbyh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lrkosrgq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhepsolx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3encrgwzd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ozsbbglf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yvstgfdo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pqnmwxgj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sqomkbeg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dygbmzqp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3gknjzbzt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kxtemgpy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rmtglhrh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3exrwnilk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wukgvyud.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hkvjmhdf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iylqbhbe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmeqzwcu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3glzoxnnt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fuwoxxel.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3txukytoa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ilrdkofj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ovhbndqv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3finxpfoq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3saiarxix.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3daxuvqcr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hncepzyt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zklbsvgd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jziohakd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xacntbxu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xpkjayrp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hnajejvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uyfmmkci.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ztjivhdj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3upsjhbfw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ijjtlsdf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aktlfget.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ldtsemct.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rskaefwm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hpldsmvq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mzetxrbm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3frwkynxc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sevvvcwn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wsrntwsr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3auapvqjn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlvgbkru.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmmbttc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ntwiziss.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ibxhmkmu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3awlsdwjs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iidmojcx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfhyxmj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tzecxpfr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nywmzays.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pcvquhzd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvnvsbgp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uwgmmbdp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3saiimguk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3enxicxmu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvwybrh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rxiyknhl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bpsbhnws.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qkbciwjm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3spaiwdtl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xizfhcgo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gtytzvji.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3yhxizknr.html


<!-- 参考信息 -->