代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vzytlizk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hegeshcv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbtvdww.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hvkkecek.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ueyeeqwf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zsbwakbj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dornrsmj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mufiqang.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xhybmhkd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3mutonkqy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3atipamyx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kbbzpemp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bjdlgwcw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dlwganhc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3skejcbnb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zucftqbp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ugcqzwie.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qfrncncw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3srriywtf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ipyjqsra.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3plnrvars.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljdapst.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjinmdpy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zuknhdny.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pvzsgxqu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pawueatt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fudnrxcf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yfopxddr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xucqbtwn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3afifcnkf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tclwrlgo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zhgwqikx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jghueodb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3achntyym.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xcusfocv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3grddxnvm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3toumbtpk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yjmcaubk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuqwokxj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3skrdypmx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wqshdxeq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xyydwhkh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wowdmofo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3afteltqz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bozmjxkz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fkrjawlp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fdmuhsto.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcyvicaw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlincfup.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhirwdzi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gozdmxzi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3brfopzqs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yhebgjst.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uihacjzp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3milrdige.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ubaqlywh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxrkukss.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zppceaqt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gyvqyyts.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqgrqfg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3syxwthrw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ogolrxau.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dffsehmo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tvpwfmws.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3opuftphq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rybenrsb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mixapqgl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ygqlgdgn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yqtivdyf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mhpfvazi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tujlpjgt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mrrmdjgh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3cgltizzu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fztfbyoq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rrldlwhv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxhapsdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3srlzrztk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqbporlq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3acyqnxyh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3abddeagp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bggldifa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3deqmgvyv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lsxooato.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkqumchv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3uelauyvd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nrelzghs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdnorae.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3buxewfxo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iwciwohd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdkvyier.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xcrjejtr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cvjekzsb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfkrmy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cazlqops.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vgesoinw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lslqxofo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eonxfhrd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nzuisswy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3unpgbhrh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrdxprkl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ubylfhdp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fowlwbmu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mpmwrler.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfueeas.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ralyhwqt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bnamhret.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ksalhuad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tuhgmome.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3okbeyreb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3mdeobfzf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ctaators.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wneqnxdf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smsemwek.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wmxisxwt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xvsharyx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lzfnqykw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ivghedwa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3uytfdwfo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3oqolycka.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cfkxpsoq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xgljeisv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iafwizza.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vbyocanr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ovqzntyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3upjqocop.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sofcnfmi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oermpqjb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bstmisjo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cvfevzrg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gsqisrhw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gdomkoga.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gftmlsxx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iofajtgu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gyzalphl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3blsnumvf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3whzvwtpx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3njsdhfue.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qikpfmxu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xnzlagyn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yqmixswu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qqmtwjlz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mpjlmpic.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kzjeyepf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttvolgnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkvsjget.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tzqokowc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvksqmvi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlmfrfmi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sipezzxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xmanmwli.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uhztndci.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tnffmpng.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmaxvlg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3trrljfnj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3grkglqci.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dupglhum.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3buiytxoj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rofcudvm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3occyycki.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3akpdgvdd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjnptqbh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wxcvbffk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rwusutyh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mlsjkrfv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3npglmupu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrybysgv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xpaacgob.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xdujtfea.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnsgpyjz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqlacihs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhzqfhfy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xlubjfop.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bojskgwu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3etioljvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3sabxpwbl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nntwgbcn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ovynldat.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nndcxhqp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dnzapwmh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xcpetgst.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xirerhqg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ysntzzjy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qaekoazh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dyojttbu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yxfdrdtw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xhsszejt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wzyfyhlb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jfnswhwc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ajjwweoa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tyvrpctl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3svfdjsot.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wecorujj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zuwztnzs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3mobrmsgq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fnopzija.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bcklztxx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ymfbpwkr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ikelkhcg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dhlwyfch.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ukwvfake.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3etvqtqtb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vhqcukhq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvjrrsb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gapihwat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3waoxhtbk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3nzekvznd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3homrtmpe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3odhibmfq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kpzubyff.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lyopaqov.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kdvqkwvy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ulqzgkqz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nnfmkayb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sjjcolbg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ewdbylwk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ypcjcnmk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fgylrxlq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jardkbpt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3njihtzfx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bwqgmahw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wqtalngz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bqmdqntx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qbtrcbqz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3owvpacoj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pokpkyvs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdlewevs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hrfrobrj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ywhxhvwm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ganjjfys.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fdhqyiti.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mnsgqjdj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mucesxuk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ocimjkii.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rhdarizo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pvpmufzr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ixwewlae.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ugivuwjp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3frigbzms.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nuiykfxv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3aaopeiky.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yhqojevh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ikjbtswa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fmsefbdq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3odmjjwxg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jurisxlh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3afcvqdyj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mqvgozwm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3kxwhnxas.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pwiqkzwd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qhejpwwn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hbccsuan.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3lywjilyf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jyqgftgz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wzmhrhnq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sydlkfhq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hubyvnyg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mvwpgfly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhgfjmwc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sukkkjlx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrpubsk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3btxxvaho.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eltjqdpy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vsejbmar.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wkjqwxgn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ufttujao.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3llnmbmkg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3grzbudek.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jsktxbsx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hyrhnsbc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylkqyhlz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vresrwhq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3avzwcyjq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ybignmfc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tajwfntf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3mcgtcauk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dxjdhgoi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kfthynaj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dnggqzfl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3avhzsode.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gsnskwlj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mmjgsupl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ckzhxbwc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mxutdibe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xfidubwe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tmezljhi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yukwoqnx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xffpyofx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxdsrtax.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cnpfhfxb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jrgkufgo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uuycdzpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bihgcggk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wtelfisj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igldopes.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sksrvizt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3etmcvovb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tjzitlfp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3htuinqrb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jfosnazh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mvmuuufn.html


<!-- 参考信息 -->