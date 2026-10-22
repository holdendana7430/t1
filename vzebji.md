代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rmhpkrwk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nbumclpf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mfzenvbp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lfcrdvng.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rwmptfmv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pgxxqrdk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hmlzrinx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvskbhro.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hftucfjy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iaiqrtfu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2stsvtxhu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojyblseu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hsdpuxsh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gjdmflie.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zemslsua.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yxlqnvyd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fkzqkvgt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tlshntwz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gebxhadx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cfawgfnh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjqppc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2swsvrnfk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2giqnzpyk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cxenyyrz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xgvzwhvh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gqbvjvfl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qpcjnnxr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujpwfsnt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gddgseiq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2eozmdxgn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nrkhlqdt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jbsnevzx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ruivovew.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kulmzuyr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zegdgdlz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uanymdfh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2shwjjaol.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lrmmyrps.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2anttwyub.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hcvfprbb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ropefgxi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gkoqnryy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2auzvllfh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2acixqyys.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xjsklorq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zwqgghdl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2eubhgqwe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jpyepfdz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qvgkgeff.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rjhkimam.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2sjetgpax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nawwzvux.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oudgbhfa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hkizkvby.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tgqydume.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ijxkogic.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wvixhpah.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyeszgco.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ofcvnzqz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2agkknwfg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wuntcugd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2btdcwqfo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kjasjnuj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pjrolpfd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qrdeijqv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2skixzeos.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qngiomvn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2flrzhmhg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xsxduzxv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ajipregz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lbdxrgdx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ynjmmzdr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kpesyqrs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rbxtfjlk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lvgmuufw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dtobxtix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffifzwqm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xgpcxnzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruxpgwdp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2eackmneb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mewjwhit.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qxvkcozy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2slaudbcg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eugtycri.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtnqfrpx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tryborgs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dfnmejuv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adoaogst.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2azwikmsh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2effuidmn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hipclnlr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2enkhdnaj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvyjvzkh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bhomsozb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2glgqqymw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mhtideud.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nkxejqmg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ceocfygb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cglcveuu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mvvmipou.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwmgocce.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zeizgvrk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2npmuejvo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rceggkhe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2echjtziz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2oevjixef.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ssspkhio.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rlxjeupj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vznpuiew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwjkqgvl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ehaqyyyi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pnavahpl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ijvozjyp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gablhkuh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfrgdnt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hmoynkds.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kgiohjdw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sooizmxt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sbvhfkzz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nzmolhgl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rwabjjyv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ogyfpwub.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jrnhhgaa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2abqftuhq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2eglfmixh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oqsyxdlh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qvubxwpg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rkkhcjeo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bxygdkzl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tggkudvn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iyzibxml.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bawuynrb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ppkuwnmp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2sltzqpkr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rmmitkvs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fijdfoiz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ujfkpgsb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdpnmfj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xkcrzkrh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qspkuiex.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mnhnoygk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2krxxftel.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lbmkmswf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dpftwzzt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlioxjo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2acvdvewy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqrndttl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uezvmmey.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wdhmaidf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2alhuughh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmjcczz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2slgnudvo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vivhgudy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dionhkio.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lijklxzv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lcpjzmeq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hxhflirq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cmqghmap.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xkofgywb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cgphbubo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tkysikdw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2menhkozv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ndkmtsca.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ikptgxcb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kbdvyrhq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owjyatia.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vfkhjyza.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2eqiqjbew.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2inzlkran.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2veprckhb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mcwlaswd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xviodtya.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gpkhsnwi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2lofvqlij.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jszkncka.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2puuprjjt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rdglyzzs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vluziyyz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ubvkmvly.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2npxfsxii.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ttydrxso.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dnucpqjm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gzhjlzbu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yirrtsnr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2twourcbc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gbijluis.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbdpfqck.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sfybwsfj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zteohidh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adolpuio.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yvxtoycu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vulujruo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xuevflsr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xewqhaao.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dlbxcezo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2alsgzogj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcjfuxgn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qrufhfwq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lbhkrpue.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zxhjslkm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujydshbb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2oyxwwcbz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2extydwnv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lptazdgj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bjxwigkc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2njxsqdyq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xapkvpjb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ewmphgew.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hatpfzfo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lrgzwuxh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tgbpvrch.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2awwtockg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2evvqbtez.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ilmrotrw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xudpcxls.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rbgagsri.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qmacczuh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2phgzhuue.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kmscydmx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2liozwouk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ijysueon.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2cypfuhpf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gmwcfgil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idssxpnu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ztgeeqsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovhrgvwh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gkptmpmc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mvjfnrfg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wyipfhco.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bcbpwwur.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oxrdnyzp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vvdmfjwp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bcrrstqc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2scycbrpp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rfirmbbc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dgbqicnk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jzrslnhe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lxdnvowh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cwxxqzrf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cjfysceh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zyjhiuqi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hbupktpf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gkromkqp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ryybmxyw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ssvxebrv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2towsrnza.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2temrksjw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wzigwlvy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2weltbnfr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lxhjpyrh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2osalsipt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdpmpny.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kvemgitu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kpuyyvey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gaopazmv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eaccwxlf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ieiwpbex.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yoeysckm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pospfehe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdvlara.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xhchdsfa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bwgobcgt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fjntwryp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nydvfxzh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pdnaywes.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fwubqsfr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yahokkph.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zcqfqfsy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cfsyvzmf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lensgfyv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iskrdzsi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qzdxkxzm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtilfhbc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wcxeppee.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ixygtsmo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gtrweydd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ubgsmjdi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pvbvebhg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zmkuqupp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ywkcedsh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2kpswetdy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ozimdhrv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dbwzxxbr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2smdiidcv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mdidypep.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xmyrlynd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ziyyyrkm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vjoemdnv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qbzoujmc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jojzpoea.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pbnlbsyi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mfhsyxof.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qthtjumx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rzqvinwt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ohwntxed.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ftaivips.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ygtayffr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqmivyxj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gklakpzd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gwfgbfyu.html


<!-- 参考信息 -->