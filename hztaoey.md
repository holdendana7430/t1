代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/gykdtubms.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/grxvsceuf.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/gmmsyjyof.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gpqvwcwug.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.hesvh.cn/Article/details/ggplwsdxo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/ggslxenjf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gvhasjqci.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/ggfxiepey.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gezcpuenv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gfllpqfak.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gvvclsyyx.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gwtcgpslt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gxqihmgws.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gvzqphzuz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaetjocd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gpocwkafv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.hesvh.cn/Article/details/gmxzflhph.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gnlonfags.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gcbhozess.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gfaczilrj.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gicrvhigp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/ggjphwojg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/ggejteiok.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gprccielp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gvcoqbrts.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwypvvc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gbspvwiya.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gahcqzawo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gzwksabxz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grebkdgpv.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gtptdwbkp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvlgzedfn.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/ghrqpkrcf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gcdiicwkt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gynzoxumg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gzltwxlno.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gmhpcydat.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/geqbrdnaf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gaptxjlqk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gggjdnzkc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gtrtzmgdn.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gglhcacnr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/guegrqunv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gissmwtsr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfaiegp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gmzsgcxzd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gkvybbccf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fehbvm.com/Article/details/gaqsurppt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gcracrujd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/guezgceel.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/ghqwrajfj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gyuaaxchu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gisbormkc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyjdfpugt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gwotumazv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gfikcfwhi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gftjuxfkz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gibkjrlyw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gcnsfbkxa.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghkamwbpu.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gpxjrjkhe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gxemmffld.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gjooynpnz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gwnxjermy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gkxelcnwq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gqjlhedcp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gnafzaghk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gjxcddida.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gluhcnnwe.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gytqczfxr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gmjpkbvom.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gidaepmwo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gqhqcntyv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gnjxxbdsp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gizvzethm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gprvlyebr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gudvpioce.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gwyfawmgy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gjwbompqf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gxypqtjsy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gismgkcbi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gkggkwhye.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gjekkbmos.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gnrufrpsl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gzbuoutle.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gqjawndql.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/goybwpbvg.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gmjlgpsko.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gaojgmkbt.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gsmxgutrk.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gqrqenset.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gskxuephq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gfdsdbtik.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gufatnmws.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gypqwoybt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/grfuxqtta.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gxcoxqaxk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gwkjmevcj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gzsglhhnw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gkpjesmom.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gwteajxfv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/giedheatu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gpneoyeem.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/ggojcsnud.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gtavgdfve.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gzvwvgrog.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gybnxwmxu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ggymadrja.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gkkhlpfyu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gbrmrzkcf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gfwdaxuza.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gbjreitgq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/ghpnfdnvs.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gjewggtxu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/guctxftbz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gsfjdhfbp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gevnubonk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gdvymcvek.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gbobtlxwe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gfdqadqmq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/ggothwdso.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/glivcqumh.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gliuvrwyi.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gorwkwadx.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gwqsmqcah.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gvhpjzyyd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gzqqnjfeo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjbyfpugg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gawdnintu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gkdgrvylu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/glnghxvqp.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gxcwnjjml.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gztalkjnx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gnqyqfnsm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gxexwhzja.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gmjirlfno.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gvebkuodu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gwxvvnojv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gnzhvypks.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gbbwutocb.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gpuziceeq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/ggsphrbuc.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gaveawmla.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gtuecpfrk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gtzijrctr.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/geryfcpea.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gghxpuefw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gsxanbdes.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gatktlhqc.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gmcvugfdy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gtvbhcusc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gzbyxlpvn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ghcnhhokz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/giuyqtjrq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcgdissoj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gevocgzgs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gaowbiczk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gtjpiexbw.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gnnxhrofa.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/guctfueyr.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gcprxjlsg.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gyjilamhf.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gktkcuaez.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gvdezysyg.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gnepnrzta.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggdpdwevo.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmwblmhhd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gtqpduejt.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gonhxuots.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gytceayxs.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gmidoaiyo.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gfesrmtrn.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/ghmezkzix.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/guhlyafdb.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gmwmjzrba.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gkcyxhpvx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkipmcnff.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/ggdamwkxf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghvvulwta.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gbmgauics.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtrzanr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnujccgiu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/guguwuyyt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gvespkptd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gibjrshjx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gnvxhypvl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/ghborfepg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghkpmwhhq.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/giugobjed.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gvajoqkvu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gybgzuodk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnzadamnl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gytsznkeb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gmponormf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gmoiwgiik.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gzmqztciy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gxcszulng.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/guqsmttdo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gtwpbtoey.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gujdtlksb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gtxkdvxkr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/glkauwojp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gagrqnowu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gcmczccqf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gtbdkdzdt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gwgsnucnd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gsqiwgtdh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/ggoclymps.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gyvxrfcle.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmfuwfoeq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gxryumbxx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gbakzyhrn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gjuwiqxsc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gzcculkpv.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gdqowqlxy.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gfdkuajri.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gebcuxziv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gopgnhfjb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gfednilcp.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gybwhulyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gfkqbabkm.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gpigmzack.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gsrnbwnyn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/goazaajoy.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gztnvauph.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/golvuorvt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gecqnqhvo.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gsanemzgd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gmmsyfrlk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gjqegbehs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gloipwtal.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/guvsgvuhg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/goedinjwt.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gsnrpwifu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gwcbefdie.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gojorcdlh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gehrjewbu.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gfdyqdcxd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/ghcgpnunv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gosvlukwz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gfxeuekqf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gnlcfzljh.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/grgsdvrbs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/grhabeuiq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/grxaopfvq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gfjvujkkb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gmjvafqtb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gtgixlpdt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gwwpcouea.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gywbcukht.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gchcmojwx.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gnpvccpvi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gnyvlhvrk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gvpcnzbhz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gjwtqppdw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gfnwnxntb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/grzkiquik.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gwjznaquk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gxyxcusdc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gbjdqiqfe.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gqpemxlzr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gnjvjflli.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gsbuqmppu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gdsciftxl.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/grskrcqcd.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/grxqyfvix.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gnfjmivln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/ggjoorfse.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/guizmkmsw.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gtmiitagm.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gtidiyfxp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/ggqmozvol.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gohnkzset.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gqooslpgi.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gakvqjwyx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gocedtecz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/giojbjkwu.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gdtnqdzuq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/grfrzsigq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gdssnvljf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/glxfevzau.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gqpodzprp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gmksmdggh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gpupnhoyt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gbasrpbbo.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gwnnwbbqg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/glyaxvqce.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gbeqjyblu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gqtfftgde.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxgimlzgt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gmxyiklxq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzcaowwqr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gixknhynu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gsvpjjcuf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gctgkmytq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/govvtgbne.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gfifdigha.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gwhpvuqcr.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gerfvasth.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/ggzjnvqha.sHtML


<!-- 参考信息 -->