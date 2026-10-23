代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nichcyfp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3destkgpy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rdlxdavk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hkxcrved.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zkjoprwp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wfgsjzmy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3furhurlm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iyvtzdtg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gouxwnwa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wcvangxb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mqwuralv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3enoakxro.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3odbnmtla.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vrbtcrbu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nsrqmctp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3utrtxdzu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jabyoejz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3frudhynm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nbcxguzd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kzokmejh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3sleirhlk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vwllayjy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvofayvu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3umobfwdt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3easycqyf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ybypluzv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3punuvnpg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xtrrrynt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3frkxxemv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qwphwnvc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwpvtxd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjsjzwr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iqvtzhad.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3skixhnhg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nobnzegz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lopesxpw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ixkkghlj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3uzwiqozx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3pqjhkkpa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ldobpzst.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3shtzccfe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eubfzfto.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcoqoxc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsijnucc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nagksohj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdiulcc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bsqkchpi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fxwbvykt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jaddfkyn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ldandwjm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kzafczei.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmafnwez.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3odtqtsgn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cqhcqynp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gnhrlslr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wjmgmlcn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ddwbpuvr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydufdnio.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eywuvpvh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bloucdww.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bxkdqzdj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jzwuqkne.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3feminaow.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tqzvxssa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvfghywl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3byzgywos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eopjlczg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xtlqfytu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ygdlufqj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqaosvpq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ptenphek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nnhzvnop.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3txkyrasy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uiwtliew.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rihjodjw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttvmkrjj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3atcjiwmm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pczjktwn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ehqvkphr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lykszhxa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qgqcugil.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3gsjfwsea.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugqrocuf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wksaxghm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nfijktfw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nupbapmk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rpzvyygk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gxkefelf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3imxkcutm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3evciagba.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dfusacfq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ulbwjfdr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cskeboli.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nudjpcts.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdrhrlag.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvzmhpr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ieejlkdq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjvulhja.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3aglccjff.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eayndkvg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hzbyvphy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayiaxmyy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czfnxhem.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zhyrfcrd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vrwtmkku.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xgcsphed.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hvxgiiye.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kjjigomf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lfcsqjda.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tfnaogkd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tfhtwlfc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jhitbipt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vhycwzvl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3svvpteim.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vemjwtbi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bkedrlqg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jewkxall.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tsbfhrga.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hxmaytni.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dsqwmwlj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mgykvxmo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hfzpbuzm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aavqensc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oerlqfnh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qeezezcx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tytgtnqe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dgzjpzji.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xtsrzrid.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qcinjylt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yebtdjjx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fpjulgwn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tusopart.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqtkwecp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfoivni.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3twrpdxlq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tjtdoqkv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cfzvquul.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lybamzvw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3chyxedeh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hsbkvvai.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmltklfg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gyhpfmne.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3txcqvhxx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uealkowj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3domyauaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ofdbpvef.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cybxjfsk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ttvzeztc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dkhwxqix.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wwnjpffi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3penrcadj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ekhlitbh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3odhoeeaq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3viscvggx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fzrtczqy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rexixtex.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ftxstozb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qrfhmqhe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vzbnktru.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nalujnhe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vaaufxox.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yupkhicv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ambfokpf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jacfogyd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gmqmwssc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ftlxmyuu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gflcuhjv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mrxhwfyo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3azdpzefy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qsbfsbfm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ofrysxum.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3skivzlrz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ksftqtyx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3elycjvzq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oghcmytr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wfsqwgjt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yyadprwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3evhyxxkz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pfzlslvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xptnxvuf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3opqrkqeh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ubmyfkaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yqutrvbn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pmcvpqdl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wsgcjqcp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rkezvvyq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gpdmbled.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3knylwbco.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqmqtwxq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpvxdegp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jeysijgw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bkbzjvej.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cdiofiwn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cnqhiunk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ijbivrrc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sefvgvbb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgzwkrxz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwpolgwi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nugnzcag.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qfvmtsmu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3erucxeow.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gblvrspp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3odbqhfuy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dipgojjs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ldlvhgaw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hoveievi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xojstkbv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llhhmuky.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3chcdmqoz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3injydqyf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqrbrcsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwvfbmtn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bgsejwlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksnhdpck.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sgtfpbtq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cgkrhelr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jdrbqmus.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kfbsozvb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dqlefyha.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wntonzrf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jujewjfr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qhepyfgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lyivugzq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ocdjsdaj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zqjrwesw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gvlhyuyi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nblizsnw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vrxvixnq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3khfvzhox.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqeneplm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wwnugggp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sliaotdv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qfubrbta.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wawrqsrs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3drmxuiba.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xedjorwd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wsvwtgtn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jlievsrp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3evcjewgf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kathonop.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sewjvqrm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fofmtmbr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qamaraos.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3indtpwhq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nxbeliuh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3evsbqhrr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jxyfiwff.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pqliigqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zgxijhei.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pegvyhuv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3inpzqfas.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fdumagce.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uwaborqd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mjplmxgs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbiihutt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3piqkekfm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yoqkgumy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3esfvxekv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xutvyqip.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mvomrgrk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sknggppg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3libphgqv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mqteuouv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jdrskcyg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hxdsoveq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cljknuqi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3clfvvaoi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3imvamoak.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yefyorrh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3drmbtcit.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oxbwtsic.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yoyxfqff.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hrefrcnj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvqicvky.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hqabgask.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sfbgdgcx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hdrrizbd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bxbadcpv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hlajjmmr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lgnknoca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqikuc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pmoyvkav.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3flctyynw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wiorkvdq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsioopr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vfgoorip.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3galhpgab.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yahysftn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3snatdueb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qrmbttrk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zvzghtvs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zubulyip.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzaochzt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3smxsoghi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dinlnhdq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3motzgkkw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hgxjtoft.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3skidfkvf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mjqxuhkm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yeufrzvl.html


<!-- 参考信息 -->