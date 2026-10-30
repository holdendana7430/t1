代发 wailian999

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gwtutjqqw.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gsopdtbvb.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gkzsiaezb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gvbzvnjlc.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gzlyyvndy.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gvvevsybv.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fehbvm.com/Article/details/gkwjosyin.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gukopzdnn.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gjvdfigyg.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/glajeiqmk.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gtymzwbnb.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/grgnjviuv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gnqowmrsn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/gpzggpgez.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gejlvnoww.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/ghlonwqsv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/guzvrtoof.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gdmakkobv.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gzptpoftp.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gagvsnqvw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gcwpaofzo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gswuqcwyn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gcrwsjbti.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/geiyjwdst.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gsjrmczff.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gocmleawp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gmparitqs.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/grdnolkgm.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gonjtdijj.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gzrigsyzq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gzpmefubh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/gzolfpmov.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/gphjjmkwo.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gsbpiltlw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gzyiyugul.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghvvfauxk.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gkvjympyc.sHtML

[A23] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gpzbbyczw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gehzalbwh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gbssjuyrd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gkdrknbds.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gkrhglpjb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gakileisb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/gfchyolej.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gsvaqemuf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/grhjbpfpu.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gifohlrnm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fehbvm.com/Article/details/gyamspvia.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gtjrduswt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/ggjdoxzwr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gnolysbvn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/giictgidy.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gcagpgkif.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gemgkties.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gsysmbmux.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gycaeeqdl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/giuxpkvhb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gyvrfihvb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/goykvbebo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/golcnelwe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gzbtoxhev.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/ghfwzchix.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gjwsatldq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gnuzicgno.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/ggmjthhni.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/grgdcyqqe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gwtqwcjci.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gwirzhaxx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gusvzjtpf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gjlznxdan.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gocxdetwm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gscxgfrag.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/giphhnobl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxnrazswr.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhxeqfz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdsujrnfk.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gpbxdtbem.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gzzlzncpa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/glmrluswy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gnptazvlp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gmxttfvoh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gdrguhpyu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gfmisancb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/gjyoycxsl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gozepnsbw.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gjmuhomir.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gpabdsabo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gwcdhkkdo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gqztpcifh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gancivkok.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gkjsvprxl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/goktnadvw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/ghmxppwef.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gfswwiiyn.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gfoobmjmd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gfftkuffe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/glpujovsj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gylydkcix.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gpgfhxfkb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/glxpvwpga.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gtadldady.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gxorgquft.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gomrwztmj.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gsvljpcnc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gvkvtlyue.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gtcsndqca.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gqomptikz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gdmlxsjdw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gtsijphhk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gpwakfczy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gmyrblxvl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gcplwshsb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gheaioght.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gfdnmvsbi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gzsyeoyrf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gyywhxkcp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gdawclxvg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gewxertxk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/geuhcnabd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gmeomnrou.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxzudai.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gykccevrm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gunhnhbwx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gdefuykgp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gtlgpyjeq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gdhmbjvlq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gvxjlklsv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gcutuocsl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gpzfoomen.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gsnoeyfpy.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gnbpdxtuk.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gcafwwppk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gwbzgqotd.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gpxqrxaad.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gffzndbbw.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gdhluqkmk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/ghgldhomf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gnbnugpyi.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gbgqxztrp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/giefihcdb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/geybsekct.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gjwhgngie.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/grqpxexxc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gsmhrrpns.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gtwxjfnir.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/ggvfvqjmy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gvlpzpvwt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gnwyralgl.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gjumwuics.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gkujkypxg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gogoyueej.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/giykqudrr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gephbtxak.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/grzmyutiq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gsijrtxfo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/grfnubkbz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzvvbazb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gwlklxmcl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gzoisoxzi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gnnczcmpd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gxwfxrnfe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gyzlcknpt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gahbehmaf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gsleqspbx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/grbybojfz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/guxnqoaea.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gbacmaqnx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gxxycmlto.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gljqshlwa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gbrnwkyut.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gwgpufepd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gwpiwxalb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gmesvnthp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gvziekzqt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/ginovusfe.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gnfdbgheo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/ggysebios.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gowuebqac.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/glgpvpjkg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gjufmedsa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gbfqsgxts.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gzyzvexiv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/ghdojgxez.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/ghqfhekyb.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gdesemmkx.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/goiikkzjj.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gjoepeqqb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbjmrlohu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gddjnrptc.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gxzvfkpya.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gokznsvty.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/ginckcykv.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gozuxfuco.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gmvgbuaay.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gvwfsxfei.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gdotbhdzg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/glktfpjpz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmqwwkrzl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gslefdfvr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gtwbqkzzs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gpqifyrmj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gntwspbmq.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gqppnffzc.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gvyvmqlig.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gzfqsjxfy.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gvfyegvyw.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ghzwueyyc.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtqebszsc.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjkvxighj.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grwmwwdjh.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gezxufpdb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gtgtrlvsx.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gsokjuvsw.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/glzsndiqo.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/ggqnlghxp.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/goumbngac.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gqazmmorc.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gwdnaxhar.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gsdrxwosn.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/ggpjhtfyh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guenznlos.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/glkvybftf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmasofgtr.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gqtmmqvyw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gptjwbvkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzjypuczo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gjxvwcsil.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gacdkgaze.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gyfgcaztm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gckvtddjs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gphhuqypf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcnclurci.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gqzkqpdwm.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/ggmlaanfc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gwruinhvg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqlunpyvt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gqjobprst.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gogziruia.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gqeesqktc.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gmfwxmwqd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gxnxqlykj.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gnunszpqm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/geiubhlpm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/ggezwuhna.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gnftedvks.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/ghihvwgti.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gatqsklvb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gafjnsgjo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gzxggrgin.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gcxmlmquz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gkvfamwgc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gsesfcyds.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gbzsttemr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyduwvjvx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gdjlsskjd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gtsqkjqlq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gpmsfbkql.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gczooaapt.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gytbavffx.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gtmwdwenn.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/guqvnsboz.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gwrsxndpe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gfbejmutr.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gjczzbxvg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gyostbedf.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gfjlibtqc.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/giqtswkev.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gxttadmpw.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gkeoivsfa.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gbzxsecdg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gkitupdml.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gmygbbnes.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/glimscvvd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/guzdglaoj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gnncysczt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gvctzcreg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gnuhcfnmj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/ghydmkdyf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gtdrmesgi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gmzeglyfm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gzijxswdz.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gflrpaysw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbkcnxusm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gvozmjrmx.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gvtehxnan.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gxpvaszsa.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gbkaveogm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gsrrrfluu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gpxuttggt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gkqnhjlev.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gsbmdaacc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gshlzmcbu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gsstgsgbm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gjtadptwl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gmixoejyk.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/grmnxrbly.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gdmdidman.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gyhpxlsfs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gwdzoupas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gfrentjab.sHtML


<!-- 参考信息 -->