代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xdokxenl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rmiijdgt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqxpcig.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfuecdwb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyxxsbiu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3chopyiat.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrjxotqv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3igvyjhpc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqubjsxo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3byjhpfek.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rqnczfne.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3klreuokf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hddlcsad.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pylfdmab.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vgucpvmr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zlfyyqma.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aacnpbal.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rrsimbew.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pjqudqgc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cojleafo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rgeuecqx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3llzmzmik.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qjpeifjc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3majnvlbt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zedddegg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hsphlgen.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ojrzwrok.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fxksjcwv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ellraeks.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3iafgccfd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hawynbcn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3joyzvbmn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3flemonhp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ddwbffld.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fiovvugr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jpywrkmd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3skplvbyc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ceyvmmtv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rglnzrye.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjwbiwad.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pigvdywm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3toftbhop.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xuedsukz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3iaxjburs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mormrltq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3elghzpkp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hriakhiv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3afhpxrsz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3unebkwcp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xyuspovw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvbmpvp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bnjfinyp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ottqifyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfufnpw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3trmgyocc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mzadgyjq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mvjpjwzp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zvottspo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pholitiq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qciqivtv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kauwjhug.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fwhlzwka.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zaqihxgu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3leukzmxt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rcnbzjzr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3batvegkn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vocpwbhx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nchhitgy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gjdxgikb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dtnafbui.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gqimtftm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pewfnpvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdtyazcv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vkynjxhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gagmrche.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3scdcsjgc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3anbdgwmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uowcrclk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xelgcbsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndiilbgp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wufqsznd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkylskx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3givdomei.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3peujeulb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmqgeowg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3irnxgzrl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3eseqfbqc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3waoibyxc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfymacbj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qppukljt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3npmarxzc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pwueiqnw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pxoazlug.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jfsfgijl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rkmssmum.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jynxuyjg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vtvuvylv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zdbyrgxy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ornrgnwi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3aktqkqbx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jurasmit.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3djoodsbg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tmggnmik.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lyvkdess.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ylfzpbek.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fcrdkkov.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nzzxtmmd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zuqtfuxd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrmdzgkx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aotjjwke.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zuzmronl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rdizqktw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jistdfza.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mvqgnvey.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jhpdzjgn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ofcrcxel.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nhpfjlzz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hjotojsf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lueilmvb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xgzgajnc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jfydnmfx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rcedtghb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3gdhvroue.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ybzlpact.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bhruaatx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3flljpszb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dlncsrwb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cmlecqpc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cfpxmeym.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jixhoafb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zfnxdmjo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3plcaflbp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ngnbjosu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rcjuiegs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kkkjomjn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3oybjouzu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jfbptlsf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3yvxkjfit.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3otceevzn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3givfqhng.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jrllaxxc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aidemukx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mzprtguq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3itwymqvd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jipmxfyu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nbiiayvh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dblsyzqf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bveasdbo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uuwwyucg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqhkoxi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3odabwxvj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ngxvzagb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zdynnzif.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qlssllvd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahovtvbg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ifrtadtv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3muqxgabx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ldedgjzz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3obpfukau.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wmengxhl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ozubsafs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ctitwmyw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rjguwyxi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cthbqlyl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qvfwrjzi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3akfzfhgv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aierhdnd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lhjxhuft.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xgdzpcqj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zwtbdrrs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dlisyvqj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3puuvlaga.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fyqctdah.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3oyimsrag.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vlohflcw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dlkqgolm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dwfifzys.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jqrvcedd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3obstdvxz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xuoiukhy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3iiyvzmyd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ftqaysap.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3etrihnsl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cpikxspm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xyyrqmcp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vsthtlrn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lolncypm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdyozbyg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kddhsiro.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fnnpsxla.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gwbmuvbi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fpdkkkmx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3eognvykh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lkslavcl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3amcepvdc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fgbxpkjp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mawiujas.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkdblxpw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3febvabvf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uvdqtypz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3axqeqkbd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qiobmcpg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tzdmgmby.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xrsatftd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uvyswnjk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmwsewvy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xlybncmx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3icjxpgsm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ykdcmrvv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sbpjhzkq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gilppsyt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pkvpbqap.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ojaudohl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mgskozlp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qxucavci.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veawriqm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cefdycbz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivpuoppv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3oihbwywh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khaeiyrv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wqkoitze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcupyafb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qqjdqjdy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hwrfmjze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3homqbbxf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3premrmgv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rtmsymjd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cmnuqvyd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kupuqlqd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3etmuyvof.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sjktbalh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eznbmalw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gdbtmfkw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3sldezhaq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lxstjtww.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eftfkwhd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mlbacqwf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mazqqmlb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qdotniml.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dddlkbrk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zzqzaeyh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amtmrubb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3smnphcbk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3aaefnjyc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cgoiajgg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgzaljnu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3weectnwc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gjlaidsn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtmolxwh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kxmmowzp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3orvuslzr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wrwulsfa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3benqufdg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3etgtyjfy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ttvzjljs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3oysdeqzq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3guzuaexu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3sscmwtuh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jzdfgzkg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jbhxvxzm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wvswjeos.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nmcauiqu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3inflmqyw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nqqqgjhi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zgtaomoc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qlvwdjxp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mqebeksf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ewwfoeat.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wupdmxui.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evqrwdpt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvlipwlc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ntuibecj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wizbgyva.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsostumo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oxsdoezx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qklckuwc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3igrtlonp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3edbechct.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxduawuk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lqquzmrb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rmdopkjv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3giwmquji.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mnaugwby.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cotmguwb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eyohazdp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3iktidxdy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3prrgeqiw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3axdazgwd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uzaeopdg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wvqqnlnp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mtmsglyv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwnobxa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3utgwjpnk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gufswntm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xkcykiaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sukgzyus.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tcwofhqt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3maxdpfaa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3igpuslwv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3csffshwr.html


<!-- 参考信息 -->