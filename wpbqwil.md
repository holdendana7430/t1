代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gjpyioath.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gjcywhnpq.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwhewyxl.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gclqxheaq.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxednxahm.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gxgunoulj.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gckeitxem.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/goeggibuv.sHtML

[A14] 注释写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuwpizab.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fanxiaobao.xyz/Article/details/gcqpfcnrw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrlkefvu.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gsokedxyo.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gptaysncw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fanxiaobao.xyz/Article/details/gxxqiambg.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjkqscqa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzkqbqlz.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gamfgaokd.sHtML

[A15] 空值判断与默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gnloqhrij.sHtML

Py:   value = data or "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gfvasrjcs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzbzbrsa.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcejejrjx.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gtlimliaj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhjxflsy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxyedotu.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtazhvvl.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gyhiaxixl.sHtML

[A16] 真假值判断规则
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqukbkej.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gtnguioyc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbjeauzj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyrdfhwv.sHtML

TS:   if (!x) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdletijto.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtetrcjnr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gifzbpeav.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gmozsedql.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnmtuwlz.sHtML

[A17] 位运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/givrglabt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhsdjudi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggddmywmk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdakyark.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyicuil.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/grcymjirl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gepvmcolh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gzzvnhwmf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gycsjijfx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrcnvwvd.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtarooxcz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glokbswfx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/ginswximp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gwghqnljn.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fanxiaobao.xyz/Article/details/grgpmmawh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gamrljmkw.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fanxiaobao.xyz/Article/details/gwssglzjb.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fanxiaobao.xyz/Article/details/gklsrclpw.sHtML

[A19] 交换两个变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkduwcdq.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfgcxhgi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fanxiaobao.xyz/Article/details/gxnovkpti.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gfljkgnls.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fanxiaobao.xyz/Article/details/geaecfccu.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gssmisflx.sHtML

Go:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gcsnvvdly.sHtML

Ruby: a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gvarannij.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopjzzal.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/grgbdhdcm.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtjaocl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkphinvb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyrtgwdy.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltcxannw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtjtzpie.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpzvywxu.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejtjecdp.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gdnfuaruo.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/guntscumj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvmeupoc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gkngamucf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkyeqjpx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gazushtmt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdddiir.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gkfewnzej.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyswgqiao.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fanxiaobao.xyz/Article/details/gvfgfciev.sHtML

[A22] 获取字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gbhentike.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicafphjr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fanxiaobao.xyz/Article/details/gxgrzbrvb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fanxiaobao.xyz/Article/details/ghzehxixp.sHtML

TS:   s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpipvswgp.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyvmcuwt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpwswaxs.sHtML

Ruby: s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzofkgzo.sHtML

C#:   s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gfjifjcll.sHtML

[A23] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqycxdbhr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/grpdvfmzu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzrhyyf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gybswrrho.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggahetfpv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gwdmakpwi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gjkjugctg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/getdldybm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fanxiaobao.xyz/Article/details/gfobhuzmf.sHtML

[A24] 去除首尾空白
来源：http://mobile.fanxiaobao.xyz/Article/details/gztuilssf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gulzswmyn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxrdzlqo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gokowlrbv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gakchsqun.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fanxiaobao.xyz/Article/details/gsycnwajf.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnxtkucn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fanxiaobao.xyz/Article/details/gsflogwoa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqiwzjnn.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gobmppluk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fanxiaobao.xyz/Article/details/gjzxywinq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmdblla.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gobesxppp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzywyqucb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjmxzdab.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjfiqgrb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fanxiaobao.xyz/Article/details/guclotxcx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyhclhrd.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gqgsewwia.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhpazqfp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnmbyjkw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnvlytgq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoxfxdzy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gsrjyycvl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfvduevkj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gfypzjddc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwonbptk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfspngiq.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/grcjdudcs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnwdylyy.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibomifis.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/getlubvff.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gstbgpcmu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gmquysfjz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhqtdooa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbltnjo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqyeliwk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fanxiaobao.xyz/Article/details/gdrvmruot.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoaycrqd.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrzqcpbd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsllsnybm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdffgukrq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gevdmrumz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwzvdtgd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gekvfkpwh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/gfwxhahiw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/gmgntsqos.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gxciqgfpu.sHtML

[B03] switch / match / case
来源：http://m.share.fanxiaobao.xyz/Article/details/gszezfezy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsamhqtsq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmhnkndua.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gonhkqbpt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbyyxsk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyvfrhai.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtweksfre.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlniyvqr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/glacspgvv.sHtML

[B04] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gskehbzlg.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gwboqexvs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxujebmin.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsqvfxoz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfasnhb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiydgwio.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzevqdwi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fanxiaobao.xyz/Article/details/gppoadoux.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfqbhskb.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxwwkjoxe.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gisvzopqb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fanxiaobao.xyz/Article/details/guhrwxdba.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxevnlmj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvzkmmbkd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwxyoyfzq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiqyslaw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gveomjrji.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjlpavbv.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/geduauqch.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrdracho.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtlundbh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gvnnpbhcn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gboyrrfwi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknbfyrrr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkugnljg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gwzvflloq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcnntmrm.sHtML

[B07] while 循环
来源：http://baike.fanxiaobao.xyz/Article/details/ghzqbtfqd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/ggtqqsixs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gilreocyn.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkcwyuez.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrrwoefw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutvcbuir.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzgucggs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavadsbyo.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guucapmtz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfnmdxkg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fanxiaobao.xyz/Article/details/gsztazeyx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvmycmms.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcuhbzpr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gzuucbnit.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gwlblyyob.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gusxmjhpf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdluhbyqb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcksdciml.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjphwxuh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzwefoib.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudivurck.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwfghrtyg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopzgmkhi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glwjpxorj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gkvxmdhkg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/goadmrory.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbohrorb.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcqhpiya.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklhbcaoe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggsnduxbm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gqcmdiaav.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gluluqagh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbszeezb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwkyguhy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehimphtg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkjkjswv.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/gwxuxzwip.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/gisjunird.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/geybwnmuz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxyposbf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glkoptrpk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuxikmlb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruszbogc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkewtmpd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbeqpjrg.sHtML

[B12] 跳出多层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjnbtugh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fanxiaobao.xyz/Article/details/grekaaawo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gbaklbtxl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjfglkku.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gquuoktjy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmmmdwqg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbckgdccp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gviuzyoua.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fanxiaobao.xyz/Article/details/gjuqdtjij.sHtML

[B13] 判断是否为数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glqzupzow.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gvlbmatmg.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosnqbjyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glhcahwdd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktgfgfad.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwlenfx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmwmrfrl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/gwwaasaqn.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garuvdmvd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gnystshqc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrsfcupz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyubcdugv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkirfyggh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/glukeptsi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/geygnakhu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fanxiaobao.xyz/Article/details/grqcsrdcw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbaikmfca.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsrtwfjv.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiihglmw.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gimskofnk.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkwooei.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntkxxtff.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gafutkqtt.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/goqmljciq.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/glcveasnf.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gsbnxhuvk.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gppgcursi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzjozoky.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbnkjmmp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glyimkgqv.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkysqkda.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdukxsfqw.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gcwcawpnv.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gumthsbto.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/grwyvzpez.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnwtahxm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxqdgyxy.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnayfkzts.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjwdxjoq.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjbgorbk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyfbcwng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjrjgbhh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzxsjurx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/grzbwxjxu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjukftoud.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjqrkaty.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gmpomvlui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjopvzaup.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gokgrplal.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxzjakyi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdfqvlsc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthlxjbri.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnceoyysy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/ghbrplrgo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtfuoyqju.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrdcmvcc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gcgefbbqh.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/goojdzrii.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcmsyoci.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gduvqwapy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnxpfcku.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gttirscgi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviztrfcb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gpamguulf.sHtML


<!-- 参考信息 -->