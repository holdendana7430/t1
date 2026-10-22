代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2eszyqyaa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wztlnvxj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2coaulgsi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gmcstzlc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nhvwvtmc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zjpaoemj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2msxnaaim.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2arpqyjpk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2imtinfty.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uiuekryq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jixwcjfr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bmvwgpoo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uqvjbfdq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ttvthbfv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gumvyego.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ifyasooq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dmtoepza.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2utisjdvf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fvxogxfk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cubsfxet.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fljfwbzz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xsffcofx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2pgpnbtgl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2orcatnua.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bgrtqetw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmdqnodf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gwrjbqaf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2btuwsbhz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ejikwoyc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zluuvksq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lqylfouf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbobladz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gcbzkrrp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rrzjohtn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dfvztulf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yyohvrls.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xjvlvsxv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jrafzied.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lgunyvqh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fhprrvfl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yjdaggzg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xmsyhrln.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hjjhqwfl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vfbgbpmq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2acuhlwzg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mwmrvddl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mufsmzny.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgeuxxfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oqldfron.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2atntjaso.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jijhtiwg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vppywxsz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2knefvmlp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fqqiukqe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gwnpzrck.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxxyzyt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rigumezk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhwblypu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zpmvnisd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2shranqlh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ahixcerj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xaipvnsc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgsjgzhe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2itcfkweg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yiymxlqq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pfdyywto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgmovu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hducqawq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hqfginho.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ygavcsvs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tngogcef.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ljpdnjou.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ouumtvpi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwupdaha.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ggromhlm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bdlhntzy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfsvnbf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzcqmokq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2delyfkqq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ggagearu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vgfiocag.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtuoqncx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2amcfzosi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zqsigcxv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2smcnsusc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nqcviilz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uwfuxuqi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ijzfypmh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ccuoxifq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2etduzond.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jidvokfn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2crzeimek.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nzuosqiw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ihwrivau.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dhkobnco.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2somsikzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzksdddk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tvafufmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvrshhis.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ermnxjmx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wdlbziim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shsrfmjx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuebsvrq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ywxuzwou.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwxeapae.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2srdxtrhi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2howibzcz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkkfkpda.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyhukrzd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bgkfzkjz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sltgnjbl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uidydhsg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xpcckdww.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2egnmdiqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vhqtlboj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qhqfgiyn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2okmpexmv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcgwntmn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qtlkaaio.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2houtvqah.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mxtoussi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjaxxoum.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pnrfulmm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ayackijp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bbvmvbgb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nnyuwxkf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ppaidbqx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fmejybss.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfdazlux.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybamcqej.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jebdqhsu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2clhqdtgd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kkrjycsc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjqlbhhm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kfmfkmiw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nllolubt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gdxaurdp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2oaryrznw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nbmvbrzo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pypyznfx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2eeewhmbj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jvxrrqom.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tuudzzne.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dqwvzfnk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2whqingpy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ubxsjrnn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2beuyjmdd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hkrnzinq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ffdkpiwd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tfbisupq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lecvdeab.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ksvukchq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hukivvnz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ywunnoqd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ayftiuvn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqpsyufe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmpnjaa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lfyjnhab.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkolvldo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tqtjufwu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hksduwky.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2aktxbrbb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2frpvrtfi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rygurxyo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2piaiqogq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2khrxhooh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpzfipna.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gpfszbtf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xtniffhu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jornrcwj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohctydqx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wldrlvpx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zxfddypd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlxmwpu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2slqquaol.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ebsdecwf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wmztixhr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2coihpeea.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2akxrngwp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sjjihvkk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rbxhzgaa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fbwaxxjy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2axhexhob.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2eqscorqn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2anvdjckw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2flwecpzp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2exchpcpd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2iieqsucs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dgkeddjf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jvxlnvzb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xidkxgmv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rzwqczdl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zocaaree.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2euryihlo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jpnesbrl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cativcrc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ldeggsgd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wuekbfjf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zttxzrfq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mapserwa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rmedvqwi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2donzjtwg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xfmiffvn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yffqcass.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uqkfrood.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vojlxpot.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2itirpaej.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2prodcydt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jcslltdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bonqpftk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ldxrhwqt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sqlcvjbe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuarwgtw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iieqzcnl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xgraiaiy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ihxtvxsn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlqwrvkd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iuitspjs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nsnapcoo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2owsattns.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gwnexalx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2swjrggcm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2aeanwqse.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eziercji.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tstxflmt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xfnpamrw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dnjkwncv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ugrrhpui.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uenafkzs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2oqhduezv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yrhdvfbr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2iffewbbh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uhhucrcc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2elxlapzd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2foagcmhp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wgyvucwd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gguicalu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tanajiqc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2utjipvzy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzqijaii.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ycltylkp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tmfthkrs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2iloyjuzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhjmreat.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dgfjtjxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoywxrqw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ssfzbqmk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hekfaacm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xqynoeox.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2arxqkgwh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2psuxuchw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tqqkcjen.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fhjzyqhj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ldjllapx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xqaslqin.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wfehtzyx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2aicnaamx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xxdiznlv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rvxzymgx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kywvuwur.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjatehv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pqgpflcv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xkkpwhfr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dlamvghk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oeocyvoj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kaluzejl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jsaxipud.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2anavkugu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hjepvldn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tquvuffs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpbboqd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jgvmzruw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ffxozdts.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2egguubyn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xtdcwmeq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipkrrhlh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xkparzcm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ujepwzdq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2skefgztb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2liwyentc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dzudxdbw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2aayguvog.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wyavggks.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tzylruyr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fwqxtvul.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vnopckgt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jlxxghei.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kytswcgc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2avkpsdse.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eiuvnbmk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jwardbbs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lorcalsk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wteclqsm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ankriqot.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vqvcwtfl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2iguxjgqw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2aayyfzrf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhmudz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cebqpiok.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2brekhyrf.html


<!-- 参考信息 -->