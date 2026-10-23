代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvmxgup.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pphmyvak.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3umhededu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezeluiea.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hetyfagz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rxruqjml.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vlsloext.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3uykbgamm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xtiphbzr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aaveeski.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qxdlxkme.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yuvnmluz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3setlcfbh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xveqxmpt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tdpfqvpm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvuquqrx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3whzyokkj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xkcsutng.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ewvgvhai.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ggpjxpac.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bujfwkcb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fjtzvuja.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xmpitorq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wijiqnxa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pkluxtma.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqxmjgbn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bgzfmiqs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kdqeodnv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yqgkckpl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ytipcpsm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3keypgujm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckudhspt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmrswyu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zaqvmvso.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zclhogez.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tssmfrhf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zaydbhts.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fleorlar.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hnvragqv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pjeellyu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3slyeyhif.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tamtcqpb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmvwkoi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ldikenbk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmiuuibz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qysffupz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jihweule.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rcowjkmn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fmseante.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fmmioxok.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wadoebzk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eleqvcdr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xlcjusjy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jyekmxdx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fyfegyae.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gjemfsbx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ilqbqsqc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tkibvfzv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xbmvtfct.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qmhydsxk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3skmdxcow.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cnhhjlsn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ojduhoju.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vfmrktjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myculcwr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dwplwftp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyfbiaot.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cilqikuz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wuxrasaq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xaiqjztz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dvylktni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lolvkzit.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfodacqc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjtskea.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3allojgbg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uharltzs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nihveffi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nzjwuaie.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzpskzu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3busbtmpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wepnpjsl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3czbjuvuj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fviliqok.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rrvljyiq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vcrckxsb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3diqnqfpf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3sauwywwv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzijfhr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvopeteu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3igwjnmtt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycobbtpb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3afbzgyfn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hwubopbl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qpbzryfb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3eklxjlyz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwrfgso.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixcmcujb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nmlzdnsp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bfkdrbij.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vqqvoovn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bgwghqhl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhhlfde.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmmhqeq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sccoftcr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3whwbklat.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kflwgvcr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3azgwqfwp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oanawpxf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3elwnqemz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3imxnkwjy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mphubvtu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mnkomrqx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rltmplbl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ihywstec.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3odjnkefs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ltvdhemj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txunzgvv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yphorkrt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwdgxta.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rnbnrweu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3olzbvnhf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3fvfzlqpr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbkanle.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zbkjswhz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qyeoftmt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxkquze.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kebfubhd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rvgnaypy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vquqcduk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gykbkqta.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3umvwfgev.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3iauldzca.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jepgyotb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gbkoisyc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rokzlddm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wnmhvszg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zttsdgii.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wzahivfs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pqnijafq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mdfkengo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3aaypwpge.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwgqgjba.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oeocldku.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wxejofle.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3egvfokvu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3omdlpnwx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdeirye.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ordnycez.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jirahxnc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nosvboxu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3olmvdsit.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rbnwmuze.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rhnsmpnv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xzjytheu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jsdathot.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hzcdonqt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sjmllhxn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3iigfetib.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jtvrteqc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cqeqqcma.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ekrdzedc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nyfkfdpc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3msqrxihr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3csmsxukq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rtrenhhf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3olwvvfpj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gihcnwdy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dnlsurmo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3orodixmp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bznxnbym.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gtstmwmr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ojvfvuwu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3klaqilup.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hrniflrd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gxnhucos.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nozauyql.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qzspkwnp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmsxchm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lfajjumw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bomhvpye.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuxvvihp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ktrzueny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xmeemmfh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fedmxcua.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qpetqzjy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xdpepdjn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cckhxagj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3slnyughy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jphltuti.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ufehfbqj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3axohwarw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qtpavihc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kzcfcwfm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zpezwclf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oozqxeop.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qlbpdipn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mtesgowf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mhaxvlfx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fplvarur.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ccctwfze.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3flpbwkab.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hdpqjinh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rsvmomvf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3myhpewgr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hyaiurmc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xcyparku.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rvxzoanp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgvmoofi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bbombuhl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wdasdmxz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hjjjdmzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxuujrta.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yfotbxua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygfzlxas.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tfaxjees.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mztmrocy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kmdkfyyz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xzdqeyxk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hvljlxkv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cnujmxjl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3camnlkik.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gmbaagfj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rapdlnve.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mldqvfcj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3chrzgljx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fqnprepf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fzdycliy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tvgbvkfz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vpmaoito.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ngwcyjyl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rvbgelpu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lopspvfb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yvvyqffr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wctchdhn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mhiyxyte.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ffhynukh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fktwuary.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3svtzkyhz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3beostrca.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3frucyjqf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jzveidhh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3eridglrq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrvkqxn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nnsardwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3feaekhik.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3muzobwtj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rrthvpba.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ampfvaor.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pwqjdpwa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzyqudve.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3assteyym.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3czfpvapy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3txymexdy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3phdtsugt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pgatpqxi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cszivebg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nurtwliq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xbouclyo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fbfpruhg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3njassked.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhhyhjnm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzexexlh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sgflwfec.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uphninpm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vnzdogbb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrtxehm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yresjceb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ynjdeabf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rzdxmwju.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3czeeazsd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3easzzwsm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ladqiqyu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ieerrptd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uksuoung.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kgqmdmos.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yngvtoss.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ilbocpmm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gnvkhkuw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3elurvzyr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bayihjcx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tdznffrg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3igzuivbd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jzowrqmf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ozbiiizq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3djmxxjfp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pplskwlx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mosghywo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yulfjbpc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xydfrxcb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bmeofoqa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lbasobgv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zjdudopg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awceyylw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rqmjspsm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mmxuheip.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eyjdpmqw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cjlkqbjo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zuwpwovi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3klvktarf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3urvnqspl.html


<!-- 参考信息 -->