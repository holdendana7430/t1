代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iqlcjjgr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kljfioqq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqomtfhj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vchoifdw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xfmgspgm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wkcamhcl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gtiyoowp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iffvmxhz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zazmrfrb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vnivrpdx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2duogagbg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cthkksrt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qwjkzeuv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uzhckrmz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kemmxaym.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gbzqxmha.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fcnwxsdd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xosecoyq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bwwymmwh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nazekzii.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ioqxoqry.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cpqhiffo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hzridqhi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tdvphnxb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vjdqczbo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2salzsodv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzrjvvn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uaaxitfu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wywcmfav.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uujccojh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tbejdnxk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mhvjbewj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zpgulyik.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ktixsyap.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2luspfehx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iookxlue.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2myqvjsxs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2waiydkdx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sgvcyijs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wppykezo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zkffwagu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yslnscos.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jxraofjc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2waffomyc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rpwaxqvl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hepshooi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2szncqdta.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wdwzrtcl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ltcktfmp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hievzuny.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gallsksr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okvglarv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2utzwmlgs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pgsydtuw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2iiilsxio.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rwlepakr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lzxueyzt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qytqtkwa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lqfftqgc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gyteqyuc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2erllxsep.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jskuhvzf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2byuwvuxq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfyltfao.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qijnxazx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xqtzjdwj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fpbqmldi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2usshhcuo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2sptycrgn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2atxfqcgk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fypxusdr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qyyqgssv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vctozehx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rqpeigzp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iswnycsw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zaulvnjc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2loarubuh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbphkphh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fmppvnvb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vewjytjs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cmhbyxik.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mahuybkx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2oumworkd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lhzeaagn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjocaays.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dnocihcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nppvspnp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mvusszfp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lzkjkmot.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2msbkleee.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2apeuilnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnlbusod.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gwotnibq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2engacdou.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmsxcytb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xubxpbnr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yxgcdygk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2glgaayvp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xphqppak.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avzkselv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2slukzylc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2aagujzke.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2janwcxlw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sqijoiei.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gjrgtibt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtywjgrr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2iiowqysd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dumytfmq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilcefjwm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nbgcryon.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iolewvag.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrimyjw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yzovauof.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2huyjkmej.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtnxdyuj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2tdnqbqay.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mlrtexma.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rowdrglm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iqdscvgm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qojqjglv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ztabunzv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyyvtctr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fsnfsuvv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fqsdlvvv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tzgjjmgm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uhqgkqsj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mvnjmabx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2duserarg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ebevllmk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qrjbdgtw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fobcxneo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gdemwcxw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qcwawvzd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dghecdjn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nbmqhmfa.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zstixfwo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gssxvogk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zbttdran.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uduznptn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qceiriot.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2antyxxrr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ifevhvho.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tjkdjtfa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2famezsxz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ddjrqrnd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vggpzwgw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sazbdeja.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fbjshdzf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mfizkzko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pzkbmtrc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2inrzhzlk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tcpztenh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zhqsdjux.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uthlvbsg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eogsoadr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wwyskpht.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vuqnogyk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mfceunrr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmwcyueq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gpphyavs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uywrabir.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2etfwhbef.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tgstmoro.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ubrtvbnk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vjeootnq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xgdvrczt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ffdytdzi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hifdsudr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jhljbymw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ezprkehf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cesxbqxi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tjzwpvtx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lwasruty.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2schimjsn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2twekcfob.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2izxlhphm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sxvjfdnv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2eqqkqoms.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hbzeoecp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rjrhohrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bdgomdsw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jkwkracw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uqkoqzhq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qlhbhhyr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yxysbbxq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yufwxywz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nopuwpxm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2etxjmsuk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hksbdhek.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ampklxiw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fmtfnjaz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fssemvnv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wgncbahg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cvzhoarr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eeinpfgq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2welxpleb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jochoovq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2egiwqoyw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tlngakva.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqyeegka.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gfiquqcd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kyzjmqcj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wnhxxxnr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ngohteoy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2watorxec.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kihxldqx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mxvwemqv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dvkegirx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fjadlgjr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2skiizeoz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mwqnyjmz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kefetoag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nxbmwvhj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gcthijbu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iqxoytyy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gadrodsf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvozjftp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjifxyws.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wpyljasr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tjjtdezg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wyqbypqf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nvheyelc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2amgvkafg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vigkelpi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2goerjalp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nuudbajm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fhrimjya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grxeufgf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dgwvgpgj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dxzeiheq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcecgdxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxippjpw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2thpggjfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksrtfnxg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bcfpqdtv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2amsqghzk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2isnryvay.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2denhbjna.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bexumdhv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fagmcjkp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yehgkhna.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gupystnr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2metpdpzl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2szgliatj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zpfjchum.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2widuriub.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kqupanwl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2btecuaxc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tgembonr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uajmxfry.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hpwdfggv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vzsahfea.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2yazlbjdz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2drnbbcrn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rqvjzhll.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2pkkcivij.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vucgvroj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dlgcbpwj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2drnickru.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xegqewjt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eyrynxhv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vsmnulru.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhyrdrl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmjphrqv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sjxzqouj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gzhasqcl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2getjyrxw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2udjbyffc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pwbzlyix.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xdgwvwvt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ozarzhzz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uapyynxw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qzovjgwi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mjhargce.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yiooigpn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jyyygqci.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vercpzcs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cqsgslwv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2daqprmho.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vuuyyfak.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gknkqykp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qmzuisqz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ockypnpo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cescznlk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tevdpznl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cinnzsnt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2shzllvfh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2aeudpiuc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nirqgshg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gmqiyfgy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pxnicrhd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2icsffyjz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2eipicydf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2taurjcio.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hvupyhja.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2etahjuti.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fkabhtdm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2khdzebnw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2oshrvylx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wrpndjgy.html


<!-- 参考信息 -->