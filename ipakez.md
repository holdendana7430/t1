代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jtgwgjvt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nxmecuyx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2twymrvhp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2knrfaway.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lwutluwj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2onkunjwo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bzilsguv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dnuiblvj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2srwygggo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2teiphwmu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hxjjrcgq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fgthljfj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukupezkk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rlngicja.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjnmwib.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fmhlhbhd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdrdfppc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nvkcfsuq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ebqjjyyu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gusgovpe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2elzbduby.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ejpdkyim.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rtgpghub.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tecdxqhu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uzdoqskk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjfaidih.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2siufccwd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cozzsidc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pcwbgphb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lalfqtum.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ziqwrhlb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lrlekrnw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oqglitfw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ozsyfypx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2onoselcy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmqzozqd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wybxppqb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wnrlbxcw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2udyuppmk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rnrkgkpb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xqthaxfe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ugsycpyt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mlobpyhd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nvfdmvdd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gwqvcsvn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pwzxhbgr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjgalov.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fzegfeaf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rhnhgqjc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ieaskspv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tuysorsb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2uvelvvae.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mkmjqqov.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ixjycvgd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cetadhyb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2regqpibv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdnooqrb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pdvvsoyj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pisbzjjn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhphlfad.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2famvgngy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgraqwyb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mojwpbuq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lqfysfrf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ocgbiymt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qypqtpfo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ebviandk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cqfenzpl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agahogsv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qrgkveqg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2buxazfbi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bzlbnfcf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nsoxqiyz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwhxubs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2skqjqdua.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2myghrytq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fhajrcpc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jcgtsotn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jgoookzh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aojctpnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpgkgpbu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ojqiyvjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxgqjpsm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmmuypfz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jxgyqopi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2httxbiar.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocwiltnm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qxhvhukc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bbmwejnz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ejeeowlg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wafhcshy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghbjkcpt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nltanejj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mcqgjzil.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwrqnifg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2twnxyioi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2guapzopj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bucsfcci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2scpltkkx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cjmbcxga.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vndgwayz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jykzzdpb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mymnzulu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bjkwcooa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sarahzta.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yafvlahi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nlsjhufr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkvqlcw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tgnzaxvz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bkaffmlz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rewlumud.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcyalfby.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2txkpxxlu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2zzzzkpkm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vrdhjtsj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fckbivff.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wzympglq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mhbjerch.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzjrzpi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rivdkqrt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kijumtfr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2omlksplj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2teghmfjj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vsixusls.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2eaihqngv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gjwrqjtx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2euifnuvi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jfenqelz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2leydcirx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hjxxjajy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yxcoxdri.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tgrntffx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2faotbrdv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xvpdisyj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fspfrgrc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2upufxnzk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2roivgcvl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xvripjel.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vrjlsmlo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jncoxjix.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uxepymmo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2oqeubfjo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uuvefjqz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mjwxjugm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqosufh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vbldcuaj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qtjiufuy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tghukclo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vghgopkb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2algkkiym.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yvpabdsu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zhzpxvja.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrplpbzp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ajmpuxck.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxmfxlmb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xpaibeia.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ummtzzdm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttgstzrl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ggwndwmf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gcdgguhp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nfsfnpik.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbthylp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hmheikcw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lqwczxpf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hfvfjzkc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zhxpmftj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2iqdekggk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qrwyskzc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zscnvtom.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lkpzpecn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zfhzjvft.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bfinqovg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kjamsltu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xvckojhx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lqoktwio.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hrtzrogp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vhyzfcgh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rpwjodlx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xaybvalz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2igfsonog.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ijdaduvc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dxjzxeoe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ycvcukzw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nwybrsra.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2aupyeoct.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2owvhsrub.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zutuejcd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2euxklsho.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qrdyuqvm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2iwvxzccr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2opkdsksx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cblwfqfz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yowhktyx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2huhggnmm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ngpdharg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2agmgeexc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jqlbknqf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2oexmjrgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rejytucd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ghfeszkc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fsdtqyww.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ztoqqygm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ghehlnjt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ekwxuzpb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbpnidti.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qcjqxsep.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ehwaxhhu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gjkabing.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2puxdsbwx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftngidty.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nwkpvudy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2sytfdzck.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kbssgces.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iazslewi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hcsqvbyc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jphmaeyz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pwczdmrn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rpodmvhk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2alabwpjr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qoljiogk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tanmwcsh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fwurxeim.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ilvjsqli.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gljovasi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lfibdvql.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2igsjjwkk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2btakrksz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hutuzorl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2czinotnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crzlecia.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vbrvaotu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2oviswhyt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kdlwpfqu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2avhmpmns.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kfhowgoh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2yplifssv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lfgklhvu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gepvsiel.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kjrniksi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vhbsogil.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iquepsdc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gkjaluax.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2aidxvwyq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ivglhdco.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mlwzwryr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gsjkdmsn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vwgsucrn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2chhbsnxy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bljptahq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lbltmymt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kphirvvc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2phfjfxqs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdkrmjhp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bpfwjfus.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2brgwqbun.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2udxtegot.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmnvent.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qqdknoxb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lecfkzce.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ajfenqnj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kvjecnvz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ncombhdq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2exxehjqc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbgwjji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cglkmzey.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uudyphra.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ekpgvbzy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fnzgbduw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2krhassal.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gatzwgvd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ipnaurjg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ozwditlz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zxadobpu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gecukoph.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nzcrhnwk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tgjleser.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2edjmodiu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2otjyynok.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fxvjkdpp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vtikarbj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2umlwyrnu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgazrzr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2waxoriib.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zreqvmqb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hehwxgaa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2cxxpsjai.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zycdjviq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2brrpzxmt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qhjwqjcj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yhswikbr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ijlbkrkd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pmxhimji.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aegyzbuv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fhxwzlae.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2srxhmgkj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2htfghucq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yplwtvsg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rsiikjic.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpsekfam.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ihuzaarc.html


<!-- 参考信息 -->