代发 wailian999

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ozdwjsrw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2esmiqbqc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nuczglcc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfutchtz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pjrqygvb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmccqxfm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ruckgmcj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vfkagizl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dtaubbnh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gzreccfd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcgzflv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmsjgupp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uzrrwbgv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wojfypla.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cwkjdbvw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vqhmjtna.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dbadlirt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sntzqlck.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wmduprcf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xksjhahe.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2udbdmpsn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ecjejxyc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldunttgy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nnyansgd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2boeflfzl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mhpgaxqh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bbgfkqgq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2teeyphpi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2igxdtmvl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cryzlluh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljmnlgqm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bumkqfhj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vpsojccv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2iacilrla.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2msurdvuc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aymhxszw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qikpgwjv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2onzbhwwx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2djynavjt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cjuxceiv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yxfpqasf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bbarmpjn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tlynpjaw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2itsvsbyn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lpskifbv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xnqsyjqb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kdmsmdth.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gggthlts.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dhhxctvq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sxnjqgnf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ukibfksk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xxvwaush.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrxwhrj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yinwziii.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ksgtfojv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fyvcuaqe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zjhyatne.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ljztsubl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2csmykeqq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dsdevkdc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gtqcpiik.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djljfvmq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qehzumdr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pcfgxqty.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rupfbtej.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjmmhag.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fbmvobva.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2crcrujne.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ctrsjvjz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2veogpccv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bbmqexqd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wzefegfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odcreooi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xrptgqyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yangxurp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2abtpdxyn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2edetmxzc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrwmskx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nglpssqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2onbqvegy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2edhdmfno.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ecvyeasy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfcruzqp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2atnggzrf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpbfmnnf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lahzgufr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fbioqeej.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okqwkjdv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpshlzql.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ntaspzci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uhqgxgrm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vkouaumj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ighsoxox.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbseyesh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cbmzqifx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jwmjgfwb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2spzvhhij.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gojkhmih.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmkpnlap.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qowmtntv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xzkehqnl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ueqizaoo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zntialbk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2twwddizm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbxyuawu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pzvmmblm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mtmchtqf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2oucggmny.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtmzzsbh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvhilia.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pytbuocb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wgpixgei.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tbkxqebq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hhfjzqrd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2humokxre.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fvybnxvz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bchzhtsm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dswdfzej.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nhdhzppr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vwvajgld.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lyavhphb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kjgmetxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qwdexveg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aqkiilud.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jamtgpih.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gyfqeeij.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdamjhb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fahzsasx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lwsznlkw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cabaowlm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dctqjfjq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cwebdwkm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2exrcachp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkkisco.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2agptylqj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2yhlytdmk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hrgbgbdx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mfmljjmk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2klupjxng.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xaxutrgc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqnkrtol.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vzdnvven.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyopcelc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gnfnbofc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xtmvxkzo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnkhtveg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujwyhtqs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tevxhumn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ybennanf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ggangrci.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hposcntk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jemdksxs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2isqdupbg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hydekkic.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2excewuql.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xwgqztez.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lvtdpbgp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kfmtrtnk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gbgppvfd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lzjlwztz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mfwnfgjs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bzkywdut.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2atswsbua.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2igvjwzmq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ibzjehvy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ntnsivpb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2agilttzs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmpbkg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jmydegej.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rggnypnt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2flxzpsqg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ifsueske.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2eiwmsodt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wjeyytxn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2blhoqumz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yguxxhff.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dwjwcebw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tdyjadzn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iwwqjuhd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2snhgftgw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gqismqrx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2buqcxbvl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2edzmkouh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ntewfobp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bvhomhlk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lywndagj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fywpxesv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2retpdslm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mwdlxqlv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ipwbxeln.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2akqzzxzd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xqgurvmi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tdfnshdb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2uxwlqlnx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2stamgshn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2riawsfzo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwasqexc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mbxgajdq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vjwuogfo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wxyqnofg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2whlgvtsk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yrbzaizr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nxfrsncw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ftsjndqs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2axwdswgz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddnewgms.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vznthqol.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mqirsxmy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mvdrpowj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2idnohrif.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2esowqncl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fxvhulck.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pvqqzwmq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wcssolai.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ngqkvdkb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qgnzixsn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2shukvqyl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbxxqwkj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cbiuqlqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybrbcana.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tosuioqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybexfjre.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xhuwmrdn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cviikcnl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yxcwbyvl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ukmnwhul.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tagmwzmh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kiopcvyd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xetmnisx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lszqwxxw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2uxahtlzf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2axoyaiiu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2oecmrswv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tispomkm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekoznozi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2runecpjw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekrdnuiu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rpemeile.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pyvdunol.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vbupiddg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2isdfenaf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2skmkcioa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2synnxycv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pawhwndq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2enbsihhh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qtrmxoda.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jqrwhcem.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wpceibbn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rsataybh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jivuetdc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2chcctwzy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulctpgtf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kcawsdtb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2njnanpdf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ytwpdbyx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtyfjko.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kijuomvd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2sdgexvnh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywofxoiu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wgjoctxs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mviandgc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ohvdpzby.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uvzcxaot.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2btjfwdjq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2buugwfhi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xawdalib.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yhsaynwl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ecqujgbr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpunuxu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfjsblmc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zxwspomu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uuumrmbh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qzdqqosy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgbmmagi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yislofja.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2zzcsqukd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dwfyyfuo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xpvfqsff.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dypfsgmc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oqskhnnf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pfmelzzy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jpnjcplb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ebitrgio.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eungcjjk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cbkjhodp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2nymctyxu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lgixssnr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dtohyanr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jczuxbkj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2sdbgifcc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpgdcoqn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dgvnmbjl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qunjrnej.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iqbvngsg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2djsqvboq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wjsspvuz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iflhxqbx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2eqcjxdgj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2voznzvfj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dsptrwvh.html


<!-- 参考信息 -->