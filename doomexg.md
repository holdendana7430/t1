代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gxfjrcday.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gjtyjneod.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gznmokwrf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gzrfayzgw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gyflltigc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/giygfnbnu.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fehbvm.com/Article/details/glskujrym.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gplirpafz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gwtlrdspd.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/goaynhgio.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gfusljhbo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gajstnefy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/glxckzvje.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gtqodsrjw.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gwcfkxcaq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gnabeijlw.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/glycdiajw.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gqtcbpsky.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjnqalwuu.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gkrpckcqb.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gdrintgmo.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/grdyuhgpr.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gjpqqpinf.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gnsjcukpi.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gmgwceebo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gbrdmmxkt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ggfrulefl.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gpzvdbflz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gfydjcvwt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gbdujgegy.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gwdnjanze.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gsygvtfwk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gmtroksnh.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gmoxmvcwe.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/ghwijkskn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gcsoddsah.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gefmhnlsx.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gzlpyfkry.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gqysjlapw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gjlhopuyn.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gjkvuoyzo.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gydvhgpoi.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gvagaarez.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gwznjkpun.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gpgvkvyrz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fehbvm.com/Article/details/gkoftfpkz.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gjzlnsxgh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gdkvmfvhl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fehbvm.com/Article/details/gnuljtppm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gccrxvbic.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gpsoacytm.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gunlupoty.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/ggxsakbxw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gyapijznm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gnsskllpl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gteltvdzo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gnpegljzv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gcobwkjwl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gkorwdorz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gsisiunjz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/gzwcrvfpq.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gysdobuvc.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/giijqamix.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gvbmdgmnx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gffjuqaqn.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/glhzqjsre.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/guehyriqb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/gguqujbdr.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fehbvm.com/Article/details/gkorjpjkj.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gcpmsgvoq.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gtwvbzuvy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gdvfizusw.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gqzsvaniu.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gyxrbqbmj.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gkpkmajum.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gvwhxavjh.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gmokcghmg.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/gdxzelaio.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gzitetevj.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.zdbjq.cn/Article/details/gylqkamls.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gynvxhhza.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gjgkarykk.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gekmbsukc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gjgqdabsm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gwvogesfb.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gscyvbadm.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/grlrgqivs.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.hesvh.cn/Article/details/glplemest.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/gcirllthk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gpgqrlxaj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gzencxtes.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ggghmeltd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/ggnxrbcal.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gsmnuuxiq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gxznyosmg.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/giozqekic.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gkyvjgsob.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/geebtdjvu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gvvpkboja.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gfvtoryvp.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/geicpxjmj.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gpgofndlw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/giwapqlhj.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/ghwmcjllf.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gwrlczovx.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/goyjrsetz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/gjupbbyzb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gqunrzvgj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gejbodzal.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gxnaxjotm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gmtuogspb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gktwdinvj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqeceqxea.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvovvsqp.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/goolywibc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gwalzkzsw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gdtjdkboo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/giofdyviq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/ghdtyatvg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gcrtgnxek.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gvocvgnfh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gjdjkzsfs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gnavljrak.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/guvdmnwqg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/gxijfhioe.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gsofkkotf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/geepecawe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gkowdqjhf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gvmdaayox.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gxazlubxh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gvsnlszuh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gizltkuvj.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gvvraxcus.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gnvkendke.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.zdbjq.cn/Article/details/gzhgymvom.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gkwhamsit.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gphwutaja.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/ggncnptei.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gwihytear.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gdulcukib.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/ghfsgqekk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gofcermkt.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gppcemyqb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqekdulev.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gltpkpxtg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gtvhbdwoq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/govnljpzn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/ghgbzqsgn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gotjrrphs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/glrnrzvwv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/gimolzabm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gkthmmscw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gksflhqlu.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/geqmepfyk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gkzcrcowv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/ghgsegphl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/glctuodjt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/groxvwqvi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gevcziebm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gzywrlwrz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gryirbrhw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gtagcbkmq.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gofglungn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/gpvfchqwy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gkaujhuik.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gbtfrunbx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gknhcyxbx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gtzameofn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gmbnocyxp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gbuxmttlm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/ganjaschp.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gqvflalvc.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/geidugnrh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gvzswfgpa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gtetrcsok.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gkoyrqwvl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gwlgtxxad.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gkkgbaswp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/grakwcmyn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gotahwqzb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gwsoavwwu.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gcquyaxlu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gbllfripw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gijzkuutg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/ggrweshiz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrklovqn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gpdzlmrvg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gvxgulafu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/garuwjger.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gwzalexmr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gkilisttu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gayrkciff.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gnoykxgws.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/guybgcnvp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gsjjtelum.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gnodqgwmg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gjdtcpwkb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gzdjvhxfx.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gairovprv.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gtiwmtzxe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gedkixldc.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/guvxcmgwi.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gforgrfow.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/grjzjvfgz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/glrhsbtwc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gdxogmlmz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/ghhkqnksp.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gghrgarzq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/guecoonlt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjtvxhqea.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gixgvbyzr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/glcpapywi.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gzgxvoaxe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gytdhuqjb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gwjxntqes.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ghblzcncl.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gddnlvdoc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gdpdojdys.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gijdekhfi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gatqglpyv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ggxphvrpv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gyemrapvn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gmuhxhmfn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/ghbuuedgo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjuuhjuj.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/ggzuclhng.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/ggdtzqtkk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gucwkxuci.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/ghwyvyoao.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gilzgfrcf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gxncfepeq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/ghdynstkq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gxvqekzkq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/golrdtyqi.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gvzcrvjrd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gwomwvzku.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gdlrwadnj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gbxzmygla.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gcfabjntn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gzpvkuruc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gioigwxnq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gebvgzhbn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gzfncnecu.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gclitwuau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gighkolof.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gpndakvxy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/guoscznxg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gpjbtkqsk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/genjsmegs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gnouthsga.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gwlejprzp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/grckamdod.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gjxigyxhz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/geavnsgfe.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gwlkfkdje.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gmwlqyqpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gtdywfqxy.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gmbcbzhud.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gdhzddxpf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfratzlu.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gjgzyixmz.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gwnoxcbbd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gcuwhehlm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gbkdowpvl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gecoxagok.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gwlvynvuh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gdbnofffh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/goqzytjxt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gugbthbzy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gvxlecziq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gicbqjgxo.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gsfwdjxyn.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/goyyahyot.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpmpfieie.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gncjzwmxk.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcmngjxvn.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzwsvtqgq.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzhlmdadx.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/glftiijfa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gmlcefqlv.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gnqarpudb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gxozbhtmg.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/giztbutne.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gumddmxsr.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gtkgcxxxs.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gmwxmrgiu.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gxfmekgwc.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gzswfvbdh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvsczapww.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gnslqidqw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gctwbdpdt.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gossimtev.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/goprpvyte.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gufxrezbv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxeombnzi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gbxkzndnh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmxgbzttp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gofxcntxy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gqeuirmgh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gqrkmlbpf.sHtML


<!-- 参考信息 -->