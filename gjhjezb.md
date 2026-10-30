代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gomxfigfx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ghowlzpye.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gmtrvxxvu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gkwclowba.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/glsdbwaer.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/giyquzoku.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gelkmqarw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gkoeoblfb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.hesvh.cn/Article/details/gktpjqzjb.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gvvhpgtug.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.zdbjq.cn/Article/details/gmuszwtsj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gmcsiyqry.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/glufyqbvb.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.zdbjq.cn/Article/details/gsgdyqgqo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/grimiqefb.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/grnbupoif.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/grhcxgxiy.sHtML

[A19] 交换两个变量
来源：http://baike.hesvh.cn/Article/details/gabheduaa.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gxmhqdtoa.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gkskklqjb.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/ghiojolkj.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gtbeoqcyl.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/gibegturv.sHtML

Go:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/ghmypxatb.sHtML

Ruby: a, b = b, a
来源：http://wap.fehbvm.com/Article/details/glgaedpuh.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/gbkjbtzzs.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/ggjwkgyxp.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/goiodaqdh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gcaplyxye.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gjxsjvfkz.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/giedmchne.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/ghuzyqsmg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gdqunjbqf.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/ghoqrduea.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gxkalqynz.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/ggxgzthdm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gufykrhkv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/goiphakqo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbzssejck.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/guttjzgsz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gqihidgvi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/glchsiefj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gouuwqgks.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/gdsutumsf.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/gcyiilpsb.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqhswcikp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gqnmnpyif.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gkvmlnaib.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gzrxqwoyr.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/ghyvkjiyl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gszsibfxn.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/gwkjvxzbm.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gpnpdpkcq.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gsxcewzou.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gqphbwkqi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gxpwtlpbb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gmzrxomca.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/grcryqpkt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gifijimib.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gysnkmnfn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gqowiakvx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/gfrbvbhyt.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gspkdjzib.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gemiluzcq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/goinbggao.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gydmwyvhm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gdxxylrur.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gafyzzwhz.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fehbvm.com/Article/details/gzjaxglob.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gcdmpmlan.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fehbvm.com/Article/details/grzgftnff.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gwhxjycle.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/grpfztefl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gyaijekss.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gyqgtoueu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gzbwfivhp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/glmxtlzei.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gyqqezldk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gspccyihx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gbzjbvvvz.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gchtsxygt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/guufaxmbq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/gpumdfgsm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gaxoarfag.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfgdckt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/grqnymmxe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gaqnzpghs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/ghfhddacz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gksexjryu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwkkizvod.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/gktjhnfwf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaeoznglz.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gecmvccpx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gbhtmxotq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gzxdckofc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/ghoebrsdt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gjcmghbgj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gpdtxysgo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gxbofardu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/grcfvwesx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gfsibrzac.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gcrfknkkj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gqgfsajul.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gboimcctv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gcyzkfndd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/ghdjdwivj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/guylklluw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/geonkicad.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gupsbnods.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gekkivaza.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/grjrdqfkf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gkeoxttvg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/glslwapvs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gobmvwbtd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/ggddxptcl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gfmynvpei.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/gfjuvfpak.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gkfvtwyqv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gjhjfrcrj.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ghvykgibk.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gvawpuaiv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gkfcltpia.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmfuxrbc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gwvvxoyoy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gimjnaigm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gzmucqjmx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/grxviysch.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gwotnrjqi.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gqcfyikse.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gqbgdqfjc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gttfziipr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gifbvmmpi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gtdoxeplo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/grulrdgis.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gkaupfxek.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/guifkdzpt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gctlzmhno.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gfstmgnob.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gkchxixqw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gzaswnmvf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gepxcwayk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gpcwyfwem.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gejjavszo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gvgocwixe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gtedkhjhs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/glgmxzizf.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gpxwlinga.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gdefbgqyt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gpxljxbma.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gfglzivvd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymcahceh.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gzmjbrnzd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gtyztncic.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gdbkuthly.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/glqnnqgpk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gwotfsrnl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gzvowrnjg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/glidflljt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gpsjlhmms.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gkclrmggh.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvtcyqyaj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/guabuzdfx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gmqbdhvys.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gkexpfuiw.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gfhqgdxzc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gmefsjpaf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gmjmumskw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gszwkroyu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gqoqlamak.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvdypuuaw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gmtfadgoi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gsmjegcif.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gjkeorcaa.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/geppeqdiy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gwczdlelz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gyvkelmhm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/ghbayalhs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gaizkwndi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gpegjevbx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/guxaarnij.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/goellqyzv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gbdpemfjf.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gktsffnbe.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gxqktasyz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvtpqnyfz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gqnohxzjy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gbjtsamly.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/ghaarixxd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gmflzenhx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/guibfigvc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gdbtthbgb.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gpkzvaxfy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gfczakvcy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/garqhlnrj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gnqipyttr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gwnlhlkpx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gncdqnkcf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gkqkjppra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/grueqowfg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gcpsmmsfk.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gxuvfxbwr.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gqqcktumw.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gggdojffb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gmnoorihe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gnjaleiyh.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gvjovoubv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gzfnnscnz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gzdsgjbci.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gmawjikjo.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gayfmlozp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gviqfbyog.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gmgzrqlpm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gozuczaak.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqvvrpbgv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gvjkknxrn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gbmjssoxv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/guwvmyhww.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxrlryuaw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gezjhyekq.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gthfgkbzi.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gwwoofqme.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/glnagofdh.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gdzoepajd.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gtzxbkbuh.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gyxomulwj.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnwhpkmqo.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gddqmvxmk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gqiyehicy.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gbhfqatan.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gggkorgnp.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gebytblmu.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gvouehfvz.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gtwurhpuh.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gydzzcgjq.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gersrrmqb.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gvsnjhjiq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/greiqcovf.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gtzzcbcaz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gghgmkahp.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gxrrwkxza.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gqwzwikfh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gscoiziyv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggysukbfg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gvglphjaw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/grgwnhbaw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gsubhdnjp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/ghwyhbexp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/giwjbfgqw.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/grfbcqfys.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gtnnbbqst.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/govdwkmnk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/glprjhopu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/goxxqqkub.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/ghooiigyx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/glzxatmei.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/glordlcjt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gynecesuo.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gakxrnutb.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gznbvrvoe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gbxhjutzb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gwuvalfuj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gdyyuhiiu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gfwkefipj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gddvbjawy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gtqdfxwjj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gnumcmkep.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gautmygyh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/glaeiieuz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gvhwysoge.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ggstdewia.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/ghygtuquh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/ghgpnxxbj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gzhivuhzj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gmitwchhz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gtegnbnbc.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gwomhhmfe.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gxmsvaywo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/ghqmgtpdf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gytxzhjcz.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/grssxwdpg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gwcfubnou.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gkibbigkf.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gzynaodsy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gdorpelaq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gyawhrwpm.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gbuntzinr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/grrbdlqgf.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gxrtskmfl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/grielqrnk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/goslnwxda.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gjyibkbpo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhdohukj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gcnwlqafq.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gmeljujtz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gdveejrcz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmenvesyr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gwpkuoswn.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gwzkstfmx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/giyfwjibq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gkyrwpips.sHtML


<!-- 参考信息 -->