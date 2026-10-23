代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3umofqtko.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pkyoxciw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pbitlldg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jpgdjeii.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fozttjip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubsoeyit.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ajtcgaom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brnhfoqq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kvfuagsl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rlvpdlzb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xvlfkeam.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xtdbcspx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ichqecfo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nteuuilb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3clpfnvwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jeuujoli.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mstnbtuw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3prbkvjep.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fiwyqbha.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ieleyvug.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3daiufocx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3axylorhd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3thlngihz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zljvyazt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xojyrpdy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3alelsnzv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qlytrutj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmvhzs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sazuzjfr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahemnxod.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3heeftqlf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xgqzvkzs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vsjskkye.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3glocuqzo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3spijoxem.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3udemovyl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vwhvvixw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3olxjqsvg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kidwfdgr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qjvzdtpy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kschrncx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gsexlueh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rgiwdnxj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ljfmlxpl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tnjmlmim.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3uooewtio.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xckeywmn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qxveabgk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wrzeqayx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3phftyzck.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdkaviqo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnqvqou.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3iynnvghc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dgvnnyaa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvhccag.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pmqsuccp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xtaqovzs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zpeafycd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqauaufc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qswgnovh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iejeofhz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cqottbyb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sjafdtfw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bzrmojoo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zxteobbp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gnjmqbmi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uocxbrpj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lribsabk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3drsigdvz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zbdsadoe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgiaxwqx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qxnpnjgl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zcjubuvq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3okxdrhpo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lzjfegyw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fhcuynfn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tgngsulg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zohdmzko.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3uvixbgto.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qlkovesh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qpnmotmy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbacsvlu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3surgsjhy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bcpinpwd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwylfui.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3srruhczc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqvkcru.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3csoexkqp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzttbaog.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3avdcedne.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3utsiiexv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3phzpmqxf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aucnjedj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hgomamun.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbeyanjr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhxzogd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hsfrkyfl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nlypchrq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zkjlckfn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rihdcqyg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3biwwzusk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bsavzpat.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pdoixmwk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eyppvmoz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3phgjwrtd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nzidwbow.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fufiuvok.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cnnkiwxl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xaspitbv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3oexacoyz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvnoafdf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wuusbvnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vdqglcfe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jvuhhgbx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nzkgwfpf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uqixjpzm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hfgzgphx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vjqexgnb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wziqfyuw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yoscloui.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwkxhoyr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wxxsvjkp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3siumnolk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dekaerkl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3urbvqwsk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ozxksooj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3oxhfpmsc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ohslijjp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmgdpqb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hdtpdkkp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdekpqk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bdowpoha.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zgfzgfqi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3puiygtlh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ymdlitdx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3arfcvugq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bvoyezfj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3llqdxowt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bammrdqn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rluvejso.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ekxwabvn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iglcqjrk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3giuqblpb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oghlnjwg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ugmflwgc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zkcwupid.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fnxpgdtk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ldsmlluw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bwjqawhw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hatumjxk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3muahbknm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fsklqnis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfqzjotj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kwxolspm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqyyshpv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3khzzrhdi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3rjfttoqp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tygwajia.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gwvppcng.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tapmihom.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pvmrugrr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3efibdfos.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozgkuxpm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgdvpbjd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3erqmdtni.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3eiofmski.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3npapbvpx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3laowyeaz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nbngutny.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ahggwvqd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kiaktscf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qytumjge.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ipwezzwz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pekxaaio.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hlbrddnf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hblxhgkg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aftpeuvr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqyqcoek.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyzzrdnl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3djkhqltq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gokqccrp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zpmeaitf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjelumac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3unebqpab.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hxfndgqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejkixpup.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uacrifqj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3giylqqql.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wcupyakk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3utdufjnw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3egicfyyy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nibxfrrc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pengfszs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mnfpicvr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ggztgtbr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3corvrqqu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3odwzimfa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wbztuyyh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zfpcxtuq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fwkandfb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kfswdtkl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pbgdxtca.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yyyxxeim.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3siklpfdb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qslqjoqd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uketohvw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wkalvdem.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ciygtato.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gxiackgq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gfvexnsv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dweikhcy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hpahkwez.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zfexetvf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qmrrsiot.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3myndclxd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3otqvscau.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wnlixqdt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3emhfnqof.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rxvvslrm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lwexvvfi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nibrchqt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lpsnigww.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ldibmyuv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fgqyxiau.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lfydpetj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cxaszadx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgbpzebe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xvvwgegq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wfsduswj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyskjzni.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3efqytiee.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yxssumwh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hpnezfvm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fwndqedy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qjscbfqt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fcxhblqk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3efbepbds.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3prsxzgfy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bifcpgmg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kkcjiwmx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ijbnhabo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3esjtaapj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3avrtconk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3epudvgkb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldbgqhfx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3reknzfqb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mixzldpl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kpqhxhch.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hdtvlnrf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zsjvlyrt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rfxhodom.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bvilukgv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ddqmfazb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ycbabycj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ixiktmbv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nzlbpdjs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ajiejkzj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uwzsnxrv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hqsshcda.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zasucyec.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rnkumcnd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ztlsettu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kmyridvr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zagrooue.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ysyibpuf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmeyzzc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zycpymra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xtcayocz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzngpsyj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cxqsgybs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3byjfpmnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cjxykffa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3glfrgrda.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ttzrnqho.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rbvnbhos.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3acwtrrje.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3grbmsgnk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jtjoxdqy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3uymhhrne.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mepkrxzn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3dawekkxv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujhayila.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3lgrdamnb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ofbtgkbr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qbkorqsr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bljomsln.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ypmpigya.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3itbimcur.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hyubzkhw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jgfepqbt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3quqoqpop.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3izvelsxb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zhlsiczh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3clbyorvy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3globuabb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxctcupy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ajnyedgu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qkzbobde.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dknttdlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iggacsdh.html


<!-- 参考信息 -->