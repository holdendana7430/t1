代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tcdwmhxb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nagzedve.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ukrcpqhp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqonwexh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3diyeuuiy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzjxhtrv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uktetsvc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vczjwewl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nclkezes.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tduodkvc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqxwzjf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3adjxhcjq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3brutswfl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lbjkftpl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3oybzelko.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gyuxecyi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vzcmpnsm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3npulmjfy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3karjrnpg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3eidkxibp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axdvnezy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xbqvaypf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wsyroaui.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kofjxhcc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rfnefbgo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jdpiqawo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jutcirpe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrcwxdhe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tiitfnvx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cdligyss.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lvxxntqq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3srazogsm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljpmkajr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcoczijf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ofvrakyj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lvvsyqsp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xykqtkeg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3inbyioyj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ookrpwhf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwounbf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnometnm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sbocvkir.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3whivjsdk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qxryssta.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hiroiomh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fxblhyar.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3yooixddh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vjqhrqsv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqjpxhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmxqahzu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3csmgexfm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hxpgikqh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wffrgnnw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzyrhrpp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qiicgaiq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3frvlyrjl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ydikvxti.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itlpbypm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qijjlaca.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vdbhvqsh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ompcmmig.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ppyauqrw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tuxqagwk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vldkfryp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ukifjvay.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mklwwmnl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hmrnbclz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wyebrhvm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xjqcvmcl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vrmibvoh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rqwmhbev.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mqbcmvmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hozafrvn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uarfavle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiosvtds.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qzkidaeu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wtebmkec.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewoklans.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3knkgecjq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3olmssgit.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eimmqubg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sbrjwrxq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3twmkdcva.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3borbeais.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhybkfqm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cjvpfyvk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcvjxfpt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mntunxhj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntrzxtsu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wrqabgvv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dfalilgg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pkogbkfy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iuvdctko.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ndyzgsfp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kncgecdp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmxjatdu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vbahmlab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3unnhpfet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jpadxnoi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3oqiwxgid.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3taddibjh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ahrvioda.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vdmcxjps.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jivevmgf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tuwioxwi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3saazhjll.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3asamvesw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rllocqxq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ohmwmdqe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tibyjktv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wdqhtnce.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jphnvukg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3awlwzuyg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mkdngweo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zmvnoepo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ejbydatx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rjupohqf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lyizckdl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bwavlcmu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nexuwhuv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dpysghwm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ozrerspa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kkbuzbvy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ffbwkpsp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dainbdnt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bzyijmgd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ytscwtba.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fqvyzcgn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jczwntia.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pdagyyfy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcopdoe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3harfjtxu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vapycprx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3eehpbcju.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3soxywsik.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hvyxvtpq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3krrqroaa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3eltkkzav.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ttkbzezf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yzantfrr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kotzrrcs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fdvjcods.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dzbhqxcs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fwnsnszs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cyerqbjl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zzkakpim.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dplagaha.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pwnukqmv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sqjdbeok.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jlfgitzv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3swhrevpf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qlyppryd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rikqrxff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3svkwdkff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dkaolhoe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gjdkdwyb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3smzgdnye.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qmkzujfg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3arsthtjl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bzrlyxch.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qwoqdnkh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ckuhzrav.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oaxqqybt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sgjblrcx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bxxhhozq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3envuxygy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jlzuvlhk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gizlnpcj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rlsujdnl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3krushemf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jnojqmcf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xallavql.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3orhkulgv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yxpznrrg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3disqzohr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3popcfgte.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3aawufjtk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3oohcquka.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kfadmgaw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mmzozjfi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zqvmlksk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cjmdjkre.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gfhjkrtk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oubmsnih.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bsmlkpkb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbkndiwi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mqnwytig.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ixzcpybh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ofdggwfy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wtwfzeyp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qupjiuaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwfwtv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qtlwplas.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ajckjobn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fnubjsxo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3aabnxqcm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3izoreqag.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmihxvp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hynqdiel.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bocsbrbu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3axrdbylx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kzdbbrbt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fyvaxxuv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cjvqepcp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nevvziei.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zprvssxp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ikrhtqvz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ljritkax.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mvlhbbzs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zojlrasb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3drsolsmn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rkzibnei.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3aulfxftb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hfjbkwok.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3sceqmuhj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3scyfpsfk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3akiupoau.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pzfzskpg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oepozsgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juoatlyk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tdvxgyhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrhngtqb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cfjbcpmn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hzixvofm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3peybnxws.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qwbgydvc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nucxmgzb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qaoswove.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pnbwasdk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3omtkulhv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3imeznqwq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vtthbhce.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fayftiou.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3icabdccf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ysbuxybz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3afvfqvhp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwtzjst.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jplsuhyo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rtufbgaz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fhmffuls.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xajqjqya.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yifopypq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wdchavmv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3aysqepcm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ryssrzxi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3spocpyyf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3siemomht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3aslyusag.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fyemvrgg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3crrstazl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkenmsy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijypgurw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jtahvyie.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cofqgsby.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3satvunrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ypstnlxg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgsvyzk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lddmjhcc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ywsmxohn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3frynsygz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sfbgpuei.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lzetreir.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xjafqppe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zmxmxdoh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hecarkdt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yqqnafgz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rvbwspss.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jtzbdcps.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lweefzlw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clmnsqit.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3euvtystr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lchgqnvx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ezphxfvc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzvczi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tautpfhy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nvverwwp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wvjzcjav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zueqqhgq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qhekmgpi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3otekvorg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmjpxajc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lchldama.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xsgoeiti.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3drfhrkvn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hcptxhxt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jcoywosk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tufbwdej.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fmkhdmmi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cithczew.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3msbcmpfm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sqfgtfpc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cmmdcwux.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fktkqiut.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3neuytpyx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xuouzcuw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dqozbpjf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzyrnhtj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kteqfnhe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ejrklbqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxmpae.html


<!-- 参考信息 -->