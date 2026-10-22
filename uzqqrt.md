代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rbgjafbc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xgwbizzn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2otmjndai.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2utorhbdd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xigakeaf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vxrieyax.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2olhbexwo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kpmxtjye.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqzjdtd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udvidizl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2krxqmywu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wdgcagvy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lztslkqm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2emtzijdq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iyegdkrq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wejhojdv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dqixkzvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuqopcsw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cakwmegm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bclixiak.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kblgxlnq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbatwyt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fsdogmvc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vctfwcoz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uuqzoivp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zcotdogp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmcgvheb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oxrbdcki.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdaubluh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2acfywzjv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2onvzariu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zeamovqy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsigdjxl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ubwsjhil.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pptxcvom.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pvzfihqa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dvcjbfnv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xppdqyld.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ndazwimi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qzjgrpdm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2purcauby.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfbafcws.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mbvklgah.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnrgiwkt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2oazichba.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvavvzdp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggfandtm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlfmront.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yqneeovd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qgqwqwob.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xmlngjvi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2seiohqoy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2piiifhkq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fsroxdiz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gpnsyiyx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aisnbmfh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2efsibkff.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucwotdzn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2izpenwez.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cnxbfump.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2voxwpzyp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dyndwqut.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykewnmgh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iomzsfvs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmpsurt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhrbbcor.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kctznbsw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lkkexugb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2omsisxzu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2phzfbfut.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zdapgpmj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2agutgrjx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2czxzyxiu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ngtuqovq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gtjatnwt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qnxqbhoi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bqggbehn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgzcmyf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oezgwlxg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2opkujhdb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pfzigrll.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vrnzcjit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2euulwmqg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dedudugd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ohhutjrp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ufkbkhro.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mzklzifq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wuixvghe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2syuazilr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kvkrmrrs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uythetep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfbwkbnw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fpopvpqy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyizrxzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cfyelgdj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zzumbrdi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hetvyxub.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ketyvvgd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlbsepjt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jshbcfev.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmnkuyf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2eymapdct.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkarenu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2szccfebq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fbeofymi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bifmqnoj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ggownzty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2uvbwuwmn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvzxnla.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjjviwtr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxkyksv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cxaagwuv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqtxzyq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ynxpvdvt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ruujrlai.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2umcgzfsn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tpdbagut.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xxbnakif.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtltpy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sfbzpnih.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2soxyrvlq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dccmclue.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tpolyimp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sxhoozti.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xmphuwrv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgsbjciq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cfzwnawu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cxqzrgxh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tvbrrzul.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dgsdkiov.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2momyjmuc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zkvyxpot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piyzkvtl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qosedsmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgpqsfvd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rsrdojvj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sijebrwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjhsdmnn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2giydsqxt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2clypfngd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bnbbbgoi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2utsmcnlr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2begfhftv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vahtutoj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxxarsza.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tbxqknjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wosdytsh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bpcbyrqb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkvewfen.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2npodqvgo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hvkuhvum.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2njkfxslo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sgxrdhws.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mfinfylw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2przckulz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lmhzmxvm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kelqeica.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pogtthwy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbwiwspj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fmwtsuev.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xhsilemn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2grqqokay.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2izermtln.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2majswqjz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bwtafqch.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qlnteknu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2djeldpwu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hbdzcfct.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vtamumta.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2swamddlx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cphuvzne.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wxxhlscu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lpyevghd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rmrdpjpn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gposbjjm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gwjxqtre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kwezopeq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vuzpuuwc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pydkflta.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ognnpsgs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ftlqgecx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cqdiukzb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2miwvuqye.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ucdfoclq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iovlfaxh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zsbmsbsz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wcqrbmpx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zezykvyl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2omnegwew.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vyyrzaxr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ndngrshd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfpdhhkh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2eldhkjjn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzzopzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nwkberph.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2psizexng.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wvilhlzn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tvcxvgfs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tkzebjyb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lwpcwdvm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2svdsjpcs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zotwzefy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lmjefsbu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2smmtaozc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hhfpemkl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zruzjlzh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ogxzzczm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ittgzgfz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uobvzmrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xmmqrmnz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wptmfrdb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rzlxsaqk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ixdtqnwt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2atvzuxcg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xsvsnbfn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ytgkjemc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wgkkwynh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2raaoarrt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xytqsvks.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xslptrgq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gsdyfwxc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uihnaaiq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jwbihxvs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yszighvx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pxsgklzz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pvymuuye.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2eieuhxno.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yyjhvlcs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bgvhzknd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ecvbsxsw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2evtgcibh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tbmgfmcb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tupignfs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wdbdhilg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bjdnscmi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hitjkdvv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lrcamesl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rgrvgtmz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rjfvpqsq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wabyymde.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ovqswmse.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kwnfqbht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cpeuuufc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lwqpkoue.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fmfyfzmw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxclffdr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lpwhvhnt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2poweydid.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixxzzill.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dwthobtq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qpcmnjwq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hrvugxzp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2amwjcacs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2soejwyed.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ipfkeori.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjdqoj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mmevyhdg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nzdgisry.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2otytqwro.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2krncqjyw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qoqbkjic.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjubkhpn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lhtzlwkz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ngrcmecn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gdvjqtec.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zpimotkx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rdqbvnin.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jpeeqhoj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2afrmdojh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nkjtdjxh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qwbimwig.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2plqxzwyq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pecxjjkf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ppvqlwqf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eqbqielh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2agbzqwkk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bwaqqpfu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2okvkvwyh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lfypldij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpcemgun.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hreesbbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crmeagjk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jxyawvld.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zjkvqqhk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gccvdefc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pzckxkdf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vyftygqh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rdirkeyz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fvikqmkr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ogmscewj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lypxyygt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jkwxxqgp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gdznjhmb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bcdaioyr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aqfvokxh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xlwyxijp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hgzvzujh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lctifdya.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjxrzgv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2myyzdwrc.html


<!-- 参考信息 -->