代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhjsxutw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/guxjdfbbp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fanxiaobao.xyz/Article/details/gxamqjtoo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtynddwi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbddbatc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkknzgzmr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqcdknxq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fanxiaobao.xyz/Article/details/gcatdhomt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrkygexh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/guloiklao.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/gsngiuyjo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvyucial.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxsmhwim.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghqkbptgn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gratvxytf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goeefjkwd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gukyalaib.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdquopugj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxotihwr.sHtML

[B04] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztudiqra.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gacewsupg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvntwmxzs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiaezpnv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnynqcbsz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfywozhiz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbuylslok.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fanxiaobao.xyz/Article/details/gniarcqyv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glxszrgal.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gymzipoxz.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/gztmdkcjk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gliqwsbiz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdtnxxlz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkzznron.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxwlltkp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmbswik.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmidlzav.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbseaqrba.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/gtmexspxz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/gznodpaug.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbewqmbze.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxpohiix.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gognfptin.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutmraidm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnmigtln.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgfledxg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfpyinbf.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmhgygme.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofiauuzr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghkxoidly.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqvkcnuuw.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyofvcjdw.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/geuxgfxrh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gzzydpwyn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gfcrzvcbu.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnjusbnw.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/gegprszoi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgfmddpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdypacx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/grwvfgkoe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqihwqwb.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gkkanihnf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszmvyyh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gfymryfyd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gjyqinstd.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwloatpjn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdbaasn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gngotorls.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggdipeafo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gveupzimj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/goghpccoc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnozvswzg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuzqbdtl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfbjnrqu.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyhxoatq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmeidzcf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giuwdytlh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzwtyrts.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/gckoapqzu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goxvwnkny.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugrittvp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoptcmad.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnualilqy.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fanxiaobao.xyz/Article/details/gfoyowvbx.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqcsflgr.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gnuhzowaf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkqggwnv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gypgqlmfu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwgrayqj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/guizuyvnl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gqtygmezx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gyesximfp.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gqaskifbv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gnruxslnl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvhdzkou.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfwjxddr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/geygynqno.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxyuaowf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyahgbdlm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gjvhazpgi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstkboofw.sHtML

[B13] 判断是否为数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyzvagbc.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gvwromggy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomsfczmk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbiajciv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuroxiqs.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/glnnyyeoh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fanxiaobao.xyz/Article/details/gfftfalzp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/grntohama.sHtML

C#:   x is int or double or decimal
来源：http://3g.fanxiaobao.xyz/Article/details/gcamnxpni.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gljrcvtxa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdesjczi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/glfnsuzxq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/grfupxdhk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbgxuwzgr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gstodwqgp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gotstidwo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvltcwfc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/givahdaqi.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/givmubhpo.sHtML

Py:   a and b or not c
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvoatng.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gcxlroeoi.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaechood.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/goqlrthou.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gsdvjbvin.sHtML

Go:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gaddpkknf.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipjsaki.sHtML

C#:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqbmjfma.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjvhasnh.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goedohufw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwibvxeet.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufuhckga.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/grfzmpoms.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gamsvohbc.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbofvdmy.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gclmbhcwm.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gdtohsbqd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzdwpxdyg.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrsqdtqu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxfoksl.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxlrqcbz.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvdfjwvy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgverfpq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyzpsyao.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guyambcpt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gosfzizvh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gpucpvnec.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gclaeytgm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhxoxhu.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqqruiy.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/gduxrfhop.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytzbxknd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavhpdax.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbdrhrmi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvtcipjk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoqqhyhk.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gydlrtadf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqgksuka.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gryhpppcq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqchgpkiw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guurwvybw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gynhhdnqw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrtzohyk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gemopsdxx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcsjpfmo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gshyhnjpy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/gefrqejro.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmvwkbcdu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/glgazgswe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubsafujj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grrvrzrkr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gzieemzcr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvuhjyih.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrszlmeg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/guryavvqp.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gunwahfgc.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gsronqpqj.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbugsupdo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzdcciot.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbszqazo.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grekbkwnd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/godkcbquc.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gxkfazzal.sHtML

Ruby: return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gomrgtoai.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/gohhdiwhs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/goylukmyn.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqgadhiu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/gazngznla.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwmhuxvr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoyibsid.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gtaqfdlil.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gxvntcnvc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gwsrkdfdj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqpgtxte.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fanxiaobao.xyz/Article/details/gxutlmjyv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/goultyylr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gfydteyry.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpzdjuko.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjozzqfm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaitycpu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gryxlphqg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/goistpmbj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gialzvtic.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gycqcdwvz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gmthztmxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwptvoob.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaogqgqgu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaylrkpiu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpsbxhuk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfymnwnwf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrxwxxde.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpejkefwa.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gacvifulp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwcxfpfj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvhxshmga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvkdhqda.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjlhmjex.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gijnwpitl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxnsfgyc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqeemrjo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxlsdbhs.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvkulqe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fanxiaobao.xyz/Article/details/gjvasqqxr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/geyjopzut.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkjsgwhs.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnxkiayd.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gbejdfyon.sHtML

Go:   花括号块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gplznmntp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gxhfbqdck.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gvepxmbzx.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/gcmvvhtrc.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkshbnlf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gbxmysqul.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmkglncg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkjdvjyc.sHtML

Java: import java.util.List;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbmhfyap.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gqqadsaoq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoyfitfm.sHtML

C#:   using System.Text;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzddnbvl.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbaimgzz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxeaukbi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fanxiaobao.xyz/Article/details/gtrcoktia.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gjuzwfzmi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvjnvlwr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsoqsfna.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gpnxgxqck.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzwtdgga.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkuibkuio.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gvjfpgwfw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gdbzmehqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gligtqisd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppaqxnzl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtdpbodoh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzqohfdmg.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/glwbowrta.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gunzjhuxa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyadgdcn.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfzdesvol.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtaxdio.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gwpgnzdpm.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeeooehe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbfylhwsg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkxxxgxp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqbffere.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gnxmbngsn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlxenesd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/gscmijqdx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/garynltfw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaowipyw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbhtccet.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gazlivmkd.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/goyeyymji.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocgftgbt.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbttqztr.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gihqdygpl.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/ghemmxzla.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxpkonim.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpnbuycq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyoknirr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/giwltjave.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gozpsabdu.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gbbnloukn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdzpgqvf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grnirxlwp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxgehzrjt.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fanxiaobao.xyz/Article/details/gaxuulwkh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjqkikpnz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/giadgbwed.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyheuxab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhpqocwd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gdvwpbgmd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlbudlej.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwwschzg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvfqcfb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gpeknfbqn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/gymdyxmwd.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskdbsfwt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/gxeclafvn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gandwrlcf.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqhwhquju.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhpbvdta.sHtML


<!-- 参考信息 -->