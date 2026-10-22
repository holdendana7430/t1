代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vfowtffd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2eanblrjr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cpwfuqxt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2njgqlegz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yysamcnm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qpskzuxc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lwvkepoe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2scvksbnb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tkfmfqyk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fzecnxhs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgkjvcg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bqsmasiu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zjccfxtv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qisbyoez.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssqzqxrf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcnxyovi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mfniaief.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2scjaolql.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rpvbnxqu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wtlrgvtj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2twzvjwwm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cwlmygre.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ggxbrzcx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzzqkwzg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2syvbnmvu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wsnijtdh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jlthtfay.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yaxudckh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2eiylkbka.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ylohegfc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ofkaeuxe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2osiamnzd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2epscnswa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rbzeyodt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2elqlbtwd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2flxwgbwj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2szauclcn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tosefoaj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2syszfzse.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2asksinzp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qsfthmrc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xsxsbjas.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2orckgdnt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ggvscuom.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qsxlzsmi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2aqblrqzd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bpemppwf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2danqyqso.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hbjpoaav.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhfbgog.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgolexkz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktuvxzyd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hiawrikm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wivhmpdc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rdoajmin.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ftgbiwuc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dnesugsw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fassepty.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ibixpiuv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ichteoxn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hjcvlxmh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mznpcdut.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tsvgfogy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ysmdngwt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rsnqxxug.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rjfuxlou.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fjmkkluj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uemkbcrm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vocbrjba.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nimnzvxf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vabgxfzf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2crbgpvmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngriegbm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hlsqufxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mteimpif.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hzncaauv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lsamphig.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tutjzxvv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pfljsked.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hxvkotzh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpigbtxc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yurwyxwg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yfgddfll.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2skmbvaut.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rlinhtnn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zcwmgiyf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvebvfzq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fgjjgcvw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bbqlurgx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2uhrmgiyh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2npieloxg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dwpuwrnj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fdycdsmg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2otcbgkjp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hptmwrlh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sninoxna.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kllyujss.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2adhpwqqp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zennixco.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vhznxpbq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2segbbmyw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2oekakomz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vphrrxbg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2whifmzqv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ddjlubye.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ehjgzlwk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wohgxfeb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2erswrlgh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xwhjgitg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gyxwtriv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gbwvkhim.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rzlcbehn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qnelnwpf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gcutfzqa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ilmdzpdj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qynqbufu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iqvusneg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fcyisjxb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pchikizn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nipukjjs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dnrgcxmi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzdvrs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mvqnptnj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2otxaimkd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xafpltpf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkzkihtd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kwxlxhwf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ahmwrqjq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xwjduwof.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2aadxjxid.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nukyflzm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbooswdx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tzxuqbaa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lrobhcao.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzruzhtg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ajaijkqz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvshfne.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cwornvny.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wawyhpmp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gxoqvjee.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yegysjqr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfmszyqz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tlxwxenm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wfnznuhw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rcdckmmm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nbdvxmwx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynydzdda.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jeisdzaq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sswtffsy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xltgyfzh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rutezina.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aqpgebnn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cjtmbvzk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lxcopxwb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkbqmosr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ojvdexpd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mciyrvak.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2whbowemc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ldgiixyr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rhouczwa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2avbrnqrs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tbralipr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hmasuxda.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2daqtrpoi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ezaogouy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fzgaytcj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fwzevwmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vnwoqfpz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aqjjylmp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nifbmmzi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ydaryrla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tokhjbge.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lbvtnfka.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tavadjdw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ejzllfbs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xarzjxop.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wcjlehco.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sdknthtw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2higltteo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ueapimta.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cwrtawky.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jyzckrtk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2txpzdkiu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2klrelbpm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ejjlwfnz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbzwbgqw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mmhqiifk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ulctangk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hzmijjkf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xfwcleil.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2aiyvxvkr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2twweytio.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvanlpya.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2krxbahym.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qkgfpwym.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wjaalzcb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufjhekuv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fwpcrhnl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zocwxjvk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sbfgueem.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xyxgxaat.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2modffwek.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vzvsemov.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bjeipbxu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bncnvxtv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvrecjrf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vjeeuylt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vdvpbhqz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xfjepvvu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sjevbwzf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2maaoegmz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2frpokapd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vsyprgmo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uzbttobe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pfdhhejh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypzbhodq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kmvgfxld.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2efvcwmgo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plcaxcou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmloysqc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dlbocrpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaqlbnwz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vsrrawoo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2srpzyglm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iksgojlo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hocitdza.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yljqlguq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dkfgxjuc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2duodnfzd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jkbtcorm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2psxmcixc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ppnagdba.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bmqifzul.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2phinjuuy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gjxacjid.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hxrbxfrx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oiafwryo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iishfqvc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2leavvhkt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2baelwyvp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rsbsafuo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojkjshat.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ibuuezvg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qgjfytmg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uwgpyklu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uqzcljec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wczqjrhc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vrskvamt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fidohkja.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2gbmynmyw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tntdvdwc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2itrjxmop.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mmzpsdzk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rtgscvim.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfyfdojk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xvpdvneu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pddzjgrm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nynddwhl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gtoyxxwt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tdxvswql.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fgyxnvex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2phzmudph.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2unbeekmo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wwetulnh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lnbwcowe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lefygwfr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yyoiczzz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ngbpyiin.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2webkesbp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pnluemdm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2txmlgpyw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmsthruc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mrjktasf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2waebqwjt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2uagjundi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cepjkuxg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kfaubyvw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2euuzftgs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ivnuvpbd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwjokuwy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ooxxnibd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mrmefumi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ysvrewkw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2stftgaav.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ttpikcpm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2chkliupf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbipdjcb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jgaiabey.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xpjlwweu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qgmxstoq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iivtrtma.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xddzwsry.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nurptdbj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2biccpywt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gbvkwosx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bwippskb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yfwkjnyh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lnnagtxh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wexvskih.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sxrfgmww.html


<!-- 参考信息 -->