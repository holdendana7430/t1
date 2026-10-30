代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gknzufvxw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gjfjaucse.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gekbqyjdc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gqhzcrafs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gesdyedrw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gonimroxc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gnzthzaqv.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/ggiintzre.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gpzdbwhdy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gszsdwhsm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gmiqjkysg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gapgrvbkt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/ghknmrjpp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/ghxilwpxi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gccybnyzo.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gmzkptobg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gfofmvtnf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gevhidwak.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/grzmfpvsl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gxvtrdjai.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gswqybonz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gzvankidl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gfqomuovu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gjdjvoqmn.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gdjnwbeko.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gmmagvgxw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/ghmfywzzm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gzwtmodqi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gvjpwwobf.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gdsbqpfbo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gngzshrsw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gopthtnof.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gpdznkvhx.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gxcwbaqxx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gcqwcpfip.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/govjzhsad.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/guuwkupbx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gvatmwgeo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkxvekctc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/guemurhwp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/goqydptqm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gqygqpswh.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gpxyiibjb.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gvqdhvebo.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gxltgbmqj.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggyuodkwx.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqhohwyqd.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/grflymiqi.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gjmvcavks.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfscqpjss.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnwkdnylt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/glifdmimu.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/guwqrfcyl.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gppysxfqx.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gnqwxvjre.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gtgxfondk.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gdrbmcjwh.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gnwumveng.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gkbwfwqkz.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gultlkcaj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqvsbeqcj.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gppbrwywm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghtsvhjgm.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gjitgdpam.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gxmmmgjsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gktupgdpj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gehgavooy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/girurotbi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gurnrstsf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gktctoyjx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gdhyyvfqk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gbbpajjbz.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gajmwstlq.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gpvlnpjif.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gugvdxgsh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/glsttekzk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/grwuudmiz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gixkkzwrr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/grivwmbwq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gxipsvvnu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gtxybwbwu.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gfqwmysrh.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gzygzpmdg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gkpnnpffq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gdbrvinkc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/goffwsikl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/ggizvgzou.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gmqrvtxbz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gpomtitpm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gjmbgqoxe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/guvmyqwtw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/grfzzvhss.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gpncrjnjk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gylvmvrmt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gggekjmdn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gbrjauvsz.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gfmhuvpuk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnoodejep.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gcvvjnhkw.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gwiyjuoau.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gelnemmqg.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gmrtnxjhm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gknbycryu.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gxljhkahe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gkgfssort.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gvlqarqxf.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gartozxrx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/givdceddc.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gsmuqqkcn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gqiocsddx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/ghuiazkgs.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxkuhvijn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/goedyigwb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gfwtjimge.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gyneuhcpw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gqoxboqlj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/glqurmilu.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gqtmrryds.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gmobatfbn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gfrmbnrkv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gtnvamrwb.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gosfczvdg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gaucbjixd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/glgsmolup.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gktuiyuib.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gkspzlcsu.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gzyqnhgny.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/grnjzribp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gpvtiipyk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gbkrywrwx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gmzgbnsal.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gnvmnnnqv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gqdvvqzdn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ghofbpkgc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gjjhmspru.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gfqomzjqo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gmpfjjwhc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gggqdawcl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gwyujjsfk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gakdfvmbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gbqcobxts.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gnekrrxyu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqcjagcao.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/ghmpolkap.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gefgumwjh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gffkqrbip.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gekwrnzys.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gqydynymm.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/goynvjeau.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/giaiemodi.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gnhycsqrk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gpiufpajq.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfgfkervg.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gsqsuhhrq.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gtfxmghba.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gfvplrvsq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gqzfqcdrk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gbrivmqdy.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gihvyqqes.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gdxxcgvjo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gygmoasts.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gwntlbjwe.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gmpnvtygh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gymxmcklw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gsicaonll.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gutbyvyez.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gmjdbzvgr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gwfzfgiqv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/guysiwtzm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/grtjjwmgc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/ghkurmnft.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/glehcxuky.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gcjswulnw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gcypexcvf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gtbopuflq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtvjzoler.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gerfypori.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gdoncjguu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gtzlcpdvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/glbauxktq.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gaacorztc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gqlbamfkp.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gafkensqu.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/girnuihuo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gnjjdmmnb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gfeeoystm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gutfeuizi.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gucqxymrq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/grjfkgqcj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gksmwnais.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gthnmmowp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlyzgmc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/grgmwvklg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmcaiqubq.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gfshbfqjt.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/ganmrcsst.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gdveyklgt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gbtlqxxwu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gjuaolzer.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gkyejieoq.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gupupbohd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/geujalmss.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gtmkrgpnb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/goxfrxjew.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gbedsxcow.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gdjnvanwb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gffgnopqw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glbmkolte.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gjabdbwwz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcstunjey.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gyqspvjqo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gmvcdfljo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gyfybtwdd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gwntkmbql.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/grwzvshhz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gywcocsrk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gmfgdaclv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gkgcqdhok.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gihnzparn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gbjzumraf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gloaixrqa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gienkdywg.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glluovylv.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ggxdckipj.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gczgoynrp.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gsegbiizn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/giobymbvu.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/ggpshudos.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gsmudbxly.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gnowtlumn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gdjwifzsd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gfvfscmez.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gcfqwpoxg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdowpjuzg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gnnqtzjtf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gwiemeypd.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gabzgpmwx.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gdoswerpw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gklevcnwk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfqnkpsiw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gnhjingne.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/godbtnpcb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxvimpyak.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmybriy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gwqzmdinr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gwjkcukuo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gvstewsfl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gssfomvpk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/ghgixagdg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ghqhyjfyl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/glsniazsu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gustmtrvn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gsiidjfaj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gozmdvnyf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gojtcibtp.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/glkjsueuw.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqafsezke.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gsqyuzxik.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqdjhjhqq.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/guzwwusli.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gtiajnkxi.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbalvvdbl.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gtksykqvp.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gjlbjbiij.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gmqtvbmja.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gflxwkiqy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzsdctsiq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gitsjgrln.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvobkvnxw.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gecyxoira.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gsdgnjatg.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gchwthmjy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gfhztzmda.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gqlsaruav.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gnljdqxcr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gsupedtgm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gdxctkjtg.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gtiydznkz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gzyvtbzhs.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gphpltzum.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/geyxqmeji.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzqaqqfzf.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/geeufvvtn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gdqzhxxrr.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gihppxojo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/ghstzjsvl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gmxwdwksh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gttflcewu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gtpkhjhtp.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gptjxdfdu.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gtfgjbhcv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gmrtdxpdr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gbhqyjbvp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gabaufhaq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqvngmvse.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gjkwezxss.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gvjxqknni.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/ghhizyapu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gocqrpjwf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gzzlipllt.sHtML


<!-- 参考信息 -->