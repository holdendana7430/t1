代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://baike.fanxiaobao.xyz/Article/details/gokynnfel.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gcdhwyrqm.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gfigwfmab.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gioctqoes.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbwhjzww.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fanxiaobao.xyz/Article/details/gkwurcojb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpxfpbwi.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxxavaod.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fanxiaobao.xyz/Article/details/gnproaolw.sHtML

[A19] 交换两个变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjipkvutv.sHtML

Py:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gxldtlopm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkydhyq.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gsmobncdw.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fanxiaobao.xyz/Article/details/guhwsqlrz.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gqovyhsfg.sHtML

Go:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gzeyeceee.sHtML

Ruby: a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gxhnicmun.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gevdlsaci.sHtML

[A20] 读取标准输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlilxzoo.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdyniqny.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fanxiaobao.xyz/Article/details/gbdgsbmmx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gdnydilnb.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gpqgaitzx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjogqltli.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fanxiaobao.xyz/Article/details/ghjltcrbj.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjhnlngm.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/gunhcqujp.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnudpjkx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gygqcolan.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmppyvyx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfugfoxsz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjjgeqsuj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpmvdkbl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrovlriv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdmfbqb.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/glietbabh.sHtML

[A22] 获取字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnriwczbm.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqshzdjmt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/gcwlrkatd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fanxiaobao.xyz/Article/details/gqppvqdax.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gncovneta.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcraegcxc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqmovofi.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwapimci.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/grcsoeyeo.sHtML

[A23] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glsfjpwse.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gfodfjywq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmvsqbtmu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqagawrbo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmqwkhqi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevliocb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxcdiecwl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gnhkrxgjo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fanxiaobao.xyz/Article/details/gaepoigff.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gdzhioczf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gcidwfkkp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfvgjzrd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmennreqd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuodlrjy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/ghhdmlilo.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxcbjus.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtdenji.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpzpthxn.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlfnzhme.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fanxiaobao.xyz/Article/details/guoimlgdk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgslpzwq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbzvcvlg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkqefgky.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guquolvfh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzzdpvcr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fanxiaobao.xyz/Article/details/gzczsryxo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbfhizhr.sHtML

[A26] 类型转换总览
来源：http://blog.fanxiaobao.xyz/Article/details/gxczhqzwi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtudyiqi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fanxiaobao.xyz/Article/details/gzjkyccfu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fanxiaobao.xyz/Article/details/gqzlrxhah.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuwfhamp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/gkpxsmbbj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcvbxpbla.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gozmrlstk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/guzolcchs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvhdqxlqf.sHtML

B. 流程控制
来源：http://mobile.fanxiaobao.xyz/Article/details/goqxlovtb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvgzmyce.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsfkgdlw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyseeela.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvrafswp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/grrzvnhse.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoqhgoan.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gmrbmgcij.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlevfhwp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fanxiaobao.xyz/Article/details/gxfqikvmo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjxnkmok.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fanxiaobao.xyz/Article/details/grvdjhjfa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/ghcukvtwu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgioebsy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoimvhno.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gglcggxli.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhlcdcnu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkhlblu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/gonqlbltr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gbyihwxgy.sHtML

[B03] switch / match / case
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwwttula.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqzjvzrx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqskvhfl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhzgvpul.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdidppwp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwnotgru.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldrhigyz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fanxiaobao.xyz/Article/details/gfvmeowgu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gusiyrsnr.sHtML

[B04] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrprdtvd.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gghtnphpd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpzfvnmpm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqabgtlq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqycggxks.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjcuwfcvx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fanxiaobao.xyz/Article/details/gussbdolg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fanxiaobao.xyz/Article/details/gpgueyxwa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gizximell.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdcaunaf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvzoblyl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwexvipqh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkqckgvx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsaswbei.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmixwooxu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/griqirvop.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpmlwcee.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gatkjjfjs.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuptezkj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fanxiaobao.xyz/Article/details/galipxeif.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjctapnm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbxkrqjx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gukadmbqb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzdfbwxgp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmqepvtm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gifhfqffy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/guvlllgcp.sHtML

[B07] while 循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvniggsgr.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gpuwesduk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsddoxmzp.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjneofjy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnmpsdll.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbqyodzdk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gqqarustm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gvrjzrxkf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gistgfhtc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/gekusyufy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtltzniss.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gfqbbyrqa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshvwsddr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gfswcxdpi.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpgjydgo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrlthcwc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzvbdhmp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjaknwb.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowbmxoa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpsogsek.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicshweza.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gviulssnk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gofvwtzcz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmutvanc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gxwrpdzxd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gryrbbhqw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxwfxuft.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gkplziwaj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fanxiaobao.xyz/Article/details/gltefyicx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggirpsakq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/goavziatd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhoujig.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmyzhlbfl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxfbobk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/geuftsvbz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gctdliqjk.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/ghxxjnvab.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyteetrwo.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbhnbday.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gujipmteh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxuutxbvk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjrvhmhw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gtddqspao.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjubonee.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gozigllrc.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/goujwisfz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gajbtvers.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtukoddv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gilwlurst.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhqxrydu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfjezdrt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqqiwyzp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gvorassex.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gmmyhwawy.sHtML

[B13] 判断是否为数字
来源：http://wap.fanxiaobao.xyz/Article/details/giavkzgun.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhtrvmn.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqotiiqsr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gtqythpny.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/glrbzlbpz.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/gajrchauq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugolwbsr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gctssplba.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvisxvwjw.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaoylnvn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcylfoafg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjiushlk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/guekwuuax.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcztyztux.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gptvjjpmq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoluxwgz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gisyecvsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghuavgxww.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbzcbmmy.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gcsamsrtd.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gjucdfdbr.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdkofmlo.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqnfviut.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gspnpvydw.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gfuyptzbk.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gkmrsddkt.sHtML

C#:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexnwnfhx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gmewwazyr.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/gientndev.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/gscnzxfpm.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjngqtnd.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/ghaeklrtv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpfewdro.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gljmzybve.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gjvkyfgbu.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gcpoivvrz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbjcmukc.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitsyxrmh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grtzbbzve.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccliijgw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnynpzbm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxufgvyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjhqzve.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grlbqlcwc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gujfabjku.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilixnqyz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhxhwdso.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjkrwkdd.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtvicjqq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/gxxzmtcla.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfjwbmyr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqncuoqvg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqoyuugug.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwqmzcxk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcittxdrx.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fanxiaobao.xyz/Article/details/gqjsqjcjq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbtjakqc.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gnffdsfpc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/glucpcjmb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwibestrg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqwxwzdgf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjqwsgasl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxmyrrxbx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fanxiaobao.xyz/Article/details/guuzgywqo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqfoyduu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/giuqjqdus.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiejpicz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gwwojjpxl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbiryyuqo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfrdjki.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/grbzpvkpg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gfgxgazqg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsezsrkf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjespzgs.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilobkdwn.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxbpwiqi.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqehwzpq.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gcusoytcy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrhgfjys.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpjscchz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzozcdyk.sHtML

Go:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gatwqjser.sHtML

Ruby: return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlepccba.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/grgabvanq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnkjewtz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/gvumhfodm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaprjuwz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/guyqkqevc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuiefxxu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gwdwddxgs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbetucvig.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioidkqcb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxmiimxs.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gnqwhjqxi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjketvhkj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhoootwu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkwsgsnj.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/gkljxuiww.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/guafrwfor.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcalzgoe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglwynohl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxtekfao.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymijkjlm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gldgibsqw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsmhcipp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxixddlo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkspgdoo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gvilgejuj.sHtML


<!-- 参考信息 -->