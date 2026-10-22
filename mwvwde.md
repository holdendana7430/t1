代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pyoytqnc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vtzbxjxr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kujdxjnx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mblqdufp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2luabvkex.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xaqkrodo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ipwdijzt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zoaokxai.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jzolhiys.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2psozgqfk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2veaqwjzb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mpzgmrcu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2arevahon.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2shpsgqbc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pzqovxqq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpszzza.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2srczudsv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pivrcywa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kawnacoc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2izyzcach.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ewclhcte.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cunjutov.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rspbvfmt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mprmgcfd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gipjqomc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2eyslhfur.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrtzqee.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2upycxubw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjcfvedj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbltmmci.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2devjffkb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kokkixnc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wxhlysbq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqzcfpmb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rneiuybs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qpwythwa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lprjlvps.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwxsbpye.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2npqfebbo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kbhsamwg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iyjjcnoz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2djdbnhiz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yrctknng.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tikmoyfs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mxbsfvzw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tljzfchb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hcfdunhm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fmckcfit.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2naouksxw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ckbukfjb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wrrcissn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fkwauxzk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vsfselcr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujffyexs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2omekmoxf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tjnikroy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gbjankmm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2izkopxsf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fdhihefm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gchaipkm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sacrrtxx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2opxasmdj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rbbmeupa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mfzhstvq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ifonopma.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bkapzwji.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jcvdjojn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cuoeduof.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bvlgbdvt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2navzgiwq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ktaswrlx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xoycwlwp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vfqemvjc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2saujlmoa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2njmybjdn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ouawjyid.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wrggnosm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zrlojrbf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qroydjip.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2oiqobmpn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aqackwea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xpzfqzyw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wpznuycu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eebkwyme.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxtkhijl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qjfemasq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rfjboirw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zqtkyqpi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2iansfrcx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nuiseyha.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkumrsgp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2imxwpyin.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2komyezdy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xzankdwk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zzniynwj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ytutyghy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hllcbdoc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sxyqgkwq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lhynfipi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjrmvuh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cgrjuqmo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxodtafu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdoejmzg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nsmhoggr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wldpyekz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eajynfls.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2uoytzlem.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lkyiqjig.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2efyjabur.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vpdvrhiy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bokiaqrf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pcsfdgsq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2duuhscjx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oviprqlw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xyzsakqz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xfqcpzsj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ytecgyhj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qukugjhy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fmgloydg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jaojfrba.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2imoehutz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gpmclauf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bqfchtys.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gizvvxqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkrofumm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bxyfzlfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmvhbgic.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2skdvrqxg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ttlzavcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpewsxvj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zroifyll.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2umqlzdfd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2elbbjcij.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xjzzgqqm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxnotjbj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dwkwnujn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2twywrywi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lgthgldu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obpkktot.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjoebgo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lnlkibwt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wpfsxcnl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ehxnvafm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wgbvjzhj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eybmvjhf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2copqcshl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhroiug.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ynzjzlnd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hzwfhzos.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2antpdgkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2aepizqez.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dlbemnig.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcavfokj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cfsycvpl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lhelxlxm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ncoymxjh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pqakyvel.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akatggel.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vnqnszxs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qpluurds.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kkhdxmiw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2psmwzbay.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrszcpnn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ybqdeyrn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zrcllpuo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rtuustvy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pmwmcpsg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zfqqfnhm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fqsahmlg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fcxxaixr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xbsuijnt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2felujijv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bdzhymqy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xgydsyyk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lcfrklwo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2peicljst.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ifxesvsp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vfjmqrgf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2lvvkwhdv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sgdvcxlg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xpiivnmy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ntctmghz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ixrvssxg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ttqhozjn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rqebxlnw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhjtqgv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuzgnczi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xkgqjfgz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgxeyci.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2svncurlf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gchmnman.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tranqprs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ccevncfc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pjhjcplq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkbytxik.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rhztoych.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wmhkolix.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgngdogp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvyvhup.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bxbankkh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2saousfoa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dnkeuchn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qqhbrxhx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tlyiltke.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nplnymxu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jgvbxdme.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2synojwer.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2obmhclwd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ldaccuot.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nnifoxee.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gkxybyss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lajocgsh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tibpzvjs.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cfobgprl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zssnquej.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pbevbezq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uebljjom.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2iiatompt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wqkrdrwt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xulcamkl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xzibxfen.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ovvfpekf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qthuiczd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jbrjydzz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2weqwcbfw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pwrhryzm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jvvjllal.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uspxwxjn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tivrrofe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ofbguutw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eegyuypq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2myfegufw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2axpjhfga.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qpiagssl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2cuajhtjg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fkrplxaf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qdvsymzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmbzbkw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nsboadsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaopumzn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kygoqqub.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2odnbhmkc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ixthkesp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pvkoucim.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kswvmwtt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vzvazwqi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jsdlwbkg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qjiotvfr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kywslhue.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xwfxnfwn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ibqsnqty.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ezavtshd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pqbmbrao.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dznhiurt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rxfrcsuj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ywgskent.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwuzozaz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaenjtrr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2swuzqxib.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lntofggx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2shhwltfw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qczghvhn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zfmohmkd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mdigtcto.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2oxqkgqdd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hjawhhhd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xkytiime.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwrqikmo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wjwakdiv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxqqyyzc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtrbyhzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uktdzgqn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zgulvqhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyjgehsm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gmqxlcqu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yeqcuqtj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2heynvxte.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qomwlmoq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kwdoarhw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kjjpkhbo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2kpxlthzc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lvlunfyh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ifemsjgt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2knlhfbcy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2voumspwo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gtmztmlq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uetkhlrn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iiwcesfq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ukimgyio.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ihwhvzsr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmdeczi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fcvbebcz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ieuqgmjt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gtkfolzs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2akbttkxn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xlrfzvmm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zobwcwjg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oowhegvz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2eqwrvbgn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2updntqht.html


<!-- 参考信息 -->