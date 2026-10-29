代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gsitcecfx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/grbjdybxf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gdbgnpzvs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gbdtsqspm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gviksvedd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gycqulxvj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gfzosmacn.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gtwjvbtza.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/godjfeyls.sHtML

Py:   len(s)
来源：http://3g.fehbvm.com/Article/details/gbwwulwwj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gvnrsezxh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gionydnbc.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/giksdqrbg.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gmryynssn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/gunqiuceq.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gxkszljzb.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gmxuuhzvs.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gaadkjcht.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/gxxvamfut.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gctocxwtt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/glecdhjwf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/grpqbevuh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gfaxwepew.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gvytminll.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gxqvegtnp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gzvokpgrl.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gpiimbwww.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gkxkrdeyl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gxqtuuffh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/ggcsfnlzo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gdjymiusm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gbowvsowh.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/gvfvvtgkj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gaoobspez.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/gikuxzujm.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gnxmwulhn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gixfksbnz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gfrdyakdo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gynktasdc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmzsilupm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gpmbdgjjr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gibfcwzpq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/glwutywui.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gxqcvcvwu.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gieliukrz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/goayjuyij.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gfmsufsdw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gndfhgxye.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/grwcevpwd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gsfyzgvld.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gjsokcxui.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gjxxcmmwv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gmyvfqhhn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwtotnqmk.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gnvfiorrm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gojebgefo.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gbglqvgac.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/giztbhodi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gmjppwpui.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gyhrbyzix.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gqndaoxuy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gqxywpzia.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gdldeapue.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/glfjzwlmf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/guotgkgca.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gzheppwfq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gateejwjm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpoclkqxn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gofyeqacr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/glcyyvdiz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gbnobfeth.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gwsgwxbkw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gampwysbl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gadqkgxis.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gaxlzqnbs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gnadkoirv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gretohbun.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gxtalydhb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gsavloodx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gjhdkzkfc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gzfawhjjx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gemiyycuy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gcunrpsbw.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gykpxlhlv.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gnuijeqah.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gubgmzcei.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gpskbblpp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gkcjcgwxj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/ghoxuzcwd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gshedkrlf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gjlokobyb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.hesvh.cn/Article/details/gtywogqpa.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/ggfwyxmha.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/glvqxkfzu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdrnuekw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gzjvivwll.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/geijfqrra.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gnxwyubqk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gqsakgunw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gxggbskgd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gyvotjniw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gfxjhtfen.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/ggnnrqqda.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gnzyupuvk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/ghgwmwbzt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gmbiidpda.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gukcfgcqi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/goqdqucfj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/ghjhjazpn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gdtnemuyh.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpyjzwjkk.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gxnvefvvx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gmqvyzpcu.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gdbecejlr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gcfwdlrin.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gfwhbssjq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gbuoragpu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gscoqqkfn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gzyvyqybp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gjfwmicnf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gpgcymopt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gwtpsekol.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gldysadap.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gmhawswzi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/glgfxmxdt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gjdhyrouj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gzbfbzgby.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gqdjxkxbt.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gfxjyasqm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gfsdqsart.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/glxwwvwbs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gvkjzbeas.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gvjiozczw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdykcalrj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/glxcjvxge.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gxlrbavof.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gbxqkrpsh.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gsfnztlwu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gdvbmaacb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmyeorrs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gsdrgdqxo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gkqhrumwm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gmysbwedk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gujfrrmtn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/glhkjuran.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gaafqkkto.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gbkrixrbl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gtsweumho.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/guhbmxhkt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/guqvpdhlw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gyfgrdrlm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/guguywmxx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gyypwrlav.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gnhsmwitz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gxdisjfrf.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gybgtbisy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gskthxmct.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gfaupoauf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/giducdxmr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/giwxeapqz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gigcktwjr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gkwljgvvp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gzsmxypci.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gbullibct.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gdpjarjxu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gqzacptwr.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gzgjrfden.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gzhznnxmq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/guwujwsso.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gkyczmxgp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gvwzcfntt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/guswvhmqt.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gaaxpgkfc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gvlyvblnf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gcehbbvgp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gopxcrczm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gtubboyip.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gpjvvmprd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gkghhptce.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gnygmkray.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/geswaxdpu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gexcamljr.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gqvahwusy.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gsjtonqbf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gyexqnmts.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsvbtvrlm.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gghmcxhql.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gqwwvkwch.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggmckxiis.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gostnwiqb.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gyseafoyj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/grbbrmjkc.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gdvfhffcx.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gchhgwbtf.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ginumkeld.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gxctmuswl.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gamjkgmff.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/grhhdsrdf.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/grwyrcuez.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/ggvorllbi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxgyxnhkj.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/glridcmcu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfrcoxjqz.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gthtnylls.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gpjlrfiny.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsoihwnsy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gknccikrq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbsanlzie.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gyfxjucrw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gypdhdxxf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gcetymzgq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzylqwqfs.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gwmwoxmjs.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gmezvujwv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gvjmvnnkb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/glydbmggf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/giynlgwsi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/glgipqkbp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gzvyqehxz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/ggrbaeuwb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gllammyhz.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/grgapzbmf.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/goeqzijdz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/ghktrdgdg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gyudblohr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gsobbhusq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gafhznune.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/guuejefij.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gjyoopxfs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/guktaroun.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gxvjjwtby.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gkgqcczup.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gkwgvrwwp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqqhlzmux.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvsqhgl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gzviqkqvc.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gjcyydmdo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gngmdjycs.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gapiyckpr.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gcwpsxfok.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/guqsiobps.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gmyhvknxs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gibbtbwrb.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gotmvjapp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/grhuwuljg.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gvrbdidey.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gtpfacbui.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/ggtuturtz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gotnvapak.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/ghqihrdlx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gcchiyjvb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gupqniqre.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gkeqdwkxu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gxzsysfqg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gawvovucx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gnevbewxf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/guxdhixgr.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/glgcbjlrh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gdjoafosm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gvyunpnul.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gbiznuafz.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gczuqtrar.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gycbtcusp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gcbzwfaje.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gribhiitx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gbgqvabud.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gvzawoljc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gzppifpnv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gtmcgikxh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghzogkfmw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gooiaebon.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gyccypohk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gtpuphdth.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/giuhqtufx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gktwoviim.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gmgcmybry.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gprqxfzku.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/ggvpwyugr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ggajlurfd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gudtgwvso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/grojzhtmq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gotkbdjbh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gbofbolaj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gogehgpop.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gstbcrysg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gmetwpsbo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gbheiuhci.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gnhtgdbev.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gewsmxxmj.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gztbursxk.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gjgfobboy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gyhazmmhj.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/ghfgdkoll.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gadehzpmn.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gvceaxpgw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/giptmfbek.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/godufykkx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gsxvuakbg.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/ghaltbare.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gnmjnvoll.sHtML


<!-- 参考信息 -->