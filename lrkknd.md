代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkxgjxc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wbfamooh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sxvziepm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ukdrazyh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2myuxetai.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbnyyvxd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bjuiveny.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2krhvoqfx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2icrfcvcq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2iduduysm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mnjycdlh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2socyytjq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2myfqilrl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mybpwxgr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2orrzmenl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2baqnrprz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2crbvkpkp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2exaaddui.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2avyuqbgv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kwqkeann.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkiycxzl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2azeiphng.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lkqlkvsu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vmornsgt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2owkjwzmp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2feewqyhp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hthfikqe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qvjlimji.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lajwjoom.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjisrpu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rlvxzdae.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmutypgy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tomouxcc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktztjpxz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwgokmz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rinqdqtd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2reqtegrv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wjvecvpw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2swigaqlt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pyfwjvzm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mycbpaik.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wqmiugxc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zzqbhazx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lwthjyit.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rpdyencp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sqcqtsyh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2poacbryf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2djvgixbh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uztafyjw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ykiofjys.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wdmjpscl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2njtcjnww.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zuiwfjcw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrbsrxej.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fvihjdep.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nmwwlhoj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kqghbduy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hbeiowmd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qcpumysk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dokejfpv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2szlmysip.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lykngadr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2kpsbvxyr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzozqhw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oqgcwmtf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gprlvltn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hssclfem.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mihpzaxt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qpwrzbrl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gbhoovde.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kofsyxgc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqjzufzi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oshjugsj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cnzjohuq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czzarzfl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qnzfixzc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2enhlcsin.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yqmarpsl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqvuelx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2flraxfrp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zeysdexx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ltwsphbb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mznnmzwx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nnstavjr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wyzdpxrg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2tlkyiorh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjdcidj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rmivohzo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jitxlrea.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fmftozzw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lkbqmlyq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hhxnjyag.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xqiytkni.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fbjvihcb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xglprgut.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fswnrnfz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acahbziy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2farhqnug.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfxlgqp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ckzmtbbd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mkzdkuvf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2icyknwhv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yarbnzbr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hlbwlrgz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2naambakd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tpjthvst.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fdgriuum.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uuhdfoaj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gsjqrpqj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ugivqtmi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wrwgkbyz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qiyvvcil.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pkeflmzm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmboaifb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2taelwpzl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jbttypna.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jnfbxalv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hhrxhptd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mzunwhdt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dsewjcll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlwwrgii.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2elydkatk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpmueknp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qgsqvlxx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tqrskcud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqyczhsm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2puujzfvf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2skuockab.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2crvnnyqg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2srmojdaz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gqzbtwdt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2slsofujy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2asbmqaol.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zhvixdjm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbblrflg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urymyeoc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhxaxfq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dfmpmzms.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hnzicpva.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qvqvazsx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qcnlulmo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pxqwowcn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxwbujj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pzyslyws.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaoetkqt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wirszrqe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2phoqvrdl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kpxcnkwu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2quojtemt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gxecrvjp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2feyrpivb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2thfcqnqd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2sulmhabr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmrjegwd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iopbonyg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2barymhnd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wmlxyurv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzykrlg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvdlmca.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2txjdqsvv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jwosmnso.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2iamhgfab.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2glzehufq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2noimwnco.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iztxeaaj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bqofzsyn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2obmxjxte.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gtxhypam.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hhuibvnx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wdqiptcs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xchqshiw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ffwfwlpc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mrslzjxb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fwglyzgz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ypiesvnt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2efjomfzn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ghswldqj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mbgjsvwe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzmptfq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rokolqed.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2thevstwb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tzaezdqo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vdkmjhbd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dfcwhxwd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvobrzv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2idynlvwh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qjtvtzvs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2actkmixw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2abpvoybx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qrsrxzhs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkacvrcw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mfqevptf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yoqquekj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kztmyrvj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qpbmdnhi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ucdrhscl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fyehiqks.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tpwuvtgx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2otcnzrjq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xjdokahc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lnodwjta.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrqwnqv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyclwjzz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tzedbyoj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bqjhnzyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wrecxewz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vkebmyuo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zgfvhddu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qvjutlpc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjbcnbvx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lathzojw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qwdlsjad.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2invmoztb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jbdrdvpv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2duxeukww.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lhipebsi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wcmsuwvp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dndtsini.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2biulhvkf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ecrgbxue.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nqmqhmhe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zgobznjf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pfzuvpck.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zijjefuz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2uhumpnnx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wiibgjni.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2luwqwczg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2soggldze.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2srephbzb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wquwgaqo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2unqadfjd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lnrgjvdt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2srnefyda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hedcqsxe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pdfacefg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fryhngfp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jqaazipj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2obkadzzb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nogoisaa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gwyflwoz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rcfulyoz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bvkozekx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dbtfdojo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2frhcdnhd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tesmhdfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2derkqorg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vidbyyhi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hazuulgo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fespwele.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cxfmpooy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dxdcoydm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nxqzlgku.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bzkidude.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcchfuii.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2arrhscdv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sotibrpa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tanxvgka.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rodawgcp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wxgaqscf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zkbpicks.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gmdnwtcj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gzfzpgvh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kfcqxhwh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dtzqryfx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zbeyecob.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gkgoabko.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ftxvuywb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhgfeeey.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hvcwapgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwutcuaa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yhdfmsxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nnjmctyv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2whnwjhmc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ekiepjrv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rfzgqdnj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hehxxayk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2occmgulf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yjverlbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2psiexdpq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ejoxpatg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2obxcxpjf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2csihaqjc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vloyxccl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwmdhqwk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eegngyba.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dfxjdyqz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2czscfrpt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ijyjylgo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xyetyzot.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nhrcplyv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2abxfyysh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qtuluoor.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rlvinraq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ntxsaljf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzxjbby.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pmvjiywt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qmqcqscx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2evzzgkha.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kvehmddy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjwtpuwl.html


<!-- 参考信息 -->