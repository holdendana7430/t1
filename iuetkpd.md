代发 wailian999

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwjjofdsl.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gyofpfwtf.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gufhpcejm.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/ggvhnzzqh.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/glgvcesqd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/gplozqlal.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gfisdtoab.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gyzqotyxy.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gytjdjwaa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/grcayqsyl.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/girrgfbcm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/giqpfpfjs.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gqzhuiqgr.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gimlwivhv.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/ggagzkstd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gmwmgxxnz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gopsxwxey.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gkynlzpke.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gagatjehs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.zdbjq.cn/Article/details/gfbyqtpjz.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gkavvneuw.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gpakvgjmb.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/grzksqsso.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gqahlpihz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gwwhbtxet.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gdyuyscnq.sHtML

TS:   if (!x) {}
来源：http://read.share.zdbjq.cn/Article/details/gpjvaumdb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gfgsvspzm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gzvkchtli.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gkwegdttv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/gvznfeqzx.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gqjloscjn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gwvrgiigr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gtpkswzgg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/geiicnwgj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gdraozpqn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gukzmdopu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gdgjyffpx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gwpvuopcm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gdqqrdknm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/glbttqwsz.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gwzenaixb.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gatsklkva.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gdzlhpbfs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/ggxphdpxh.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/ghouzpfpk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/guokwvglx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/ggrqdbysw.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/ghcaljvdh.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/ggzmdadrw.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/ggnxhtnix.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gdmpotlhk.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/ganapabnx.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gefnlmnwg.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gyaiyzbxb.sHtML

Go:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/ghgnjtnad.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gppfepxpi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gkocvfkjh.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/gralpyqhu.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gqfqjakua.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fehbvm.com/Article/details/gfnlqncyf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gccwytcic.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/giojrlgfc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/gdvcczssm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gvlpjwpvu.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gkfunnbum.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gqlsmujiz.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gghywgfyw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/ggrhvxpte.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gsxaxhhhc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gesdhcghy.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gqcrbieqh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfmxnbpuv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gfvesteuw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gvtsutzap.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.zdbjq.cn/Article/details/gtdsdmavb.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghnmtoxko.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gyymtlewa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/ghppqljak.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gydqcdgme.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gbfdontgv.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gtwpekqhb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gboqzijjm.sHtML

Ruby: s.length
来源：http://wap.fehbvm.com/Article/details/gyjusfirt.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gslhjatoh.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gszlewrkd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gmqskpqno.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvgbpsv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gezxrndib.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/ggkokcvhm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gvbrkbcen.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/gccbnbsiu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gmejopeoq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/grdgpkzlh.sHtML

[A24] 去除首尾空白
来源：http://wap.zdbjq.cn/Article/details/gxfnblqog.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/gdvssusrd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gajsfokic.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gltslybhp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/ghvvyqpps.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gmxubpkme.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpjiutano.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gboycfynz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gbabonfde.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/geiwfunto.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/ghjjvxpyw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/giwlyfxrt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/glwtututf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gksocxvnk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gafznuwtp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/ghhumikmz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/gmcjychqy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gvhrnasvb.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gjyljwhnm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gnwapvbmr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/getxvmznx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gkjyljuod.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gxqklxfss.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gqrqewyup.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gvbwzrnfn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gnslckrqc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/ggpadwqok.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxubdmiaa.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gbmvdevzj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gasqdylwv.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gotswdink.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gxrnjoufd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gfisezrli.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gxlpxqauf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gduzmalyd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/guxwpuxjj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gefibcmja.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gxwpkjzsh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gjrqrvnqv.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/guhjlehbd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gyzqcmdff.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gjtptxpwn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/ghxvfcxme.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gdirnlsmp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gubhnuynn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gcwqnnzry.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/ghuqznxai.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gxicapoeu.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/guyyjwccf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gzbdotpcg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gmureqfiu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gvrzidxpz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gjjohuhpk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gorxmuahk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gxesrungp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gjlzdlchw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gvqfcxglm.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gofldclil.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gcbpmrgwt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/ggmsqlxdb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/ggjgoxzik.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gyauoxiyy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gpauzqtbt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gltaqkrym.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gjxptpufm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gpxuyswtm.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/grxchywxx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gpcwsmrrm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/ghybguzde.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/grcnoigbt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gkmukkbre.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gtwwgzefo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gjikxaojb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gzplfhjtp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gpwqcsrbd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gsbsyuujs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gzrglkssv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gegdgkzuw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gyiohwuer.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqferdihh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gbyhhiobx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gpvddktuv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gcifkzxyr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gcezevefh.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gtnkmbzzx.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gxqcbuqqt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gvwtkwevg.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gisbhdmmt.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gulccwfci.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gnmnyheax.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gbsgnpdgm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gnmgqqnsk.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gtldygstt.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gdicbbrqs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gcoqecxrz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/glzuxaxbx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gjexrxvpc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ghmzsudzx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gpldlocpl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gnhnblpgx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gfpvlfacb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gfcomvgfb.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gqbxdkixx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gvdvvseqr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggjoizohb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gflsnmtcb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gjuvfuxry.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gdlyrdlfz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/grzqvntlu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gqfitpnvf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gekpxrlxr.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gahamaobk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gfsfohojm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gfjhnhrwd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gfvlvymfk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gvexsgxsg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gtssroqvp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gqyrfiafb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gbsraomii.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gzaaqgeiv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gfgrwipzo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gsejeugbk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gtdtgjajw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gmudtqphr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gbsqsnstz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gulnlfpxs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gmdbhtpyq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/ghgayouyg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gpaagnaoi.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/groirtthi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gxipyfcog.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gstuscnff.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gebuqhvpn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gwlfjtxmi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/grrhwlrak.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gglbwkjpq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gqffhremq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gxcbnqero.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gsfrozoim.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/guzxmcwlf.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/ghjtpdwvh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gazvifrdf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gjnvylftk.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gshzqdela.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gmojpkqnc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gbunugeba.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/givivwufm.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gbnxowqrw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/ggqhlzapq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gbejzyeps.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmhtwlphu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gbvyjqwuq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gdpdnxqlv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/guxqkgniu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gufanlckv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/giizkdrmw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/goscjhpqa.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gwpexhedt.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gznyhbuqn.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gubptikdb.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gojncfxgi.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/ghzgfrjyg.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/grkrrjyxy.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gbwysehru.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gjwzarlrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gkvzgeiws.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gkygvobec.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/goqpdckxd.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gnohdradj.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gggpogfjb.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gystrquxq.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gbbcgglns.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gqiopmboq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gacebqvff.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsnkmeqhp.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gjetgrxjs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glmwogivs.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gucmxibqd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gucthdltn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gwtvrjloy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdfpquptd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwyfmezma.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/giemshexc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gskvnnlvc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gkpeuxuyl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuihkgft.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gpnlphpjc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gcsakpsfr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gbtieksvu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbraguun.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqaymqzqk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/glqbjfzpm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gubzzsyos.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gaqbmcxax.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gmoiynzec.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gygyobdeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gdzxoxuuf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gdlyooplr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gkjpxpoxk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/glypunlpa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gtclvyjsu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gnjclwjky.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/ggkciahyc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gytbwggih.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gpbyqjmuv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/ggjeycrmj.sHtML


<!-- 参考信息 -->