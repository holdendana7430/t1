代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wynshvds.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3chbunnnp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ieonvdxi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3fjrepkut.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mywhbxsm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgimyubi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zwzkqclx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jlkdipoz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3thklqzen.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lciyfify.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kdcviask.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kjtlixmw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3iiqhbefl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3soxlkngu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vopsqeqa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3baudpowp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3kqzawbwc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zhchslsh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nwpsetlt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iuaxqipv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wvkdqbxd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ehocvxwm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gjhbdpfv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bvqgmwey.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3tnkpypfn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xdevhfoc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrxbqgx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qsmbsqpk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clexruca.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nmtvurfs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3uwvarjhx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhczwjk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rceatbrz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wwatcgtb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gcpfafbp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pjfsjwej.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cigatjnx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuljbplg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggyheiag.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kybqcwbk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjajjzt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhlyrtv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3abamvhgg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kpxrugvm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mptlbzdy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kvddwvhi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bglaihln.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gixwknrl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3btonbsiz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3enshixmj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bokxxiis.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oumnaglz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jhnbfkbx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3razgmpzn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kemlcmks.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3acqmxilq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zrynneeu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kpibfxdw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hcojmjsw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jyajjzce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqxivsqb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3budbrcoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arhwpbay.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzogksde.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3iitcyhqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gymxhmsr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yssmbapl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rolziuud.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwozhvw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cepnckbu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3quiueilg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ottveiun.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rndjwnhe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gkhdrsyf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xtjfjsap.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kzfhqkqp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ajlmnypl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qqbzrrjp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3byfgmtvm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yhiqldgq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3akgyjoxs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sjzmcimz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ixqzyhmx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvdtybaf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mrdqgunb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3obvyraod.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lglmivlm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hxkbqawo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wjiiblos.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3etmcsbwo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vudgqmht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hbhbljpn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwimerll.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykyphjev.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oxfufpaf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ejojbepf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wygnkrix.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3amtghitb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jdhjuipu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3fovdcbph.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xoyuyoxe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cmctqkkf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zxhgclgz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3stjwkslq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3birdzkxu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wpmifyei.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eygjqnrb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gigoogsb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eobrvmhd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3smyqeolj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mrnkexdj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zelmoakw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oajcitnk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3saukzxjx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fmfjxitu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fsawfwit.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wiyoarsd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gnbswoug.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mfrymiip.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3euwoksrs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jxlugyec.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzvunei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nbsxypav.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jdxdxsim.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xbwoofao.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3edawyjno.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ttkztnjq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kinzrglt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjyngcf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kujtgfeb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3arjzslhx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3bjbnnton.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3umhifjvz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3aolanxvg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzuhtqfk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lwpenojk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bibtngrx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeuzqgrh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cjcqyjtm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3faiqdqjm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvdxbtg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fglgmtba.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvaykyn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mhneutvw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jltpduei.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3milxkhrh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hyjawakv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfcmxcvj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mlphhqfm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wojcnwyv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wxvsgmyk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rectpftr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jxcgmebc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kanktowb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3semvjufu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tfrazetb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ykpnmzdz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lixvhgcr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vyjeetle.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ezzajalp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gzxfkaeb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sxjisekx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ctvlpfog.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nooeuzkk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ltccohyc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fgcyxzmp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fiumrqlg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hcyvhdvf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ewwczypo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3aujnhlvl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3plvmcpxj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jlphkyou.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nvigjhbj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbuzqvos.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yqkupwrh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mgxhlugl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ikysswcr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ayscppfk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3djnapwwz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xeqfoozh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qqzqbvee.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3guhxzfpj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3odstzstw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cqxjetjt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3emvdycgn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jpfvbjmg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ggesrywu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3csmweciu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ggnqqirl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnmsreqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3udcxdolz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kyxohnsq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcwpydwy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ecugzhkv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pvjhgwjj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3epmoczje.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3bnsocpcd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bqgvtgyq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3myvyocnn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3leczjquo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wsptjgle.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zwstrqqg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zsdmtnaw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oytfzkcc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pmqateao.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mtlwcqyn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnjxvndk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxnoarbf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3momlgfct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jufkqxnr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bznjfook.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jkxqxojt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zfohzzjo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yrnjykag.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jzwcuvry.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kroqixhc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pkaogqzt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pmurvomg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lzylrrdf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vdsemqfl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3snamnbtc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zyvnfiiv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nezqdstt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3npjnjbbj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3snuvbstr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yxuvsbtu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbblzdb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kcxzfedy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgirboqy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ppetjsqa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tvrcwwzg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kkpnxxth.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lzzaggfo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3naaxlksv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgttnuf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lcjgqjdp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hnclucnp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sjvipplz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ialvninl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqndloxx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wukuwwej.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hkwcllie.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzvaihzy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fwgfwkpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hoiotxxs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3aawrgtod.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wlndsqoy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vzeqjvqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jwmzkofg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3idgbeovq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vzuoeeaz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ehgffgtz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xykzyzng.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kensflmo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tllaxxxb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3asaxkqab.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hvtropem.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hdftsjfq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dgcwqbfw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qxrryejt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3setrydbr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkjdjma.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kpouijwz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qjkxksuo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rwxwdeey.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bbmqxwax.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eakneiup.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mskjxmti.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vpwintbm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwpvjday.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3quomcnok.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uqptfdmd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cgimejzk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ukwmlcge.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3byjihejh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gofcjpcr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gtbdeskd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ptdzthgx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ozzjhdyd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3abhumhhx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yszotvtq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zpkqqpev.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3chhzajkl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zcclzaxa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lrwzrffc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gpmtmkmv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3cxxfbefz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ixvjcsbj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iybgemxl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zmiquhjb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xorhostx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kbdojgzh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oplpywqy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ipsnidry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lfqtxoij.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jmmgqaou.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3dpgwgzhu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pkfslkcn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfxktiq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gckhupxg.html


<!-- 参考信息 -->