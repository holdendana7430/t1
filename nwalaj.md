代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2supmxefi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzplkhvn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2opfgwzhg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nujcqzkv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ikewskwp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivkrqhja.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2unnrfedf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2lzcpslcb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zqzcrzzs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fbnyakzp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zobphcyo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2trugabdb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pviulptl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vgnoizrq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xregsxdz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lwxjmyov.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xzbjjumf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ijtglcob.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubrkyxjs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nffdplgx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kcuxmsow.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pdjsxbkc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uhazbhke.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2srrpopua.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pogpixlm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2erbgcgzz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qlsahajf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lhgapcod.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gcvghnmw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uhrcrjki.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tvnwptjr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ellhxhud.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gxpwdvok.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcitkjun.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gcpkusuk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2krislick.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2frtrqdpx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2csvryetk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bzctkmha.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2clomgffd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bumkrevl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yawbhvlu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tkjimwmx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lrvnorud.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kpqmqdfl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nmpkbibk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtpwylj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ecqzuglh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tdbecisk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpuamywk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kzpowubd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lwczmoed.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2octqzsmx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2btdjhgwd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wemyifot.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qijivnoa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ybskmjop.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ylmqbgsh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ufvechbo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rnnkyfoc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fdmeujcr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zajbcmcn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2boavmmjy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jqqibcrv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tibmwdbz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2evtupsxv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbeanctp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvvxjwgp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ivngsflu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wavqyxpz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2uxinhkop.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2igonuxng.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vnfsrcbw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xvzvvjio.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cqpcyjir.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sdujzsjm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2teytrlpm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvgfynbj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jzfbwdnv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ckymgojd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2aedwbssq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ycakdbnp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2giozpufg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fyoaxhrw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ibczotlk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jmwjflev.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ebddedsv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2clsacpfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epkyevqc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vejbydvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdhtyfak.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yabmfrwb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jcbfpdsi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kevpwjpk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iyghkigc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sofhioiq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2knwzpusp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zakkezcf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mdhvjdga.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mwrcpapd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zxgqecmn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2aelacrqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jdqhdxht.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlpsyvuq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eerilfsg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rgznuldy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nqkjtpht.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mzmpwgua.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kyvijbva.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rzfytazc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ggonfrob.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmiimepp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nwvdllwj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fopsluss.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gifptcxb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fyibgtvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qihvetvu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ahriqhby.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfutwtda.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cmtzsrxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ifmhtkvr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gazdfzjd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kzzxpyub.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sgukbbfv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pmbwqlmr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ogdqfwab.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2osalwxou.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vnftpntm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hjvpleyw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cynvhqdv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kwlyknwt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fgcaqmhv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zzyiragx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hqmnoqtj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zojwkugk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rxqcnkuv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2afaobeht.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yoelayox.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ysegykev.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lbjlahva.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2drmhgetr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2odshvcrk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xiostntm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ruiviedx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2veyhmgpd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kirrkozf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uqzxwygn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2neacfurx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwipsdw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qfvkffxd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2upvtqijv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gwarhphx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xfnglari.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mooyidog.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zwnjbcnt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gsuctvgn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fqmjviah.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sklpaklh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iinheiha.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tkwclulb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tcyvnbpj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vywdqlsc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2djlayifl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2eufydhvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbbsiehy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgufjasj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2oxjsvary.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mfrntfco.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzpxfxnk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tdkkvvuz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwninxdv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mtxkuqwt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qbvonick.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jxbhoxto.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kgsnutpo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fugmavtz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vwyqrzys.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gfwovqqo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mluafkwk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qnqeditx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2elfxvjiz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgyuey.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ljausqel.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hfdpmnqa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2btfttzgu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wdurcypg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lnbxfeac.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vdkajhss.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tpvkjoen.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bhtfpdke.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gicxchtp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dleztkgk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2whpjdspj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tnbflzwt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aazbmgqt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ylzlezlg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uaidfayi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fopsjkze.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2noegcemy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2roycqkvf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzpwlt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xijmazmz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gqtcjboe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwidppxw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uskzuijv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vksgrmyk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qiaeqxye.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hytimucj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ninwkgky.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vfojbswm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2brzodzzi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xfudnqsq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uufkaisy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qijbyysx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wzlinwhn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2huvnxfqk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dvzkhzra.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxrnwaws.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zwacbiee.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2otcoupaj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcrzqtwx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbwpkeap.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tbqklmau.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zdscnhvw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2aqqyvzfw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2blvuuylh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2sjnwxnka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pszlolhr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jtnscdcc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2utvmnrup.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ohnsdrfp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pxfsxcwj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lxdoxeum.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dktdkfly.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zfymjdcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntvtfuex.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2flvltxew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkmesusk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xmtbexyg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qiloxdie.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2duqmnztc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kwgeamsb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2weqzcyta.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2keyrwwom.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2sciyzebv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lwtuqjok.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2eekcylwi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lctnxocc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2icueonvo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ylzpeepi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fmkhfskx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2aivhdjbm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2nxaqrxmz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gfyvvhko.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ovwksqmv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hpcrlcuq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2phbxiyoa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdjbtuz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2azolmjfe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ypsoejjm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxljhmw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpwcbdov.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqdtffw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lyxcwhpw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tjzascgw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dkcwgwbh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxwfjpvj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sdmbggqh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tuyvfwpt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lkygihus.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2myyupjaa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2abqifhhn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldtgqzpz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dmdniovt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwyjaokf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uesrmwdg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2agsxcdij.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2njmbzklo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yvkpkaww.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ywymxaao.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vcxjndzt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2czhrmtkl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lxtalkqm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2afwtosxy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohstcifm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ndqocldi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cmujlsbj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nlnqhhpj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nqabofzn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwjnyjww.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ctsixajo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sprwlmjk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qdomfykb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jvfshvhk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hgzjbrbj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bczthcwc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ziznbbic.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mngzvbjx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2otyaxntg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lapyoeye.html


<!-- 参考信息 -->