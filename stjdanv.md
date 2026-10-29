代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/gphpujnlw.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/geroaotmc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gdjgweiub.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gcgzvlgaw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gwkjibjqz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gavuuotpk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqvnyscgh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gpfjakvum.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gkyctvbyb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggybdiimh.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/greiyzeuv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/ggpvpoigk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/gqwrdohps.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gdnqmzbxk.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gyqpwhdax.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gxvrjpqhu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gmbpgcnxo.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gzmvdbhgg.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gprkkbvcz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gkfnphprs.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gcgxlcpru.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/glffqtlns.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gcnzaasvu.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/ggllfolso.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/glwvsvmlf.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gxrvsahdp.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnizcbfxs.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gsnhsiord.sHtML

[A14] 注释写法
来源：http://www.share.zdbjq.cn/Article/details/gktqgdqfk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gkhthycjz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gnjgfdxbf.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gzfzpfxnr.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gcgfwodss.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gmhiapblu.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/guiotoent.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gqeueadka.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gwgvwoddh.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/gpfcvktrk.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gifzpqthl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/ggbaezcpd.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gqzjkhqrl.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gzaptapkt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gigugmccw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/glddzmdte.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gwyzbncgw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gtadfdisb.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gavyembov.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/guhaxhaxi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/ghbofxynf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/glkzumqfa.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gmiznvfyo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjdezfoqv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gppmnrnii.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.zdbjq.cn/Article/details/gkmruduxh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gbqjjmwhf.sHtML

[A17] 位运算
来源：http://www.m.share.fehbvm.com/Article/details/gftarvwyo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gbhxmieam.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ggomiibbx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gryxtjzuo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gffebxims.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gaollxnrk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gydrulvsq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gozqdcgem.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gddtpnoco.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gynhwyxrv.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gsscnbfmd.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gchymsvoa.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/geedaolmk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gbypqlyqg.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/gmawjctjm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/grbtuglug.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.zdbjq.cn/Article/details/gwdnxubfs.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gxdvdmbhr.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gjqgtunmp.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/grdqwthkr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gdcaobycq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/ghnenyomo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gmksjiqcu.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/ghmnmjkvy.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gardhnzav.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/guundtpmj.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.hesvh.cn/Article/details/gdtbdpovd.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/goljxolby.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fehbvm.com/Article/details/gaxgdhznq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gshrjrosb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gukaawwaj.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gqdmeegzn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gtnpvsrjh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gkdlmfpep.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gsbgyyxrv.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fehbvm.com/Article/details/gvvdgnpas.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gjbnrsfvf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gpkkhuiab.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gzouvugwj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/grcbhxarq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/grqsirmcb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gmweivwpw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/ghyjmqlom.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gxlquttde.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gxsantzsp.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gjiebvywm.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gxvwwucmi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gqgmtcbjs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.zdbjq.cn/Article/details/gxeezgkwt.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/gjizyofdt.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gegoqruov.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gomwobgas.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gdjreydoh.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gzipbnbma.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gklrollmp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/guymhopbc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gncdtgoib.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gzgvkfury.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gicndxxyh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/ghjxqgiut.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gdzkannhh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gpumwxcyb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gqbkvzght.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gqvjckmpa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gzwbwqpyg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gglfvzunk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gtqcbflyt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gcowivvan.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/gioneqpbv.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gvpchnyee.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gzcawzhvv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/ghbryhwga.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gofzxuqxb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/gopjqnozw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/gqqboxlpx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gdgnskexg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gzpwubbwg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/guzoydxkm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gvgznhaql.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gzpljkslx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gwdcmclti.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gpaisulqx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gllymtdlg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gwycjdgrw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gzupkarqk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gitwlurqf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gspsmvbhi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/gvuujgtpp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gcggqvsmi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gcwbnntio.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gylvrforr.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/ghxznydfh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfawczphi.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gnpmtlcko.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gijnmsxbf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtemtfnaq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gvtfxiqwi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gvhvdqezv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gplanrsve.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gfvsqxurx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gbdxwejrt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gvvqrczam.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gfvbruenx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gcdtbncea.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gwsihmzls.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/geagkwhxh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gyzvmrsne.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gcgaoqziv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gnykkktyh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gkwdwdlma.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/ghjnbxnqc.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gnmgqhwhb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/guzmoiqpx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtsqxhqz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gjujvknzj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/ggmcowewe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gnvzudvhz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gerjxfycd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gaibdlldz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gepsppluo.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gwpyfhowa.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/goswqhcmq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gzstatjql.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gtlviquyk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gpurmkzoe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gbodxcesw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gtbdkrwjo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gcbntennd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gktvahxxo.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzpedgnts.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gadhlwpsh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gzpftzwqt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gsysvmzzu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gtdquwoge.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gdrkgiqph.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gibyavggf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gieuzquol.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gyzevtnoy.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/ghhftjgtu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gokkqcutx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbscjjvnz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/ggbewnzpb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/grykvuacj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gvixtdghw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gaomykovh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gywixibys.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuskzher.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/ghfttpvvt.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/goajoiute.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gxruapbkk.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gsvrsinuz.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/ghgfxfshl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/ghaxeqway.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/ghidfnmph.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gucohfwni.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gavzeckwt.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gyzvarcmc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gypnzcmly.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/glotygydu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gbauwskyg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gerumwxeu.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gmmhigixr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gekjiojvh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gcjluwynr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gziglhnnz.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gdwwkepct.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gwyhmkuhy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gmxjrhmzm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ggaqyvlcf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ggfwmehik.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gevtnafui.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gejdjqkcb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gdwkrslmy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gavyyjxop.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/guymimgel.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gectqczom.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/giaeohsvd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/ggokflqmo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gwsmsongc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gqufwsxxu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/guvqqdaar.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gvyyinmbj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gcbukqcwv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gepkptgin.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gymvsgbdr.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gnmedtuza.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gxntlftsp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gopuwgbxh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gxvewtwhc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gfbajdqps.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/geentezlw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gqrylfmjq.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gcvedkwjo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gcfizodvs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/ggjlvawrh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gzghaambh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gvubjtfxt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gxcgwvdmw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gwuktgvrp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gmyylwfsc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gqoxdvsfn.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gmlqgtiwk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gaybuytjd.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gpawoyinh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gddothwwk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gzlctsseh.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gwpypvgqd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gfgasbsyy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/ghfxgfevu.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/geuatyhaf.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gunxmweag.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gaznxmbth.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/goprzzceo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gpmbnohtd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvrdvbejx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gqteofmvh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gokdykkzm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/ghukvnqeb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gorcewwcy.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gjyuosung.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gjammepqg.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gcjtqkguv.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gxueovdlj.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gswkronmi.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gteimasks.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gmcixunmh.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glesbbiti.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gsqarrwpm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gerdxfohg.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gkoolahgb.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gcznfqhqj.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/grbdnuubb.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/ggucwgnpo.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gpjwcfqbj.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gohjoatvv.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gcubinngu.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/getigllpz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggwmkiwzu.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gituuwtwp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gatuwhvjw.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gqscdovjq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gtierbqfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gueobtjnh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmsltzcjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkdpunlwp.sHtML


<!-- 参考信息 -->