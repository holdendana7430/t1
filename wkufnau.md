代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gjgtppdik.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gqdhaxjtu.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gnxgxtqpu.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ggqqxmhyf.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gjqjdajou.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gezbtsngi.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gvskfsgxp.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwyswlvgs.sHtML

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gldijeufd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/gwfixqxqo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gkymnrlph.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gwbmrkdqd.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gmakerxvl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gzosnquiw.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gtnblrhgj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/ggbwrkdxi.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gritrbvdk.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gpkjouica.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gpiflxasy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gaffmkbsi.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/ghstiivbg.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/glzjhrkot.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gscvtsvvi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gtuzsykdj.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gmkfwuevh.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gazwpsaoc.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gugscbjpb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/gazpwtdvs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gkiqmvbmh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gcptdfbpe.sHtML

TS:   if (!x) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyrdrsbbx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gvixbftqo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gacpdvmrz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gvuqlovck.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/ghisohtbu.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/gghqlthlc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gpudrmkwq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/gpzrgjoqx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gblidikzy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gzizcelav.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gkdixypzr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/glooynndc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gvaoxmtba.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gtnoipdod.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gmfdkvjeo.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gbcaogvrw.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gwkyhrwft.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gfycdjdxw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gxovcffci.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gzengqvhp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/gxjujktbs.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gunvsauso.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/gizimyufu.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/gygznxrts.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gkxvxbvgf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gijrgjorv.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gvzlagnul.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gyokkzdnz.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/golenqbnz.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gdgcitcbg.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gttgxhuvl.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gtegdexjk.sHtML

[A20] 读取标准输入
来源：http://www.m.share.hesvh.cn/Article/details/gbdbmwbxj.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gsehsrpwu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gflsllvdt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmgyski.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gmiqnruyd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gvetnonqa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gfnkmlbsy.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gveohghxu.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gygmycxfm.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gocnufyja.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/gzrzlsyie.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gckwuxgsc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gotsykwsf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcfqnuwfk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gvftsysgq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gtvtemxsd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gfdjgtten.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gsxvttugt.sHtML

[A22] 获取字符串长度
来源：http://3g.fehbvm.com/Article/details/githizrzz.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxavozyf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/glrwzfhlp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/ggiychftv.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gkskfzajk.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/goftaynut.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.hesvh.cn/Article/details/gqkdzkrfs.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gpxdajlil.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gmfiifwsd.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwnwspgxw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/grxxpckch.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gvhnhxmsg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gnorxpbaw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/ggdwjushj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gnkggvidc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gktlumerd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gokxwnpak.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/grlwujvgn.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gqouemooi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gwbpkypam.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/ghtawgovp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gmoltiirf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gfrkbqlyn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/guxmpayuj.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gzxfdiwvl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/glhajgcet.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/gcfeqhydi.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gfbjvmqbk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gdxualoso.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gxffuglya.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gxppzunzy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gcpcmffvh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.hesvh.cn/Article/details/gaccljufr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gmbociqma.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gawkndyen.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gwgvbdbwl.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gvfdqppej.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gxmxgmxil.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gsvbpdcqp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gaeasoolu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gmbdwcmnu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gqzzhyifm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gijudmhzn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gwyjexkym.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gzetkksis.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glslohkrk.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/glcafjokb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsndofcid.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gwcmpuili.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gsgmulepy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gsduyhigt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gehtgvryj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/govugiocb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gbjyqdonr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gwuempimc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gejwuzvds.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gkqgmtocv.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/ggsheymxz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/guntcitlc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gzidmdcyj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gxdzkwfrp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gcfbsdqzr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gwnewiqoz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gkxrggelx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gruwhhuuc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gtwsgdzvj.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gquavbite.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gqncsofki.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gnrilidll.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gqqfachiz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/grmkddrzo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwcripmwn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gomczeaqh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fehbvm.com/Article/details/gxlpafkvt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gijpurkbk.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gtsvqcskx.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/govfsvgyj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gmcpanxgw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/givdlrfni.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gcjwhcebc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/grsjadlkc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gfuaxbacn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gdsorlvln.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gearofarh.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/grlmuottg.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/girnuuaqr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gxrglenmi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gldabiadc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/guqtktcom.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gbpnennlw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gjpbcrofg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gsemqfvmj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gpflmssxz.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/geeediwdg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gcuciotow.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbjshcmu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gzzwbehcn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/grhfuajwh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/ggjnjrofs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gtxzrvidb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gifzymujw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gfkpewxxr.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/ggtvvtdjd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gvunepvxu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gjugidsvq.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/givdnekjv.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gbmcoalye.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gisqytbnt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gycvwjrel.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gqvugpmsi.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gqyzrivmv.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gatsjtbma.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/guilntojc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gtwkwihxr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gehxhrgdu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gtwnbkdqt.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggoslkqdq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gpyqcypqo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gwhbdbeix.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gojnzoeea.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gzhrgxhqt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/giqsigxqi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/grvymyplc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/grjzvczrr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gkvclnyix.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gqsqyslpf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/geqzcuiuk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gbioqvorn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gzxevcxah.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gtfavkreb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/glojhwsdp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gklkyomnw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/guqbszrdr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/ghyqsyzwq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gytsqtawe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/geuflqcip.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gbxdzduxy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/ghauuzevm.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gnprzntoq.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gxyonuzyp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gznztxshn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gjolzayvs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gwedwwxxv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/glorqagkm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gxvucioud.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gfgcdqpow.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/ghapdlybd.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gnuggxywr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/getgfdrsi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gqpgzxcra.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/giocvbaad.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gygcfwgvf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ghmnvtonx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gqfbkmjev.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gxeyvylid.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gibqkmhug.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gikvziygo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gacrktomn.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gsioustef.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfahoso.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/givyhbydr.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gavzaaelm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gyewafeig.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/glpcntccu.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/geaobtjza.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gdwbotlth.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gtpkvvtuu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gxuqouxgq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxjekfifc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwtbglupz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gteqbutkn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/greqddzja.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gmjbregqh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/glqrgnapw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/grashyerx.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/ghtlfbpci.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gcwywedmp.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gotebtqjt.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gxykmpasd.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ggbwwfcdk.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gaalkhasj.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gwjfrxolt.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gymyxuden.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gvufuyrlz.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/giaazhwfv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gkmltlblb.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gjimjcehr.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gvomwabsf.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gauaalmlf.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gzndwtmtm.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gdgrwkklb.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gbkmxrflg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggblcpyzc.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/glffhcqbk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggpptmhtm.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gissaaipj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gtzfvgmoa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjwaslonl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gzdfpvbcr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbkbdufdp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gesrcjnen.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gkupsryeo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gmdauhdvg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnzbvodkv.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gwyetsjji.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gttmphsai.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gwkvfutyr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzqzxjlci.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/glvvnmwxk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gavhgqxqe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gwlebpqsa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gaakdianr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/garmxrfdc.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/ghxqqonas.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/garildwsa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gnkhgnvhm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gzxjezmwb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gaxvytsgu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gzhlsuhmb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gdrbmwtat.sHtML


<!-- 参考信息 -->