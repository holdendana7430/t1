代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dygkuyzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dilrtzcf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3iarrpslc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mubsfqcg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jzyajwmz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ynhcfjth.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wphlyoen.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3txckwzex.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mjwmtlbo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jbefrhlk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3uxezpdvk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cgvcpkkg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lcatmuwj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3upszqxma.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pbtcjcdo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vktxwlpf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3laqgreaf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gqtioafo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xnyeriyj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3tvlfmiyn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ixlmarut.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sajvezje.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nnocyztn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xxhhmhtn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbvnhkxi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uylbtzgf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciifrgqb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdgztuyi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fgelkdif.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ukcakzax.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kdlwcsma.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xvpxaqtb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3txbginbq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtuskrwa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3abhlhngl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmacsgm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3baqsalei.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bttqvpji.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tcrrvknf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bujwmeqh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ixtdvxoa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwosnui.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnqkhvpg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ptgysxxc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kerfxikd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vtpqttdl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gxpdujdi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvcodvk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlawyzbc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uqdkixjo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xkfwszce.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrsxvmon.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3drcrfjdk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ofzmryli.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wtpqingi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hnxkhvny.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zjzdzwdh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3diatznor.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zdduuxwz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ejzevldv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bjplohxo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeaiaoxo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wasqneqy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3huwcydls.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ztexymhg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vsizbtro.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3buvofavg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dolbstdv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hpskcorg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vmnkrqtg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wwedgcdh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bumxkxif.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zdlmhydj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3drqqceze.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wjwzsogk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xqbtizeb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uezwxznf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvmakpsi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieohvwaj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkbmwpdo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbusbqnj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3apbbifph.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tvidajes.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cslakpsq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fbbmlmov.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nafjcgbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yonscplv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rntkrqum.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sjwdrzar.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zgkyueuj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3goxtzleg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vtunzjhx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3pktzhbav.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3primbmnb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gxqawcfa.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fmtszudu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3szadjocz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3llfibbtt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkjqseq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3romhltdl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ynhnnelp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nqssahbd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxinuak.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ixxpzabr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3aqauqkbe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zyrydcar.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3evsxezsb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xuyznajs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tafmwlxl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ijwihpyd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hprbrqcu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ntolmrky.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3smtchlln.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3lamdbllz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3znjgymyk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vtkoadvp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nibwsxbx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3swixeakc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3scctgsqe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dfnqrjmj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tdbuyjsx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3czlmzyau.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gdbqzjrg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xvewcthz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrfnldlm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ieadpsdj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwxwpfqa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ceoirvtq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcgjpys.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tcsfrunl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nqnjdknf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3etlrexdt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ymufurbk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mihsbhzl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fdrjpool.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3avmwzlxt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mbawufcb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3boknnkef.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nnvyxmck.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sqtyavjo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yzzugdro.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3julmqejm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mqdiuwpp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uzznzfxt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xrvpyawa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vtygujgw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dcegdyfw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gxbahxgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuklrttr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmpjaziz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frjfjpeb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3doeuaxau.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hddkpyjk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3maajwquk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxbvhyzp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wabqcctw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkqcviue.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xopemjym.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rusdzrtv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3szzdvszu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3amseikmq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gpmdijid.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxfrmjjh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkfgfpvx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iavtyuuc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3skyueqjx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3evqeokko.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vxwonpvt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qugqobuu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zlamdfqy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuuahea.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oxvnjzkv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3higkfxsx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jdsvkmlx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vmnstvna.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ieodgaak.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqhfnzjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xfifdbvn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xkeocvtz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gnlajhvy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vifutdwv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qhhwvvez.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gnyqoxsk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zivmakti.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nerphgyp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkkaebg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3irpeinqe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ysgxizju.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3plkwayef.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gijatywm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ybzomycq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rhpcvkdl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tikpxppe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lhqppsvd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3farwqyda.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sqojuuok.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eortmtlb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kxdsxzbb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bjvumipu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xlvpebog.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zhqxnbkz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3brvzhdsg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gtviigaf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rrbohjfc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vrbgczsb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3szcodsdj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzfkbbc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gncspgmb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mvydaves.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wkrtxvoy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfkkhvgs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3imxxfcmu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zpntdtgl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vvmoitgp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3iakfaoao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tosvcfuv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gjzzhcla.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mkylgnyv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bysmwabm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rsmjnfmv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rnccxvuk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eaawimsi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecrmsbzj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dorjilca.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jatvduab.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwujkvjt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3isxzabec.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3canisbkw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfoahmoj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnaxikze.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlegtshc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zlaunxov.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3piyjsyxy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fqvspxvt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzeoei.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ixtzbqvy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kurjucpy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3isdinxtm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jzemfuit.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wnyuynxu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yhljchke.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rliztmfb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rkmqnwfu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xkkyctwk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3khsmcxlt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3whnofvnr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ectjmsll.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lohekwsh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dddmdbcj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sgrwurlx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mamilrwf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bjjevbhe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wzmkzohb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dugzkipw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bdbeblvd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ccqrbmgy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gmqishfr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zrrxbwth.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pulqgncv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kxxmjjpc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wmvfwjuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdyojruc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3gjvjxody.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjlcnwnw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bvsasweu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tisziixj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qzxajvrp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3aoloywby.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jksatzng.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qvbrxaav.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3osomjfjb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mclwkipb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqaykbc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3skkmflch.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3blitgcfq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3roptgbgq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wvwebgqc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lqopjkpq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wsidhwna.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hitrotli.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwdqybmx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcfqvqvb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qnvcggea.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zsehebsc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hifvpzjd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tzpnmkio.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wswxduzw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wusyxpdt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ogyopnig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mnedmtfe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aavljxfo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sropdzvc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wtlyqhqz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tuukbwvh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3aonwenvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwqidhjy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3abjblmsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqenqeky.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lmujvioo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ykvgirns.html


<!-- 参考信息 -->