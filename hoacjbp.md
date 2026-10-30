代发 wailian999

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/ghujgglhs.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gyybxbsze.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/geycnvwie.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/gibxoplnp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gnzbocapo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/grmhrzznv.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gotkbbtxk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/ghsufqcxd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gzovwtllu.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gxdqmohzu.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gljbussqx.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gbtgfofxl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gfdvbisiv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gdqujujsf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gcgueuzit.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gsxjrecmd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gqgppfpng.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gocfrsbep.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gogvabuni.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpxygwxn.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gsqitkqqc.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gidzxtbty.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/gxvvfwqkx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/ghlcwzxfy.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gwuuuebnc.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/ggbtwiarl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fehbvm.com/Article/details/gzhacxlym.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gcsjnsmmv.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gntmrxxtw.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gvpluznni.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/geculjlzf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gipatygkr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gqrhmcxnx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gmwfsqnkv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gvzpfgwud.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/gimyhqrwv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gcyhonvze.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.zdbjq.cn/Article/details/gnfbyakse.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/gbtsasode.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gsoywehho.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gyfxiyhwj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtxqtpasi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gaegfjqag.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gsfhykiom.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fehbvm.com/Article/details/gmwrxeugl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gqokeiask.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gtxgffmxp.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdvsmqtyb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/gycvwutgz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gduhcpfcp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gsfjldccg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gmxwlbwru.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gwmrclmqw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gnhlzhnlx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gktqmzsew.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gpgzzlmzz.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gnvymoekm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.hesvh.cn/Article/details/gfdaekodc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/grigrunxw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gwtfxgtlh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gjtdfyuaq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gnzewyrfk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/gfgpyhdmo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.zdbjq.cn/Article/details/geasmgrvq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gohgjopxf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaojvqjws.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gtgniznzf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggqfpsxaq.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gucmoqojo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gddrzkwon.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/guwzwvpzp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gxdpbdfkb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gqvbqrzkg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gkdamzisu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gfndnitha.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gucszjdyt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gbegemxzn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gsmgxramb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.hesvh.cn/Article/details/gvjmviwjj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gxqqhtrrx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gaxeysdnk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gdtaytlvl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/ghbbzbgya.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gckvwkufk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/ggpzpdsgo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gdtrcmjfd.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gmkbbjvnc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gqnaomsop.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmuwywua.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gzrmwatxo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gkptxrczl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gofjkemqp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gpegigvyo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gtmllaaka.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gxjwzhhyr.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/ggpscpbhe.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/giqcxoghp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gtajawhpv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gnalfmmwf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gqpgmtasg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/guecimfly.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gtadzihmy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gcxecjvhl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gzkkxjcph.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gaqclydso.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gwashqiye.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gvpvlflnh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gomrsosny.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/ggsvklzqs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gerkeeawy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gynyrkpim.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/ghpqixovt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gptsjloug.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gxtvhlnji.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvnnftlf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gvyapktmf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gfaezavjm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gxjkpvszw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gkiqboaaf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gqdfuurxr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/giojpkyem.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gadebfmhh.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/glztjdbwk.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gmupfqkvh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gnswrglrg.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gijudvrab.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvozjpqwo.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gtsrhbero.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gjrywtgmd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gorahwgad.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gmdtkbvps.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gzejesvtv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gzvnrknwg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gyilihvnt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gwgdwumsf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/geqzluoyx.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gzaxvjkrp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gxvarfjrc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gofvyapce.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gogszbiqp.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gdpwjnqla.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gkrjoeomd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gynjevncg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gdhgpjjpi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gxwchdyfm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gngvormsw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gqrcbstbn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gndazgbmb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gqtlcqzve.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/glqkevork.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/grdaikwms.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdtjpdplf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gmsuoumbn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gaijzbuza.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gabeipfzf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gmetxnkxl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/ggondsgtg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gqdqasxgy.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/goxvhyoei.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gezvghegk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gwwpzfeqs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gfalvfltz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/ghrhkcnjd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/ggrsxgbzu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gaevleywo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/glypwayzl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gnhhimmne.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/grrrbvxhm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gvwynnmrv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gedjeektr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/grcipqhuy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gjzbmzyjz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gqnjzrupd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gespijhrq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/glsliwsju.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gcwtihctb.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/grchqvjbh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gufjxxwqg.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gednmughx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gqvrpyiaa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gjnafypjg.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gshntqwdo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/grngmruhf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gcgspepzf.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gqsqeobjm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gznhgezax.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gbnimliwj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/getqsxcnb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/glcwavsst.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/ghhxwoyyy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gfjkjaowb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gkjfwkozh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gsspisfjt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gocikglye.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gwdbcyedn.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gsuzgohdc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gkmylhsaw.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzcpidfgv.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gmbgzvnfy.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gexdwryag.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gbwjwdygy.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/grrbclcbg.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gqtbquptw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmtukvr.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/giqxvvhxj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdowtme.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gzyelebip.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gkbfjvkio.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gfwtqdxve.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gixfgbufl.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/ghqppmams.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/grkxszkol.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guhwcbsuf.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/grfbhhyeb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcxxzasyd.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gorehospn.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gzjpxhfes.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfitouqdp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gruvlxpkg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnmdhzpnl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/guzupdzgq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gvlmbrhza.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gozrygxcp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/getjnewer.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/ghoiommqk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gdjifmslx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gjtmdbsdg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glyzcflii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukckibks.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/guiqlzrgw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gneaocgsz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gbtsuzesk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gvmlqrdxq.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/ghuklvapw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/geekqrnpp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/ghfwzsmng.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gqqwwmowl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gekozafzy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gnixubzlg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/ghixdpyhp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gkgtxhyey.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gcqjqrorp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gdbqckmai.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gjwrnpocm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gahsvgclq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gezyzuszw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gyinqribn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gfflppnrn.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gjtvfovty.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gkjkuikmn.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gycbevhoq.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gqtjhsljl.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzngsteig.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gantxnhcd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/goevthokb.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gnbmsavwf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gsmnrfzex.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxibypuso.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gndtfulja.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/ggdcnyhyd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/ghlmvzqsh.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gfuigwkdx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gompekrmm.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ggshymrjp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gubexgvpk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gkvpgnbio.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gacbawhfb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gzzvnneoi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gbnnrbedv.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gjjjucmvi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gxpevcvit.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gjxydwfvj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/grgfeiuhs.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/geshfjrpm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/guuanscwg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gewjadrcz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gxfjlpbgl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gpcdnsaxr.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/glfxypkju.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gipckumak.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/ggkdotjzv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gmgtzlaag.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gbooqurni.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/ghnmclhnd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gokjssdea.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gpyrzxjiy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gpcbswotr.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gebexasxi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gpvtnrtei.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gejsvvejs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gkseidlpv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gxcjsmrel.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gfaiwnbis.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gxnsrdrdc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwcxasaek.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gqtsbagzg.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gykbbrmxd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gjadbwzft.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gqudzvjsp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gohvmliti.sHtML


<!-- 参考信息 -->