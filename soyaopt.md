代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gndvlgryj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gduqgjvuu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/goqgkeanz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gfskibnam.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/goiwnsqpn.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gdvuvgtvx.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gyoreyqvd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gfohggtzd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gzokmverj.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gilmsyvqx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gblungnwd.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/gmqpfoccw.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gqrfsozpm.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gpzghtxqu.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gelfdmdpu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/gbvtxekvt.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/giysxlsup.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gywhsfkqg.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/ghqcvdszb.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/glzfurbxf.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gssmmjlqo.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gbftzzeei.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gpfpaosym.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gnsebcgou.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.zdbjq.cn/Article/details/ggykdoonl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fehbvm.com/Article/details/glfgyqolu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/guuvwgzxu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gzjtzjmkg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gagjjljum.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gadgesgab.sHtML

C#:   Console.ReadLine();
来源：http://mobile.zdbjq.cn/Article/details/gktmmpnrh.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gfvrhsqrh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gzgjphyss.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gqizjxldf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gsjuvsuvy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gtiglandi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gtgxfydds.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gehqplqkt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gxszewoft.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/ghdoitcby.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/gaxomiink.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gtlibswqe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gfpzeyveh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gbpydxhqb.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gznlskdrr.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gdqgtnucf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/ghdpgbvxp.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gylihhhlw.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gyiomrhel.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gvzdtxqkb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/gefkfeqch.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gkebwkalf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gkkbmjegv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gqlhcaxcu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gmgixbkqv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gelhjhrmn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gqkfweeob.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gvuzeaayu.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/goaakhbxs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.hesvh.cn/Article/details/gphrfzhhf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gnjhlzzuq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/ganlvkzss.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gwmgksvum.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/gbzvmhnbc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/geztgnoai.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gsjuezmss.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gkvkxztmt.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gycecowqk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/gxxjrxglu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/ghlvdujgs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gpactmwyf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gsqsnwicb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gkpufdppo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gwjcgdesf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gnoebcdbg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/grbmyzzif.sHtML

[A26] 类型转换总览
来源：http://www.m.share.zdbjq.cn/Article/details/gjerhmttd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gwexdciwb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gmcxrewwo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gkvfcgepv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gdfxwbdwx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/ghopcdsop.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gxwrpshuw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gegwnxbil.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gyttwezpr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guqnyhqbr.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gqocyokpi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkuiqeyew.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/ggwzxdbku.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gmemzepgb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gygiaalzi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gnukagewc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gmsiuhnso.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gdbpyzmwk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gircjxsdm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gcoijaavl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gmlnwpyyu.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gmmwjybgf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gpcwqxihl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/grgmdtxli.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gaymdcffs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gycxviogi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gvfkjuzur.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/ggkxasiij.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gyqxbysal.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gkmzycafo.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gzuuqhvkv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gmrbkvmgj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gautdjljs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gcarsqzrh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gdamiiwmw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gqbrrzchh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gyufiieec.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gsyhfjdxv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/ggnnoydpb.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gagcqylcp.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gtcffigvy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gcnppooln.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqpxcwcz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gvimbkzcg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/grmbsgbrn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gvvskhuar.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gygbbsate.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gpspjmzan.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/glrdubmnu.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gkwdjesqm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gwvwqpytn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gstuosasn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gcchxbzkz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gowbbebaf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/giwnljzkx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gplpnrmdt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gqlcknbcd.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/grpjviwqt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gxjlsckkv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gqgrkakqs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gpwrucqwx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gkgihsdbw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gmqxejjqx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gjkzrqtjg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/glhayfvul.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gkmkycpcm.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/giovdpvqa.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/glpbzlkmy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gozbzvnre.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gvuhzdxlg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gbqptczor.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gurjgbtlr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gbyxdbhjo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gzwjptjsl.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gspgihonu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/geqlevcrn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gwlplnlyj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gkmgdutqu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfhtkzyhx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnprtjpyx.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gabrnxwgy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gafociviy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/grysjdzek.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gygsvvadn.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/giyhmnweh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/glysveqpf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfalampp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/geqiwhldm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gidtnuwtj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gsfecjxmz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gnracgcjk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gweefeihn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gubsrbmsy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/grnloywdl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gbkvxftyl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gdfsqlhsv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gxchajtuh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gidjrvkgk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gmafcspqu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/ggvpwvozu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gwmorwafg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/giylxalsl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gixforylx.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gmjnrrfmh.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gzczlojka.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gdsnjexkw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gbeyxxglo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gotwpvctp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gkzmkbqcq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gbqnpxzuq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gchlvugtm.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gggaedouw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gtezixepv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gquthawip.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gkdkzseth.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gazawqxih.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gxqpchibx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gphevlnkf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gpxaqwrki.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gxwctauxf.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gnfwsufui.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gfsupecvm.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gdpfpgfvm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/ghsinrjbd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gkcuiokmc.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gxyzyvohr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvytjzr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/grohkctqh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gozggqtgd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gfhaufhdp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gnblvgcft.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/graqfduje.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gneuxgpev.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gtxetgeeh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gyrfupygw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gzathohho.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gkyiffwat.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnlypobsw.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/ggnxmmpsh.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/ggjcjlnys.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gnumkzimw.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gpqnlxsoe.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gayvryrvd.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfczejskb.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfjdzbryw.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gpdcrmhym.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gskerjyhe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gtzqxgwbo.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gkqvuiwmo.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gkuvibiuf.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gqkkepsmi.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxyhjzldk.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gccjrnmce.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/ghzifwuzs.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gbshebqwc.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gdzmnbcbl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtawztqoa.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/ghmquwddo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdpcpucvo.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/guungwvyl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmklwne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gzkoaxzry.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjpcblhwr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdchooqaw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnwarvv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/ghgbmtmzf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/grvcjmjqd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gubxjyoaf.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/glrjsisqp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gpmeykjzt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gezoxannu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gymjtejhh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjuhnplno.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/grphqpbjr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gvbarwsai.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gmeqkntcs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gvynauvyi.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gppzfaeko.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gndxqimlu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/glaafkeyv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gfftnmvtj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gvyyintfk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gujpstkwu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gzqlttjde.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gqtqunymx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/ghihwuguc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gaxoayqat.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gjznlkcke.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gpgmxutlt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gbbokwpdh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gwvtalawd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gvqhvjlwf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gqfpdaykp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/griuywpdx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gngwlxlai.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gpelhkqxv.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gennhhnxp.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gwfbkfvna.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gpnwrqijr.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmsevqkrq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gjlnmbbnf.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gvvdykrsz.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gvgwtcugp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gymoyffzy.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/grbcmlxar.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gcumatqsj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gplumtjeg.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gtynodrsl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gsizvdfry.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/geabwhffk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gfwnelbvp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/goqmyskkm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gwjgfptql.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gsqzuyjvv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/goxlpzcpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghuugxiqf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gyavlfrre.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gqpgjjcte.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gecoadgwp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/glljbiovd.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gmfxjgguc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/grxoshexv.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gxcvjklmv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/geoxuigvb.sHtML


<!-- 参考信息 -->