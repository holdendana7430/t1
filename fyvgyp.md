代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vgesnudx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3whdicdnu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zihknvix.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3avjryqfz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lyslneid.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3spmaqfod.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrkugbk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3emlgeotf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtsvfnj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qpmcbchs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3njwpcfro.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tisrhdzn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wkgdnlvp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gvjpgqoe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnzclhzf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3usmaqjrh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sopqqwtj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3njmnmxoq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rkrdnoqu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tchuoaju.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3szilejuk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jdczytff.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nrwffomd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tfhuuzlj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fypajniq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3odsvetfw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywehhesw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ffxdehpy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmcelby.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yuzhfgbt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vbhziaht.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3exuchxfh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzudtxkr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qwkjdvnf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3odjgpmwc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vhlmulez.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3eipcsadp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kmjejrrj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkvlszps.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gwnwrmxk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pbtfegne.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3btbildjs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hbepnfkg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pybwwnay.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aekhqihz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wicvdbzm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jzwwrutv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jrdskgpc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yfccromw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wnrgbeoz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zxixcspk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3knwsmfes.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfiibvs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qrvyuphf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zmeepdcc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3eepbkubi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljtvultg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yikungsn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ibkwqjgl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwykzrci.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rhbhapek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jbzjlilv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsklrrjd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iusntmrk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kwwvzfpz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgeevde.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3aaviozqt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zvinjmen.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3icouzswf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ddlnajki.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3izampghs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ecxbtulz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ntjejzcs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3luovsozn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kmztrmgn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3joszdmny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3iqayqwsv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cirdqzqm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3smbiovnn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ucvcqkhf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3evfelysh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3htbltrtg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lhrksayy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qlmlfeeo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3cxbdfkip.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3asnduvhd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bmtpwstx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3imvovozp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwqqrnn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3fjsevnko.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fqptvjit.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vrpopend.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3owkthopw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fqkmmfcm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gkrpeiuv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sdvzfgzr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nldyyedi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hljsatnb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmucjki.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3dkyeipvw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3weosrqfs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mdwnpefk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bzctubsn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ownxqptp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3imjdhdpl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ynajdvlm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cwwboyqh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fbvyhlca.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbmioymv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nhdnofoq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mxzbbcni.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gecriizl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ztsojdxc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3amgrbyyc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3diiqqast.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dkijvcwr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3psbvobfk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3iqjxlorp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3huzjsmnu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hjjddazy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phnrnbet.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zmnlucrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxgyvnrc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bausnysf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xpcycuwr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3itpqmuxu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3asmnoklt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fskjmipk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhutquwl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dhcjttst.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pszopzuz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uxrpcrbi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wtcskrvn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fpelmeno.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jhimhudr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qkrhlpqw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ueniegws.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fxbjbjqt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wzqvugvc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xpqrriel.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3thcshjkl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hsuyqxwe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zisoxllv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpzqvezp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqlztdwn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xfcfgrok.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmlymihd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dqiqcwdi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3teqbpbsx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gssaxhkd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jnfongzn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3gcnqayro.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tcjjhqsj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rcpochfh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nbwfvzht.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ordkqmam.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kjdwwmkr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scdyemez.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrhokphe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yqkopxsc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bwpalved.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hznzyjcu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3afxzugyk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wzovanyc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3amjzndlu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3alejevfd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oxayfhui.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ffthpcuh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fatgryjn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rzdodowc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lulvbfvl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fthpcmpj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bifesjph.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jfgjamol.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pmljyzij.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bovtjeyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yzoovdje.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cbdtewow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dwfkweny.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chjwlaaw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3stzhqaqh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mqchijgc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yzsrtspf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yyqhwtbz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dccndvuh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3eyvqnacb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vhiidegk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lzrdghyf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfgrvsnz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3plcssnsv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jynoewaa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3powqdcmr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rsnmkubh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bxxbixki.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rfqwmbnn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fzuexkwo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3olckvtbw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jqdmcqpv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ycuxwkim.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ahzeceqs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jqhyzthy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hkcynltq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eksioxgi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ennrprso.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lwqiwflo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lpdkwzlr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sddhoiak.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pypzebwp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sbanpxiq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rmqoktsf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mzewyatv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pikbiznv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yskgxqqh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lwpucwnr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qfzogabx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3iqoxckuj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hixrqacf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jmuqgndn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3noccwbpf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mpchwixx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3eqrfbqkm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nqlymelf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3avmepuvz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gnhviljm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rcaopubd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wepbgcip.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eazbkizw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dljbrgil.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xsevngix.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ejrrobfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tuiduzkp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vmtrkdww.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3asuctqwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmrywcg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gcuomcxi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bsotzwcp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cakwizah.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jiotuyvp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rpxxmkyk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cskqtqgq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlxkercy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rptmysra.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cumhvjaz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qcukyjqx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qdtxjiom.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ujyydjxe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rnlqmwca.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fuokuwdz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3yhvwnvpp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3udwsiqaq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bxfpvdiu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gqrncsps.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nogcrhwg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gotidjun.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ihpscbrj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xfrfkgwn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vllafhil.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qcajjgoh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mykhuunh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ddenkbhp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ylrejdyx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pqfmctoh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mhdjrrbh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cftwqqev.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3dmpfahcw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mrjbecxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rrabziwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwktrlwo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ywkzjzui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnehqmkb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lnsmnkei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3upicdpfh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nzcezngz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hodpuixq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vsfcpeph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uzqzwsdf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kliyecqd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dajnwqbi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3sxghdjbb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3opmovshq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xqtqfmay.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3geushtox.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ddcrhklh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dtmcgeoo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mvnayrku.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fvbgvcwx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pvarcopw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hofhzrii.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tldbhivi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjzxngq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmehippn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qiodnqnw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3klbyqktp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gctuafgb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3oyvebrcg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uxfjbpve.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3feajcgne.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wyojfxjw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kdgdcfkg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3enwyylgn.html


<!-- 参考信息 -->