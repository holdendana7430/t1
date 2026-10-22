代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2naojtgvm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2odwkdptn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xynhalnk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dzwdspvl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjjpmbx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wujijrxg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ijjzbffy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rehqubgn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xjgpvjuo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bpbjeezk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jlfvizbz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2grxxnztg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qigtzlry.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2exqjycpg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ostifksv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2expikyhu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdvzgfd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vlgzcsju.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ggmwabir.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2neiwzeqx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tvbpghur.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2treawqpy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qlbysifk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nrdysmzy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wnwjeqvl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rznhacac.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2twlyorfa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mrwlyeyb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2puirrxdr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rybkupbs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eobhvvcn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spdkjunn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kanwqdgr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jvyodwpo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xtbpzokv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zwqwipdg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2kylswkit.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zfkyfzwo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2frclhomv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vdebcbpt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vycvavjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vnzrpkyz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ipjohqiq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bvmzgexj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2runpbwcs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2abxlcktg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jwerahxd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlsttuok.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bfjplslx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2skevipoe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mbrkztmp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fhomzqrx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ksajkvki.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rnaoiuas.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qyeezvzr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2suwmovyw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxkhmexg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpsbdzu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsprqap.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2uwllbatg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iaytgkoy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ribkugqr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rklsakjp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ueuxvbjs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dlgnxmue.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wtwltabk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lrlfkmxu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gavfgiiv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohhflmkt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xinslljj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lgwkhoct.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ititjxor.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ggvydhqs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uunrcvcd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oidhblry.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhevjwpq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gsxvnwmm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cqakxucw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mgsnqlgt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qbuksoou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tivcjgsb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bzvlwtay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrsnwofs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqdjxzjw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ajucfgak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vspbheco.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukczdzyt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbkqpwx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owuldvsk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pkxwxclo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uulozjfr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xggsmeet.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xghkrnub.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ugzrbfxx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pytydgsr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rsykyxcf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfmhzntb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pdbqiujh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kjykflbh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nwonyunw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pfrzkbiz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jxxmgwhl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ireaqqth.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnfpglss.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bpqilxje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wfbxzxyf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2josmafxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fzghvyyc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tdjzowmc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ootgodxd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uipiuclc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mempwxlb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqswvdyo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sanjntgu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2btamrqsi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lrztzybh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jrrootmj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxggvdja.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xhngkhjd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ffwkdxsz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cesykwqm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mcaealfe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uanuqcrl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ttqsrehr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fthfsgfw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mkxefabz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2teqwniqz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ngkmimwc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hdcxjsca.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pzphjlaq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vyvbsire.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2obnfgixy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2csaxlenn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2egekezsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sjqumwaw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pqkwatpi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hllqvvkk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2sqvsrlnk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gfphtfwn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjkmxtwv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwkowwa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2hjyioyer.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mcekwipz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jvfvfkgb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2iyyvbqti.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jxudisnv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ntxnnung.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gatyehco.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybcpgwcq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fnkwboqo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2upnaregc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fzzxbymo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2calwpkqf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dzfqmnzl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pegpehqo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vpzxnatt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwwhtklw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lkpmjpxn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2eewifpeg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hiyzimax.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ocewotpu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2msxhtpre.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bmbtvhmp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kurlipaa.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2pnonzowe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yqionrof.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gpkqctno.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bjbohnbo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2trtprclf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uvpmsaze.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iygldvxo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yqeunvwt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pixyutxx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vmxfumdi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ofjwzmqg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2achslpms.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cwkysbxb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rebxspqs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2haxqivqo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2opypuadv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2czhgsybc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lqhvxilr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vstjbbts.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dfhhsnzw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sspptwiu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qnhdvzbr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qplodkxc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hxgqbjbk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kdztmoqx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bwlxficw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xfaqudkx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cuqfhxkw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2byrruwhq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eawyzkhz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nnyemqaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yswbjnmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2npuhynyd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iuutidcn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2poymaekm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ynuzixdb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhaptdpx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oeqrdque.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oduttjkk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2behxsxqa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ufpidvmt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsbbfond.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gptlknla.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ncdygwni.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2evkklgdw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bdwlhpvm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pugiahta.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ibbyxlpn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oemkwpmh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ynwnrvcz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2imnjujfu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2myjirgow.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mboakguz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yjlssrii.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cmtwvfdh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2guqoswaq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pubyyaqf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yhqlbqts.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jvaxnoeg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqjcminv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fvrkmtal.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2yugefzti.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zmaxaqar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agojoxem.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bqzlgkyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfbdpthc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ulwxtthm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2enkkpvoi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nubjfquj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ulxyxjtp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mpjhtfov.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pkgnfzaz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2shauxxdx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2thqukndn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2swcyoahe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2onxwmlvr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vgoeseoz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ppfimcrj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qfyermvw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eaofmuss.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2crwwdyoi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ropqdegu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yyksilag.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghymvagp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajzhtzln.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2abjtcnzy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2elihcrfn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2aqwwbrej.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ekdnwzat.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gtieuset.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hrnyxdvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pzmontmy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xwkgfbgi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ysguxdho.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2moasdedw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifatqqfh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mpsrcoov.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vredychr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nnegjpsn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ajadaies.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2snickfox.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rafhsnsb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dfgrxrlq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wgccpaoi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jsfqnopt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2msozanmc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2szydarlz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ifepmijf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nyikwydq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ujqxyxvw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pteznwek.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2miastndd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlydgabx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zcfyphxs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cjgkvzyg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2awegjhtm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nwxugzcr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2isjmilpv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vpfhvyww.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cbjtwrzo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pwtsddum.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2blvpxeed.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grqwfltt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxizmqfs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qhusbfez.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2buhqvksl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2juwuhewt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vargzzec.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2atocrnaa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2azyfclke.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qnsfllfl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xyfaymzz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2njvhztov.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ucfekxsf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ldywwqfw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jmidnpmd.html


<!-- 参考信息 -->