代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lrjmdxyg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nzajeiws.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bcvmjoeo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bpgxamps.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2anbzrjgo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwatgmme.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yztotzbw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yjhogwwy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2blshiipa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gollftxd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pessloet.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbplfwln.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2awmxqosp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpyumju.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2iackuuvg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkkdqmjb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2khvkzply.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlgyoeti.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2linpxcai.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qulfxpzp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjviwekb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dcacztqo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfaltrf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2szpapvpg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hohnyske.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lokaingx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ccmjoikx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2frdgmtfa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2apmgwvkz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2htaydapk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2whhabbga.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zasonsqh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tjbwqvbu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yczywtuo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dxfekpnj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhmxtazp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ezgamccj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mynajeqh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nlmfkmza.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xefzozan.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jkywunvm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqvnkxme.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2airvxrim.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bxfvoehp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nfkxyynu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2idqrgmyo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2epyarsrl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rokhmaaq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zaepmwtj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2umpkgerx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uaswrdqs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylihoqkx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xohipzos.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zamwtjlp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kkhnwbex.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tyivicpz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hitgctpc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xoaadbei.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdtqggq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szjzxckm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vpxdoers.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mrungigk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sstezmsb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zstnkeus.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bplyvkhq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ozhprysw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wspzgzfn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iphocmxc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2yyaafbrb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bgzwowgc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxjpfrbm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bhezmpgr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2napetmzz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lqlblxdn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jiiburid.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ktoajzol.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rftiklbh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ghiiurnv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2erlrrcwm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygtanqjc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fzrupcco.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ffwboxns.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2sbtkwfef.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hfzwznkv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rdbqxfyh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xricjfrn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzrxcwwb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfusggv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yixhpmrm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dbodgxkn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xwyysgmc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2erwimniq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eotkjvvl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cqxytzwk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xrxgigny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sylbbwqh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dafiukgp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uentbtet.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mifdzqed.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfwakom.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mfpwcykg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ijprimtd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vkbdehde.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zgohelix.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nkmhvoqd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zfgggvab.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yhsdbvsb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rlptfguw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pfttibln.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2juxurnvo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nkcbqyqj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2miajbukb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mqlthuvw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbyjntnj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2enbwismn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cqhbwnky.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fyeyouag.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cuvlcqlz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2emzolgwm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dyjqctsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idwknfgg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vzkeaqpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opsxmodz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwjaamgg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2edbzhtvb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwipccs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptnbvplo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cncfpznb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wscfifgm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ovcxxord.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2aaywzbjq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ggtxcygx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nhtbtxgb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2olzaaoug.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wydnjqsu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcncxvbh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nftjgtle.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ruiezuxr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbextlze.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kmrjbwiz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rjlsumqu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2grriiamy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ykrycudm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2awzubrlu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlevpbpf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sslavxdf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qbjkgzyj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2stvszjmb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tbgmsfxw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xfbzuhqz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2gjcriyuy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pjesouco.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mujongli.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uakyrtvo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ufmazmwb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lqxvfurp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vubxqvsl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjtnkelg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmtyftq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2issuwbki.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xdfohlss.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ckrxisuk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jmndfkjx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xetdlasi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2utwxjjdb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xqeqqbwc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2albtgegv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mufhnoeh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ijkdckxo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2daclxxyk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tjyzhrtb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fbhoajrt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tgxztohq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2puwnhrrc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2canoobjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rjjlvvip.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kwtoyalq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2eqwcihxh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdosvcc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dcwmpvfy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bkbwfmxv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2miruiizw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pvvpduqb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2axzutlih.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2plnrxrvz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hiyibscn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dbzpymov.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zbeeccfu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fqalwmar.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2crtncbst.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kanglqxc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ngkwmvdt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rkiudijb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kakszlsh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2psbmvymc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2csledawu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tusixmax.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dcsmtrct.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xizmyprq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2batzomhz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2goysatfx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kzrmharn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hhnlwryr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dvoskdzn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2utnbfvpw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dbpfwpxw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dmikbnad.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bcovhbqz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tbljjgfw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dktscwzt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tttjvjvn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dpfbtnaq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oleiiutg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2actaqxeb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ayyawycc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tgpepdex.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ztuwtaiv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bpnobjey.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wwawbsra.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zhzljbbm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2plhrdznn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nyjopbsf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jquvlwgu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2idsmooct.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ovbdzktr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qsafmlyv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ckbzqsel.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kbxkucol.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nwmggirl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lrmrfxqf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzvhozfg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nigaufzv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ljntluon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zejdhiqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xvuaaame.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2npdvvfcu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2btocabnw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pucgcggv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sopwhoji.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ejzfxgml.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bnzjfqtc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dqzlruca.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lbxjwfbz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kxrbuwcn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dziicgsc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xpwruhkm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zrcegvzo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2axhqbhsi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rwimcadq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bqzagkpj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hzofubjc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2korbxico.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fgutgejg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2accgipcd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fasvynvj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2klfikrlz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2agxljtlp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qphybqat.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yzfnmlke.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mhnpiqjm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yzgybngi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jvuftlzp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ryboduux.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwgolqdo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bgeizmpw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mpfobeea.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoulpjpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iftoadtq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hamkdvgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txomwagd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wspardnz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qunpgucw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2otkcprvm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oxpbtqcu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jumcdcsr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rzvvrtgb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ijekiolp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ooepjxgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tggcgtwc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rgnqrllc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tqjcetmw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dkeqcymq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwwliuw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mgpxtpbi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2voxboyvp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gvutrzak.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tucaeioo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hnfjtvxf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2drdmpjis.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mwscztfm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fauqmrlx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cdxjvpww.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igtkfgha.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cytfyeas.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ygkflqlp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jtffeexy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ivgqftnz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufbfhfql.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ddzrbrdi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bargrumg.html


<!-- 参考信息 -->