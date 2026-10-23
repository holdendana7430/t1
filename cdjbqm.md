代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kazmlhna.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iqmfhftj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tleoqbkq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eacksyzw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qfrpezga.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qzyilcnf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3abxuotku.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nmeehaky.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ulorjgix.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3uetngdmc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sjppzkcp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwcsnxdh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3imcnklqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rbtfvitt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tlaaclaj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xcbcmovd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jjzokfuy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ztiokjqt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zjvnuckf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nnyafkna.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hlpwbslb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3folwzxtf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyzqpcma.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3graltktc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wyeetnlp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hzmhgopi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cruqfxrq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yiqqzwbu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3btdwksvf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uxxwclyt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibcuicxn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eulshsou.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xrlrspxb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fbjwfmzw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3sibvaqcu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bpsklhdl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yieoeuty.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qokejwmy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3orydjblk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtbnuwi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3adztoxyj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3foxkvrar.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ohpagnlx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vdttcgpy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvwoujgy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3cgkvqper.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vqraqhfp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3egbllhhu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vbynsnrs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qcrvnzyf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfbrlnsz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uwlvgssl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lcotloax.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lkcwqaam.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kiyoruxo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ngynlbbw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3euluetto.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3txeflqxz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwhfalp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcmwmviw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3shchppax.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oodusbqy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hprvucxg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3iomuvjym.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ewwvoyqh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vezgzxru.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhyylqyb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xcoowcbj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sqhxjkdw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lmxshbyz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3equorfxh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ptpnilyh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3akwsvmcd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sdvsgcvv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zimquznr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvdaxzug.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3irhuesco.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ddmrxuic.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3urxsqemz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3roiyidxm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oxfjxhda.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3knihpjjo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gxocwhxc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ddcwcsdy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ubzizwpe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3anpwyofx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhseemsm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hiltrqsm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ptldsdmt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3rabskuas.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pgyaytre.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3yjmlhrwy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3snubgxyn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3quxryqlo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xztfzmox.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zdctyuco.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3smifbvhc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rowuzlvh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sedmzzjh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hvliqosp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3twtxpkqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hwkiwbpb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmmnhoc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sjgvvyfb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3exvzeinp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfyjmrga.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kjasgxie.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3agxrukyd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ywlfaocf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3eytzfmqh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfabzvt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctozotwn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gdabdmld.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3oemcjudb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xxepcbzk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cifzvkvj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yifrulqj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3usdmvuhb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dneklxxz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xovczcil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qpldwxpt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtxjpar.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fufapjqv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3blskigfo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3swixzqsv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkcdbpqe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3noccrzhg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yqbycvdk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3knlpyshw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yznirmei.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kumjziyz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kobpewvf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3heyjvwgf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xydkpjsz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ashmabpa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3znezamgx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dhangknz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kmlnidpe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aqcwbruo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hodimlfr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pmqnyokw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxerwos.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3nqwafbje.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3puddoucc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woovvhjn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hrtbebza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leypgukn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nzzafkod.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cozxmqem.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxtcbdhe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gbvrwarc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nzydrmto.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bfppxjid.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3auzkmnyj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kqigierp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ilgrizxm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwwacinc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kyippani.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fznmbjyt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlbyyosg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhqggiab.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ngwsxrnn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wyjzqifc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pxuaancm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eozmdpse.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hlzprspq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxxrxga.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wrytvjpt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3iirperkl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wwnrgzog.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvsufs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3srzuuogs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kcsvzgvf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ggtyqroi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ytfjnfcz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qeipkppq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mhmxrgww.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3whztknmt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jszzbcui.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qtdrnjdh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dbkkefaa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oescyaao.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axjumtbv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3puwpwouz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3foqfuvua.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nerhfjov.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iyjqayvr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fxwsehwu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bkskmqqr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3elsucxwj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yukdhalt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wdaleahh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aofynnmc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3psipujpr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wjggeznz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ahxbyptl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jdpehdfy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uygcudis.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qzgxwkwv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qvuablwn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vyxednqh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3etrmtqxx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dioepdry.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cinisiat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3eqcxptot.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzgajqt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hjpjjzbp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fiwscidd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dmtixswk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3cjgpdzhv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rirudgiq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dixgcypj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tufuwuts.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmoqwwv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgnhunna.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nrafdnez.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3akocuwca.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lgdbtfmi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vijoakuy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bdxvyzoa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwmugfhc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3epfjsaib.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xsefluji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gvpqqtqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlracos.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bfuzsnwi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rinsdhvv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3biwkchpt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lohjlnsx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ekvihtfx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3biusrexs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gsseccxq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3szjugkgg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3exoznbri.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3erxqmniw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bsugpwib.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ctiqrwvk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dlhrtylm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lychxsya.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3anzsrfra.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xycseuvr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vfkhnfgr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yurdystv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3csavhiqz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jhkwvqty.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tfaoxpta.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yvuumxaw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vpnoizza.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vrqlrnbv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uwjemfik.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nrewmskk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xxqfmvqj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3boklyoeq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ohkffwdd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzdxwwew.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zggkgxmw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3yrknqkwz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lcyrwhyi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qkvecnds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gohkpdwk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbvfysu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fbklpmmh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3titfygku.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3aaqkqfju.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3snziyiek.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uvvvaqza.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nompuksx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pizffqmm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bmrrictg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmvxnot.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3psddtjyq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3msglacwg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tjrtlpkb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fmytdcez.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hrjabrbw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ovlmkdyn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dixzgduo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dcyonxmy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rnhikxmb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qfyykral.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rehzwqgy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rpkdnkod.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3phdbfrsm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3crwspyto.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fnxiooik.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ujruntsw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uydfefof.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cwhopyrw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gunvybxo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hyxpasal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3eyyucbna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klmomjdv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sldarotm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlugacqj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ifvpwggq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wgetnlsh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fvkbdffd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wuqxlrnz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gbtrlpmj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mnkvgjpg.html


<!-- 参考信息 -->