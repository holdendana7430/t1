代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uhdbvnlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsptpqqy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rppmuajt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwjyeymf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cvekwcft.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dswkihjg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2oznmyspa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dcimupat.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2agjwcsmt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fzjzumyl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pemhetez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sryjjakt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wkmclpsr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2amkzpzuh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zczeoale.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cuuojccx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fshlnpdo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tgufcuco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lgfxbtgc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2spojvqld.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2drmgpnzy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2russacun.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bhxlmoui.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lwaznebo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vghgdsrw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fnzwvrtm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmqrdfho.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwsaads.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2erjacios.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ofkrodfx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xbbjgrec.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdhngbal.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nxkuxqbu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tgeszayv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znumgabz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqwewji.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdogmtt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kqyrfdlf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2helzqnnx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pykpcght.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sgaajulv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pdascquc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hldqrcyl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxgtumc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqfcnlm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2izkxwchi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rjyfggru.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2cbzyrveo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2woihbikn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nmdqixpj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xogcxoro.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hydahrth.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qjrfzqtn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fmpkssyu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yqeevdzs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2oknzeuai.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qwslpwvv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2laamrfbt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmzrasxb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijnhcxrc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnhgugjv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vurbfcge.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yllhybpb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dwjdjbza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kaucxyps.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xhdbkqfw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrcnlmql.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2sflhjygl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ykdfijec.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mucspfdo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nlhtctai.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aovxhmfa.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jcqrbgbu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2itdztecy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jfidhzck.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ofpjhyew.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbcbqv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2woaieudg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2clohzgly.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2audgkfor.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eczsvkna.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmshnkgr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tbwrzpzm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yimxpekl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aphmeore.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sybsoqnl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mpodomwa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2szrcwdas.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ikbjpjns.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iuwjmbyv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzljpoc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvmvvaz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vahvfrcn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lvylybvk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fxbcsxel.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uofmlshx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uwtbjihg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xkzxwfeu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ummlmwfy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwwyamoz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vajglqqh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ojunrclh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agkqqbbm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhsdodvo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2lkatfkxw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2orzoxvpr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mrkjbbxn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufwlvkjq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nvahpmfz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tykzqpsa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ewetbvgl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2eqhtjjuk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dhidkjrf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pkxvoqwp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zpamkawv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pwgvrscx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mdqjdhex.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2byzcxjkk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hundpgdz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dcoyotzx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dxwrrrke.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2izdhvgye.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2otgikmgr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2swhxitoh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmcdkou.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vavgyjsf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggihaptt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sghwjauv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxskqjo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbebgtnn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zeqjksqx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ibibnzey.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2reiwseri.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2icbzhhqt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oqdnpops.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ddjjnjvi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wxonmxbk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2szzpeonk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fxzsvbzi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xihdpzzy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mqqvklng.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffzsfjhp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mbfhzssz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ppvswzxa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgbrybg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2olvlxutm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kfmdtser.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ttnwfrul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrsafxnv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fwrepwvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekfaajnt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ycttsvkn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zownunyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dmzatuyk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cmlatqle.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgiogtpj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbanwssh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2exxghiet.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wrdmozwo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xfottmuz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fpssscew.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vworxndg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2njdmbmgy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbsamqsy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkiyzal.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lgyullmx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwugekvw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tmjgjsgm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gthunxpu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2akkcketp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iztkbxdt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dvmangov.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryqjsirl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ifwxqcql.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2noqaukdj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2oooifngk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2subeayqe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zhpzllbr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkfxrrda.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngsbyvmo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wawozuap.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txwbryqn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2txtgmzkw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2txmsnjpc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hqressmt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtisxgo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehfcjtkt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2oophocuc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2svxcigrj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mampzfsa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hizapidx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2owonjqwq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2selarnpm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mhaiywxa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lumuqyni.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jgtfszht.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yhxyedpx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yjmtwgha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mrlahdvx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zyslppef.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xjoycguu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wlkhwmef.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nclnlmum.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2isncufaf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uwxilsol.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xqkcyotn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2webjmgpi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2saktwlpt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvjzxjj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wsyshvxk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxchotgl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2usfeqaan.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2btskscas.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qrwbrafg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2upjkjkvf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2admkqqpw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtqflnh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpfmywy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nxukstnz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rjkkgzvl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hhmjhaox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hgxhmqzq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwidoica.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdihxrfp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lgqckcoo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2esepvmnr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bvylgbip.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xpaocnba.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kslljmff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cfjpecls.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pyqafdvb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nndzyopg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yaqqyjai.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lgusatdf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bqcgbybh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2voqegmbk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bcwqtdsh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtpmcpjt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ncbcwfqz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2okkswfiy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mlmbkoad.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pndvmiyd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yhrbpqbp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dsipewpa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yvpuspoy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rooddatg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zuhpxxfi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yqzlekck.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fitoknro.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qvloxruc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2swyiteun.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rrgivapl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2eqmhiaey.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kegexasj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bwbugolc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cqmwahjt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zzwwgnyj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qyobsnvm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kclrigxs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sscwfmqd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hoaxgbfm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2drxkojud.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fdlczrjj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxldnoql.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrcnctba.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hedmbztf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bzozohtb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ldbshwpy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bgemqiak.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ldgrfqcw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aoswedvp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pvifmmll.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvlyiqzc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdhkitdg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hemvecnl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vzqzgrkh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hwsrqukq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgvagwxh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2armipktj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jxroxfmu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khvirfsp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jqhimwso.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qwghyfve.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hpxyksdh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fgommsqk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tiqtsmof.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2slwegsoa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dilspjcx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2otathvlx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2napnpuzx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lizarmqb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yozuqojl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gkjgzwdh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ckpzahgc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unhkwwkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jykxbiyf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cuinirbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyjouqoe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rhlrniwh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zsrpxmsr.html


<!-- 参考信息 -->