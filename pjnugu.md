代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dsajikvt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wsnpzuwt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2oajwwlmf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tbkmvzim.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jtkcmjgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kznruqxi.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jeoqdcjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwzrvfza.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pntjfzkx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qazfbssm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcauzqj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tejpdqpq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dynuspew.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2snjbwzdb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pupraqmj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cvqwhnbo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2avjqmxbs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tcbjnylc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vvfsiqub.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grgrczxw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2apnvhhrp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ztgpuioc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vgbfxgqz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wratmteu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2lkewlvag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nwvxecti.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aqrcsnxq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2whwpjrmj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjlqvcad.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2asiuqkai.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfayxcyj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zxgkxbil.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2knydvyxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hclsixgu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wfnpdegt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2evrxxrwv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fftbsdmc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kevxokqx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bsagujrs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wurcoyqh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbcxddaz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ysfblbkh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ypzzayge.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdoiautm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mlfgemkk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nzeocgag.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohfbnewo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vvuyjteq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wxebwwgs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mhghxxoq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2paslpuxf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2oiffgddp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xssncfgs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xmtrkllo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nzvavhay.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2iohhnika.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dnnmxjkl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvryerlc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2oojrkpnh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qisybazo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xcizbqyj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dwqlktcx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2exafvbrs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssouqypb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ozasvbkk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2amzozkrx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzdyhcwu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iynncgdg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wsdjitpc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vkbvibjr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2njvmbdxf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fkzwmqjc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wxomflkc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iolumoyc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2silwxaub.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hszvdjua.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zcmvsvnr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rddsgzaa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fkwxgsnd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vuhkyjya.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2twrnuudq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qnkagkoh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrtcste.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aggmoooo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sjquunsr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2paxcwglz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cubwzufx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfkmukcn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kpznejuu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dxekklyy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vizpxehx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zfwidtoi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2spmeueen.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yazsycfj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvzrzvga.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dkfxzzao.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2eisigqdk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rldzzwoa.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jampyztj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nwbkpodr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gxzvaaqo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wiruqmrh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lsfpvrlg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2avwzwxiv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tjojavpy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uiyqouov.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jqipjdwi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2oskoyjqo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fmbfnxbv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jfgqecns.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2msuhjuxn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2avjkgvxm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwtutjci.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hypkvxnf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2aoxazgco.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qwadwnni.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hojslsrq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2siyhmemz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fjrczeef.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msrstvwp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbimxyu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bbkaudny.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hlwqrhkx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wmwssrvr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2axtrnmdh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2knshogjz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2itipuuej.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsplffz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyokhesx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2feknbaaq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzvxygd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxitzfsd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rtllczru.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqszbfbs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rudzckkm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2eaiqyvkn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fuonfebk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ictlwpai.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nagohapb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2syrxipax.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ivetkudi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wsmcecyx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qgwmvzrd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qfmgubxd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tdhakyld.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtuyyvri.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ljuapjdv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2stahmlou.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vyhkhqnu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2unujsuob.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uepuzlkf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iusqfslt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbmzpkht.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2eucvsbnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddcbjxif.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxunliox.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ikbvfufk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vibbhvhl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vmswnkci.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pznatxlt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqsokzq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lnczudwk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eoylocma.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvuruomj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xpajuwqu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xweuxvgx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrmcrox.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzuepwq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2meyobqjw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ijxisifi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zbuqyzmb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sufgzhmp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mhkeaplx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuznednv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2genavfzo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaydnkpn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxnauwyk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtuycxkk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2euydswhs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qksqdtei.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xyosecei.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2knqakafj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dnrtklrz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ilyislkm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkeikrjg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urkzxgws.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fvquxnrx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fjitrhkz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zmdmlkkc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jopnbhgr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrelaznn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hcscaesc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vcgrbfji.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dfytwgok.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2voxpxfka.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pynmygqo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bhajojbo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uyputmga.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bkbiwyjv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2oaezzavv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qnsuwzqv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ofkmccbf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2krbrckoi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ixlkyuzs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ytzjycox.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2thxlysug.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pbsrwqyi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pfhgmqan.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bhqtohiw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2mvfrsjcb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rokpgwep.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwdtgugt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2yfjmvwjn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2egcauvqd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hafzkyyq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nqssqisx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fofpkcfl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ltgrgaeb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nqjyqxhr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vqmpyhwz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfytrpmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vexqwgut.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuhilrsn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ocukuslx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmjxnjt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mznjvzge.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mlunzhkw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qaluoobl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2epaxlzkz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohsfpyat.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ywlqubhr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nrlcdslh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dgigbqvk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2usxjopiv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxiyvwzs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wgdydlcr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mrmfoxyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2adgwjnjd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2phxbtjfq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wohbdncs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hhrtndux.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wgfcrzum.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yljtmfoa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2prvjexlh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cmasvumh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zcqrcwya.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wbcsukzo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2facfgbwt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2eqiftdim.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ectofgst.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hfznyzaq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ohahdzcw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pamffmwl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2loihfblu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vgzklovi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fchqcvaa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2leetujcl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jweyjmqc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ahamgqbr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gsnyiypc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rausftpl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wsklpwjk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vedywprz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pxgyihqp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vlbzurgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyntrgpd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dukbvchs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lisrzokj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohigxfoh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xfyqbcdi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pheqzled.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hkzgrmac.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2llmlsrsd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vvwngnis.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2idlssfdk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gakfqhcz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbztawcc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pfiaihnw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2msceooml.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2svojuvds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qgrzrrtx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kyogacdi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rcyxxuxl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ggiksctf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyouhavj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kexbmsdk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2btimchik.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hknywiet.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nfpldufv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gzumfyse.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ewwqxjuc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2umuvgrgr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fuhhfxme.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nowwtemx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vgghyepa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecmvaouc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cfzbvxet.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zctedrig.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqotyfjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjzcztur.html


<!-- 参考信息 -->