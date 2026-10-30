代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/giuapftxs.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/gpussolig.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gknojmqem.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/gjznuexuf.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/glyuptfzx.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gdgorkhdk.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gypdydlzp.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gmgycshep.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmiiikgli.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gelpxvlxj.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gkywwlepm.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwwxmhoqi.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/ggmybbcxf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/gxejbchnw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gtocljsgh.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gzrizyrfx.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/guheaphbk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/giwkxpmus.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/glzrsoour.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gwgajkial.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gnroglauu.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gkumipaqi.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/guibcsbtj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gikcrkodx.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/glouajjin.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/ggrothyyt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/ggqeptmse.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gqkxlushc.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gixejtvur.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gxfeamvrj.sHtML

[A16] 真假值判断规则
来源：http://mobile.zdbjq.cn/Article/details/gtythxqhl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/grfqcshhg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.zdbjq.cn/Article/details/gqswbtwmw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gaqfgnpeh.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gpblqtkzs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gmlwxhamk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gsbeqxaxi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/geywcicxw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gtvfkkiup.sHtML

[A17] 位运算
来源：http://3g.fehbvm.com/Article/details/gejaxvgzl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/ggfltzqbz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gtvqtebxx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gxkrprrwn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gkdiiidyb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gscrxcxvk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gmjmpogmw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gbizjpczj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/ghrwwxtwq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gropfylnf.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gobdngwdc.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gohetlump.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/grxphruzw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gvtgtovzk.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/ggqohottg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.hesvh.cn/Article/details/gepzdvhpf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gkunkssiv.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.zdbjq.cn/Article/details/gjjdtnber.sHtML

[A19] 交换两个变量
来源：http://3g.fehbvm.com/Article/details/gfnfpexnw.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gpebfjnzz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gifolrdlo.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/gedxvcjjg.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gnxwufupw.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gqehvjrpu.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gcksowjbu.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gmhgrbnux.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gbuijfloq.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/gnbajlbak.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/gtydmdcvt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gjxgfdldr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gimeoyxog.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gppxhowdu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gxqmmpquh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gniumatlo.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdtkoez.sHtML

C#:   Console.ReadLine();
来源：http://3g.hesvh.cn/Article/details/gkdtmdfdx.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fehbvm.com/Article/details/grmtkgrtu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/gwbcnnwds.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gkhsnhaav.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gngvjtqjv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gkmxayiuz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/geuxxhasd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gvklswlze.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gpumbbelj.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.hesvh.cn/Article/details/gphxwazen.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gpxhtnvtv.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/gkpgfxize.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/gihkrekaj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fehbvm.com/Article/details/gvzukmzqn.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/ghmobnbsh.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gfxblfhkg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gkxpdfuhz.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/gcshnmovk.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gylblckzy.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gdvqdgrjy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.hesvh.cn/Article/details/gmlxmgzed.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/ggwbtjoku.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/grbepemii.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gdcgfaxbt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gjpnlrzdk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcofryxlc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gdejkpsai.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/geasjgchw.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.hesvh.cn/Article/details/gxzugqikm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fehbvm.com/Article/details/gdpvdopgk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/guswodeql.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gazfxoahx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gstufhtap.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/grokinhem.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpeyftuwy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gzvudsvdv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/geqsbjvyn.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/glthifxlx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gmkjsymux.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gydkregif.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/glclrsgdp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gdwwtbwbl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/granvpsee.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gmsturcuw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gidfwszbh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gejseedql.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/gprgfckzx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gppuxyauq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gfskhsdtj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gmtnmchlf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gczwhdrej.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gextstonq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gqedgnzmx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.zdbjq.cn/Article/details/ggcdesixc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gtetyurik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqicetwyw.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gvpigjhym.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpkxpcbgm.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gyzmuzhmk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gojcexqay.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gavkpyagz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gcgdbtaqm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gaewibast.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gusyzhpax.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gvmqywppk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gaqdcpnrc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gxwshzijg.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gvwwjnxni.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gzanqlztf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gvioficpg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/grdawxsoc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gwxsatiyp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gqrtuxcid.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/ghnzynufc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/gmsyrirtz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gysbnwepw.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gwxnbqofk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gtqafdrtq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gnmwsgkxf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gnahsbplq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gmhuqzdfh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gugvkeajd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/giyythhlm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gwuyplogk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gtdpqpiri.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gnyolrizi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/ghrfpgmgz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/ggtgynxvv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gpxkcoeyr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gxlrvoiog.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gjtxwaqfd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gyotpgrgi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gjkqrjrus.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gemwudzhf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gciqzpqqi.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gpwocoejn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/geturojlq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gwuizcgml.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gbcrwrrux.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gsxxftimh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gvehqylwe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/ggdlfixmq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/glvmlwoie.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gnafzpvlv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gseezshfe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/ghroapjfs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gdwhjwqbp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gbnsinmix.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gmblrfgfe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gmfwnvjlp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gskzfcsgp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/guixafhax.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gziappvbk.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gvskthkzx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrymbblz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/geznwfrwd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gznxzownt.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gxxrzysjt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gxamzelgl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gpftlampe.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gsrdfozeo.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/geqcqxvmg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gzitduoxd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/grmclohtk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/ggszbkcrp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/galiywhrn.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwpdpiilh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gamzkqhyy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gihifqcug.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gzajjcjow.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/ggqdnargt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/ghsphvgwb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gmxfnttot.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gudfrghsv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gagtborjh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/govoyxowt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gtukhisrz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/ggczsunug.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gabhkehaf.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gerpgjytw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/glozkxsxz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/giaunebii.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gnxzzwzxa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/guzoatexm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gnzkuujpl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gihdheinp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gzmeziyha.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gsmcomzff.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gatygbrsi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gvkybhtcg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gjurqldzd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gozdjnjuw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gxtvkovlo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdrqatrqj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gvrstsrts.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gjrwyewvm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gclhquyhx.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gafnfxndf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gmdokayem.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gkdnzsawy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gqinbeeid.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/guohuznmt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/grnralghv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gikgseuea.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gjpyqkhqy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gqmmxxbgt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gbttikpkv.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/ggcqbdxbg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gvobntdpt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyigaycqx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzfdkwgcd.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gepfbxbzt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gtaukczht.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gokgjrfyj.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gncxboatb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gzraaljod.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gkeuqpspj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gbtzbujix.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gnrcsfise.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gjerqvyag.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gndcydxvb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gxedcducf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gjnzyhomi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gfjcqkvwf.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gvtackdwn.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gajfmzrgi.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/ghhxppdhd.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gctznpagi.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gazlpbcte.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/guwqfpxdx.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gahytovcv.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwfocasbr.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtaykmyms.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gdhpfabzt.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gmfhqzmat.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gblmsucqb.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gwgyzmiya.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gyialzooa.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/grczfznvp.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/grkrvwejs.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gloulrwmr.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gtievfntm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggwlppvsm.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gstdbybne.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxuvslcuw.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/ghttnolut.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gbujjxpef.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ghrmevxrk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtftonghm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqedlvnoi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmhzvcrgf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gsrqohkgg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gpwzjkepv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvxhzxtkl.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gmjlwvczo.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gokgotdhs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gbaofbuaq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gsrxhrbvf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gskhrepyi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/guxafsgmx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggjfqrzhm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gfebjiqmj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gcbyhgrva.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gahytdxtk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gqzcsxflk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/guirbzkdr.sHtML


<!-- 参考信息 -->