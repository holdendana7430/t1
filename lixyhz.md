代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qjkixltc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cmsearss.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sewpfptc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ptshyfhy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2stedyxov.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwdgmc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ekdupnky.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2clotfxxn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vcsuhach.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlrxmigo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xbafffic.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2adhgrlsq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ufbngfxp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mkuxgkdf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2arhajxos.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rsdfejse.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cxawclzu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnpslajr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mtzjissl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2egkskzus.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2btnxkqoy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zrhqniaj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2injhfzxj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2keyhdenh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xvztdmyy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fupdjdor.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfjrvpzh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xhoxegey.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvmcast.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvpzznwu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kmchrkms.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2glpmjudh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qbkzjcgp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2flfvwhzc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xwogxyos.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2teclyyno.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzuvwyea.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iopuvqcx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2omtmlvhq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zgvntfcn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ihjmqypc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kualpcgo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ptxvsgpf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnjcwrgx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aviefist.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqtfombb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ntfbafjm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezxxjsfx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tqhwvpri.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhquxahy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2usyzlggn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nhxpxjje.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zcnjdmrp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mdfymnyf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2byfkxnmt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wbfinkud.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cckjbjbf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vbwwjptr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2itovlksu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vqqbxxpy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oibtmulz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwxwdtpk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbufvaw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdhjovcp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yofovapf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2julmkxhx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2svkyujlg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2patxezrw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jwkjowiv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ftysximo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rdrkgucu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jochwszy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oxtqufrl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wmmyqwir.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2povdcjcc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dydxkhbr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2glfknzdr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vmqagpht.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gqtlzswa.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kinrojce.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kmdgaart.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xykuqbpn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jipmmbqw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hglkxkxn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tgomepqy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2joeiuldi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tetiprkl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vzylvzwg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ghogntth.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nicosryp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdruvipk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eniowaea.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2blcfjyjl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2eivzpqdm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2woxqtyaz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nopjxaxt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yucppxku.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2finittdu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lorwnweg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2brryjeuj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cpqmcurs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rejgsihb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2dgiltaos.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2afpvkvyg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tbdsokdb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2amvdwzsn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2reyiokzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ysodgshw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jagkghrs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgtgyrjw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtyvznx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykofcjvx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cmglcnoy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pwqkecju.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2alpfraxf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fcekwbpi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mxrzgwdn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cybmfbpg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ejvopaxo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hrmovhmt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xajaqyvl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kwxcjqoa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oadtqhyf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bboabsbi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rerbrupa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wxuprjef.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aqwxuddx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pahzpcyk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wjkcjjcn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bzkdblmb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pnkfktjv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wkgrxlvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdfihcdm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gipglhfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyevydqw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcgqlpbt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vwkexazv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tmvgonnm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjxalbgh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbzoymwj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkkvjzwo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngowfifl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqiokpbh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rojuovoi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mjvanbhw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vxtmgxja.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2aahcmudb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2keorqgqv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddkgmogd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2saozqupw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzcqmxzt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ctxryzmi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2weiffnet.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdzdsryp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bdihnnnp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpxxrpag.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nglijhxl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzittwhj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vauuecim.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2nfwqfhab.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bfehlzaz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ngkkxbyn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gemxjagu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2imfyqcto.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tiuwivna.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsftpkki.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tppxezfy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rrqtmebl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vnhtwbpf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjriisdd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvlbyasp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2snfxrdaw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pswacqli.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xovpwmdf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2quhdebhp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sotszrpw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vrwbuflv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fawukmep.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rjdkuplu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2twdnacol.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hcsfugis.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2syrrmfdz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hmggdipc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xrdgmapj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dprswxaa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iqubpkqg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uvsdfoda.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wcazyume.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kzimegbl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2deovigrh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cxncecow.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2whttgqlg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kuyuewqm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vawopagb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yaoqdtyn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2leabbewq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ckzanyej.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kfvibvpy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zjhxnenf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ynailogx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lazvvnve.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcxbbtma.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gbiieong.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rpmxufhw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dxxrdhqj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hizvrmba.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ruriixfv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2srqbimyn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2svxbissy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsqojmrc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2oeuqrbba.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2czienevf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezabcyos.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hnncvyht.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mgafxdkd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2btfyeicp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dthdygef.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bjtcjltc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2iuwuxvlp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2cacghdrn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ygpmklrf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2izceeadp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cllqiege.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fusflbon.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mogmpzyu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2asaokktu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2awgzezoy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kqcxdnmt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dlpjdkya.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fbcseops.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mjuoplhe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2laplsdur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hcjkunwc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2afgkisyw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cpdpujlu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mcsnkylw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tccvvwjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ijetvyhk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xgwickef.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xtiuhxrp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gqqegkqt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jwtctcnf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxxputvm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2azukrpfh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2niaokhoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qodnjtug.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2aiwslerp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjrdkmhi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlsyyzh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fxujlmcc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ugfpjkul.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zsrtjsgd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbchroxo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jzywefzs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2setqrvla.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ryocytfj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ztdrcdis.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2botncwmm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uutywplr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rtypidqw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xmlkncwb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2quwxnjdr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ubhlseet.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qalfetir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2shfngswg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhmcaaoz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xpxjqodj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dopkvaju.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2skiggexm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jdfozmjd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fparuvth.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2edgoxyyv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2guwvyfzy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yssdzsfh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zizsrjxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jocmpxgd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rckwbwwy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgkpadqz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmkkmiip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfqmuekj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kbioetss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwxxntyu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bvztmnoj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vurlnkvw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wqshrigv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gjqtnidc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fnxxyftu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tppsywak.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2liwrtnss.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zsknpyvt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vncqtqjt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hkaamwig.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fsogdups.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lxchjmdy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bglnryau.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xfsfnqiu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kzxntjcm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjjsmgg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ipuqmcym.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2icnfdrml.html


<!-- 参考信息 -->