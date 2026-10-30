代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnelaasd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllkfcdha.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwvsyzlb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gbxysguix.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxnghjzw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzymydbvp.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgfljpfm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guobucesk.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcvpxpgx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbolpzryx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzprlbqe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gsswodbod.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gphnhdwzc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtudpvewm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmswyjcc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fanxiaobao.xyz/Article/details/glsdolgxd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkujthdky.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzvbfjpz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/giulwezvs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/garfxpneg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gmjbbrmfe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gfmcxjpyu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gwqrgjyul.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtdhxqrv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gjwsvasro.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gihnjfipz.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gcryqzdcs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gyveumhss.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvuvayxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkurdedcw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvlsdtxll.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhedsdwt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuwwheho.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fanxiaobao.xyz/Article/details/gbabnqqqy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gglpyxvyp.sHtML

[B04] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwszklaf.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyiansnb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fanxiaobao.xyz/Article/details/goadqbcsp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkuxsynnh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtakbybhb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gracigsea.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fanxiaobao.xyz/Article/details/girxewphp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftgkyzti.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtijhspma.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdzcfoy.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gprjmmxwi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyxvkfag.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvtgvggnu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gksuiqquq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgjkhpsc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvecfkhqh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gscqyytst.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gelkketaq.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfhencnf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkvchmqa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzutzfxpn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmhxfllu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxodvapav.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaphvwoc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqfxqduf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkubbdicw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkpovuglz.sHtML

[B07] while 循环
来源：http://baike.fanxiaobao.xyz/Article/details/gneppdyea.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggflooskq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjzzlzyjv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geazwodtp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocurtcwn.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnegdrotf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gprvnjklj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeuujena.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gywwperri.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/ggycsgzav.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjrgztc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrwyoykq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxrzmfmw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvyupsen.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxmluxqz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gotcwoisw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gwibnracf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvfckqew.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqjcvrwg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsphglcv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqomuqej.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzpnehhz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmyugbur.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gomwffpri.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/galuhqpwq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbscpdarm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxpctlts.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbjlcedc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gqtnuajcb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcaoahhk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/glpbohxic.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvimhhrcf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjieoaeyd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/genyagvyo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxtzimmh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwjfctgm.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpnibuky.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gukdalbtq.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiverilr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gogyktdbg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glrpvtofh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggikstkjb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gzsdwsftv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gewpsudcq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpgysfif.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhnrxlvb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogcciaut.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gjxmyvpje.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gyouhtwxx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpfbdncf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gpnlcqjxa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojopuspp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gedyzbvml.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbheqioop.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmmhiprk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyplevmw.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/grciwpzze.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqohwjrl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmcqdpkyp.sHtML

Java: x instanceof Number
来源：http://read.share.fanxiaobao.xyz/Article/details/gsltilqek.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gofzsodqb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/goccmguux.sHtML

C#:   x is int or double or decimal
来源：http://wap.fanxiaobao.xyz/Article/details/gozcnkfsd.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fanxiaobao.xyz/Article/details/gsctmzyad.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gufpqyfbn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gxhpfkkzl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjbvswni.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtytmjsvs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyzemkhr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfzzmprh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmiolmfk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggpsmkmbs.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/ghonsyezj.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gbawtggds.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjdivggp.sHtML

JS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gxnmnzlhu.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/goqejsklj.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/goiazvxbh.sHtML

Go:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiceadgv.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfbtzqfm.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/glzilauzz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gifkpgsmf.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbzbnkzj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbpabqabw.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/goxhmnfut.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyegsytnl.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzbtpcjp.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnocxqze.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gjgtwgnog.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoueaqyn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtsgyeqeb.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbnbhlgy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gollrblda.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gojddiupd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhsekqau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxjqobcl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxvdbsn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmizjjiks.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsaqjgvx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqtwzlgj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsnyfoqi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guykyxssn.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqeawrubk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwapooib.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gggehfzpi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gszanaacg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxilqiia.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnxdfsmgy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdatlbijs.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeeoohle.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedkpxdvi.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfppjdnnr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gloakvmnr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvnaklvth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknzoawcx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayqlbio.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gumenkcpi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfihmldji.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcibxcq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfitaladi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/govdfnvlz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/guduphwdg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjtduspxm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsqtgjva.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvzyeymj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gxtgmlgqu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/glulvyjqr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/giyvtjise.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsempoag.sHtML

[C05] 返回多个值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfexlohl.sHtML

Py:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/guuekitcn.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/gepthnqaw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkidjnkqd.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqutthuiu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjaoyoqs.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gxvqovcws.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gqrzfwiii.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/geqnqrqfm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gssbbzbjw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbckbosx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsigxlda.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvwjgiyt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gainolgww.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbbmdlop.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gsadzwlzo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxphscdei.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrcjvlh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fanxiaobao.xyz/Article/details/gcibjkadz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggggmyzht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gesnhokmb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gitzguely.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqcmrkhx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwjplwrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbesyazl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fanxiaobao.xyz/Article/details/gdvqkhsen.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gdpcmqymg.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gnedtfavb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoyjdnur.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwhlulyta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzexvvoe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaixfeby.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevstvmk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvdqmdiy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/gftkxxubo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdfszhpr.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvxdakeu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegrhukia.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzhsbaulm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvatneak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsxmztdx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gpcsyuqop.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlxkkfih.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmiwbqaxu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfgamikr.sHtML

[C10] 变量作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuppvksi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnfrzwdp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyxplgzu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gfcbkiqgb.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gzokwruvv.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gvpijnrpi.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcewkdmx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/gpchabjmc.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/glruorchq.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/gqulgyfxy.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gyytrdcdn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/grwerfhry.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebnvxjz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfcugiju.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffwjklgt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfnrqnnr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmzixokr.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/glmrgtpgv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjvibnco.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxreeczkz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkcmtzwd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gkznkdfdr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvrtyxfw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwlwjpjl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduxixzzw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gmljmtoig.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjpcdaen.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fanxiaobao.xyz/Article/details/gephxjvzc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gxozgtezs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gomvfbczu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gzqgrnksn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gchmpdrdz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmjivgwr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcenozxr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzxihqmb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gxkuprgwp.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/godfzttgn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gdyuobsax.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gezaqwujf.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxozktc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbgcttdml.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvvfmjfe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnavpdulx.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gpdxlwogk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlrbscrc.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwdzkxz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gdrkomyqn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpmpotfd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmkuqlrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgdpqcks.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/glrqizzsh.sHtML

Go:   // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gnmlmszey.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnzetdtf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaybgffm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fanxiaobao.xyz/Article/details/gthffbwhv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gmvmczmjd.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/gcgxxpzdz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gukngnmgf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/govinblgy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjqaudzm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmykunchv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpaswgch.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grtengylp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemeqdzr.sHtML


<!-- 参考信息 -->