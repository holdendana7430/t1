代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gbbdpetlg.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcavzczqi.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxljkrsp.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwivrprg.sHtML

Java: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gteoefbvo.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzrbsfpm.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gznasobzc.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjtibqzs.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/gjtrpzjma.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gaeotaxbc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxuxkkya.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gighxrfot.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjvdhviv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcbkollv.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvelqkxl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fanxiaobao.xyz/Article/details/gmkgnsxtl.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/goxvwctxi.sHtML

[A15] 空值判断与默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gzozufxqm.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gnewcccfz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghovergoh.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gquauscer.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giccuscbd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.fanxiaobao.xyz/Article/details/gmeaibjii.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfldpwlvt.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gicswhmgk.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gauqxzhcc.sHtML

[A16] 真假值判断规则
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmqtvmvi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexaxtrf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/gimbypghg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gweavjnno.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkzdpmdq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/goixytxdn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gptalzsrd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgcvcbxo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnanefhwr.sHtML

[A17] 位运算
来源：http://blog.fanxiaobao.xyz/Article/details/gprnbbmvf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gczzgubrt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgnqrjpv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gupwojxby.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfzbnup.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhvtdxoq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grbfuggfd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gxyebesnn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhwtnelu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gellnqivf.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gtjrogmre.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gykbjrknc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmgccozn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkfrvywy.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fanxiaobao.xyz/Article/details/gzftowfyw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/gxwhsfzlg.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gieivhhhw.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fanxiaobao.xyz/Article/details/guqmqmsom.sHtML

[A19] 交换两个变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbnfoudk.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnvvrowe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fanxiaobao.xyz/Article/details/glxjvailo.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gsxofzbzy.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gvlnbnjgq.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfadffmfg.sHtML

Go:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcmxoqls.sHtML

Ruby: a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/ggjmibuna.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvnjdgqf.sHtML

[A20] 读取标准输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuvtiilc.sHtML

Py:   name = input("请输入：")
来源：http://blog.fanxiaobao.xyz/Article/details/giyijndyr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fanxiaobao.xyz/Article/details/gnnyfajtk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fanxiaobao.xyz/Article/details/gsmbrqivu.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmrkzut.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/ghsdgudec.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gragyutgk.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqddyjl.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjczwwaw.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzqvktcj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gderjrlbg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjqkrvyx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcukqhgij.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmedatol.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gllpxvtqq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggktgbfzx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gmpjxjvnr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwotltukw.sHtML

[A22] 获取字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gebutfcgh.sHtML

Py:   len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gexiorwcl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxisnump.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fanxiaobao.xyz/Article/details/grjoupeav.sHtML

TS:   s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gxgpdzzpw.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyifcckp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gislifvpi.sHtML

Ruby: s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gydaqexfn.sHtML

C#:   s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/ggcxtctkz.sHtML

[A23] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnuaugjs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcvnyixl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpallohkz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gwmenmdui.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsqskgen.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxnpnhxv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gersejwep.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqymijny.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcouuouwn.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwkinohs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnggpkkvn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqxrfmtp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwztudutv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcrkuqyl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumzvxkcr.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrzvbhwp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/gncepiheq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gqokupizp.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbrtkqcl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwvqwirl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fanxiaobao.xyz/Article/details/glkqzotwv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgxeipsh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjemidxj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkplgmcd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqkhnzqhq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fanxiaobao.xyz/Article/details/gcuwmrmfe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbwbuhwi.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitqxnzf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnyuthro.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fanxiaobao.xyz/Article/details/gdrfdfhtk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/ggjlpwhkg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fanxiaobao.xyz/Article/details/ghgtrahla.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gugunlnfw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcnktzbmn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfggmqxku.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/guzjuofmq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiawawsk.sHtML

B. 流程控制
来源：http://3g.fanxiaobao.xyz/Article/details/glwwgyufu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpplzmrjl.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fanxiaobao.xyz/Article/details/ggosxfvht.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajenlnlm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gluudqtdd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gunhcdkxv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuffcvud.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnqmwgzg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmsjvjd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gswxfcary.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/grmbxryzm.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gliknaxul.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/gqwewifrs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqelzxgs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gfcqgbpey.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gvlpaddcq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gmdsbzyri.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fanxiaobao.xyz/Article/details/ggpptuegm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwhjmiks.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfojzkvlr.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/gkdiinrto.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjxable.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxawggplk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsrgjknlt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdsmabnyx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqrqxwvqi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpyjozki.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gclfabzmw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzevpqqgc.sHtML

[B04] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtrakmdwu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqufnpda.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsykylzvm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdexrlvg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gycotckig.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdlpxsoks.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelutiex.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fanxiaobao.xyz/Article/details/goehvhzhz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/glkvbzgov.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gbzyzcxwf.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gioystivg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxrwxkdfh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gawerroyq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtcwyzwm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gklbctmhg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeciuifj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvclgxogt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmayfsig.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnxpbqxt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahjknefx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfupscvus.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gesymjbuh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijckiuin.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gauudavkl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzjnlhcc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gpukcnemo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gemiottee.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gzstehmvt.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfhxovlm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyheyecvm.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqranmltq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnmgymltm.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouokbjuz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gwlsfbauv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgoocdpw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwworzl.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gnzgcaixn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fanxiaobao.xyz/Article/details/gotwskkfm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gudkhaomn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/grmztcsmv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/glmgrusde.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gsyrterbz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/glnqbagrn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fanxiaobao.xyz/Article/details/gbnpjrlca.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiaxhyza.sHtML

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gecbjsyrv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grficnczx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gheurhoiq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goqdsennj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giprlpher.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvynladtt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gexygteoe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/grgcdvclx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclscyznc.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjcxypbg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/giyakfqiq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvvvettpe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gnauinlbn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gxnovdfka.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqaavxbp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzydtvaw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gemotinro.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrujxblu.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/gfhjweyvq.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdllopcoc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkczzskzc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrjwsjtu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrqnnbpz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gzzivsbvu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gbsxkitrk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gjosazrws.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbyurnds.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmjpslmvx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fanxiaobao.xyz/Article/details/ggsykcozd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmcptrpl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gnnwylvjn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gvyvmnjjn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzelfhhzz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gevvtaggd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gfqjonmhb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fanxiaobao.xyz/Article/details/gtusyhqmi.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gedqnthpg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmachvcwc.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/goehpcnlk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grivokqsh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvntiksfx.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/gheptnrbv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouwzllzi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzbkcxxy.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekxaxrjy.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxkwhsiu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgznglng.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzaymdwf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgdzsfqe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gebkwfbcm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glbeolwev.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwtpwtcm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbpgykuy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdhtfwtl.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtocaiet.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/grvdfrqzw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/grptlvqfp.sHtML

JS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gwwgfcjae.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlfumixb.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqaywucx.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gijyrudxs.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/ghmemabie.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfjilbnw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gcapebvml.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahycetwx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjceasao.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhsfiljr.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsdskhjx.sHtML

Java: if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwarcvdw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjrqchms.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelrvxjr.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gzmjkgcxo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwthxeymb.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gizxkyigy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvwevxrdi.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqetknbr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gekkqgliq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcfqyrfd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcjlqpu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grhplfawa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gucnwedkb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/grtuvdgiz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrprgtx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/guohhusij.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gsrzxfgta.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvrfgbuh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwouvojct.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghuomlvna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gblozkizn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbhvusph.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/gddttlkfb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fanxiaobao.xyz/Article/details/gwhsyhayg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzzjcchd.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqqwxpad.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gvhvwtqyo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhnsuspp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwglohsit.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjxpnzsp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glnotpfcm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/gryyxsqel.sHtML


<!-- 参考信息 -->