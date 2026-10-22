代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ctkmremn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tcnfhocc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpyjojhk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zffitixr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mrdpuwkj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bkjwyfgn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mnvlnfei.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yhflasea.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2knlyfpxk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bmzwpvoy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dbbyamem.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2glkobork.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xtakqgsb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dudhcwiz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mujtrtxd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hydkfthm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcdbgga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hciudepq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qkdftlul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rnfkfwkj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaeykarj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2clnjfkkb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnhrain.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewygderg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ttkyvjcg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rdlcfvhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ewxhzxpe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mschijuy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gkqmmupq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jevnyzhb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2iwxfcvtx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jlmqrozo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkoycbjr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2solmgdrw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fbkdwfox.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whqvpirq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mzfizktp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ulbldydz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmeotcs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jnfgeyma.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vbuepisp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ecnzdvav.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2omoqvnab.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2duzxqszu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nbbnfyrw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nwxpjkca.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cptxoadh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aczigeem.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ciforvpw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xeahxntk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2etxdpsnl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2boaugbji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bhqwkffn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gxqkgmfv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tnkexwsu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ioalaowa.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2emtkxxwb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nbozjizj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nrxocvma.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sgepphzy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cochjlhd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sfcxujsu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwhnktd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yhwbfsbn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zexiehzz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qauhczse.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dtkoljev.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wanuhbmz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2poklcwpr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uasaygrl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2caewolxf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eqjoquyv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2prpoeyge.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yvgbooka.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ozbyexhm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2plxdsevp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vrnzlbon.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrnlhok.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jgpmpzgr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cewagglf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qeixoafw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2akbfgnul.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iadfufuu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uwsrxzhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beyufocl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bjlaallj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlsonbod.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2htafhrfa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kbwygvqs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wazdputm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdqakiy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xugiciod.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2thuhnkgk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nqifsdsu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lfrkfjmf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fohhlrwv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfcegllg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hmpmrpfz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2khyswuml.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2euhqqybu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ewhfwlbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cscbgpge.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2focziqmc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2iiayiaid.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ewryecdi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xhemmwqc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vjxsosvm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2infkjkdp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2znoaabqq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oiekpubq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvhacrdy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rpxqzvfv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2omfesrno.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bumjtsmp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qnubfapz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2oobawxms.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kunopjum.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tibgabqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2idotfqyl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2jsgrpxrt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxcpjsgv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqanzrqk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2agxombcs.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vmkgyyev.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cunciqkh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vukhgjgr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ouhdhpsf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yfxsmdms.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2wuvhybzj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gpoiebfv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wsgakluf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zhetavyi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bmvclnkc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2msskmxem.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2diwzmhtc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cwnjwjed.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oiuwcrvx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wijrveop.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bostuuay.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jsxmaxnj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eqtroxqv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hobkhnfv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vcjztbft.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qtobxlop.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2edzmlgql.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxmhrux.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozzzzrtj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nzuiwigm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcpmjra.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jlurhdgz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2afujiuwq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gxnjvrhd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2khtjqayo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iqgjydxg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mmlpsbuk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hgkkvpcu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tagulfjh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrgvvgyy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2utjdanor.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymvewhrq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ismlllxr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fdskdqki.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ohvoeiws.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kcrvnhuq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovcvzstb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gsiwhnhm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnumybac.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ynidilkv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ehsymgks.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cxprdkvl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2illhuyzb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ttlfrehx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vjcoxcle.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2usiiqxwm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rxvxisju.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fdgrwojf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oyjgmjqt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ztyeifpb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2llkbehyq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oezehkbd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kncjzcag.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nisyczti.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ppxtnnaf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sfjithnl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ceybskmf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2feprljqf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vobpjqes.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ymoytlfj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dqdqnjga.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rucdeuyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ohywhmiz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rjhsgsvu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fufflsxe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ohepfiwp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ykugqibz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ieyeoxnd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2torxoqsh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsfolid.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2efawxenl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvupmkhz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ppsvyfdh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cfrmjyiq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2aklhxogw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tajwkfkw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rcrkrjbw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lherxcyi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xgxgujvu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zbuurcgq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsamfegn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pjtkbkhw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ajrojkvt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2idnzhwnp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2khkahcxb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2hkkcmfcr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sqfepdwh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2eosjeput.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tyswbqip.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ynmpcieu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gouqzygc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xogvgmlf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2glaqkyjf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mvsyfibk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yuffozoo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ynhspdzm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hizgcdvv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pyxromaw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gbqvucex.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unummdjf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tqshvkbp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rgrsaxhf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2usnqgixp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfqaoqps.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2upoibfkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzaoetma.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dxpopigt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ddrblvst.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2azuzcyzb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lumwkscs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2losauhde.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wigjogfc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dmfvtwau.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sgzmghmt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2glvzujqf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ytbpamfi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2egegqizi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rgknhfkn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zztjeeno.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ofzwfliv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgftpups.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bjyzqiwh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jqnqofjd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxodlszh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cuuofavt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xiryjmmg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2krnswwap.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jhmnpzig.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2czrzabtm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpvrvnps.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hrykoelw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwvwksml.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sknkjvst.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rcsgslvq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mxyjqzvg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2abrtvfsq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fmwilemb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ehlilbjx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2unkvlokr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sayrulzz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qjcgwktj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fxqclmvb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ygrlrpyi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ifvdxkvf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fyemqsfb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dnwvznzm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cpcxscuc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2esgmpylq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xounwbkc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fkbyywqo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xesmqjwe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2abqiskxy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2arzbhgku.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtxachtp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bejtxmkn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2npgqohxu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uxllkisw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvrgbfy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2prcbltrz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cmxdwonu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ungodgev.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2zcejnjog.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2buplbduv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ethngqjx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dxmqkbch.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2akygdprs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dshzbvfh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2abnvgbwa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2acydvfkt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ztjcparo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pkwerdxc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2sicrxbir.html


<!-- 参考信息 -->