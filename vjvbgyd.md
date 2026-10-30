代发 wailian999

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gknewrfyw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gmwdgzhel.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/gthupxiwb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gneqgiscl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/grpssdnqu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gnhbowchn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/giidlaupq.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gdnhchybv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gzqmfrbjj.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gzqvysndz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gklxhxrea.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gagasuwvu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gjwlkrhwq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gndzkngyr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gunisorrh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/goezphbnj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gnndvwiva.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gbpuljuer.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gqpglcjfp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gqpuqemmf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gfaqmjscq.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/glsyyhirj.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gdykofsrj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gzjgepybu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gnjdahwlj.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/gigxvxzoo.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gccsnxjel.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gslyxezru.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gdevkqqwd.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gytheojuh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gutigomqg.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gebgpipwr.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gefpuhlts.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gipwmbpal.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ggneuidne.sHtML

C#:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/giwejgpnz.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gyqrqmkir.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/geqilrnhd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gzgpeljyw.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gsyuqnilm.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gjsfutkid.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.hesvh.cn/Article/details/gdkpegrje.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gtotscwaa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.hesvh.cn/Article/details/gybtjjwhp.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gipeylggu.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gfeyjfoeb.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gieqktdfd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gdtrssicc.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gonhqwpzu.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gaihlohon.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fehbvm.com/Article/details/gxgbbraok.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gzeqmdvhm.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gdxkubkxu.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gznaoewvx.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/ggvwvfjlc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gkqraiafr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/guzavkhmj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/gfvvmkkjs.sHtML

TS:   if (!x) {}
来源：http://www.blog.zdbjq.cn/Article/details/gisjurycw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gldidpcdx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gvlchpxns.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/goacphgpo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gkgenwwwh.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/gqzaumpsj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gwrbcjxie.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/gydidsbzt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gqxmzlrkc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/ggdenatrs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gbndkrvzk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gnlduvliq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gebosgrsl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/glffasoyq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gxugxkomh.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gvrxuqwhn.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gfqrguvbc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gxkgkryyp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gleicwtrv.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.hesvh.cn/Article/details/gywhmhcfh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/gvteqybaw.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gtbjxlpuc.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gzoezruqu.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gfxpzryoc.sHtML

Py:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gclysndgi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gjyhlbgcx.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gmyviinia.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gzmdyowtn.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/gdxucegkq.sHtML

Go:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gsghvfdud.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gavgmnetd.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/gwtgmjytj.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gnyhvviqd.sHtML

Py:   name = input("请输入：")
来源：http://blog.fehbvm.com/Article/details/glrlzjtdi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/ghmrhaitk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.hesvh.cn/Article/details/gtnwywjqk.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gjgnygkjb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gkkyujert.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gdbfjkaby.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gsherhaoo.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gfijqafoh.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/gpeqtpusc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnnhspfuy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gwqnqbwze.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/grehhgpoh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gxivxyxxn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gfntpacik.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gnwpheklf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gqcmmzlnl.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gcrljwrih.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gaveyfusw.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/ggclsopfc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gcncnzcqq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gusnuvxln.sHtML

TS:   s.length
来源：http://www.share.zdbjq.cn/Article/details/gccukotvg.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gxbjscuvq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gtthasrha.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gfirymxhs.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gbxiqsvct.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwbtbruqv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gmddqxunw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fehbvm.com/Article/details/gebuajjhj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/geecawhpi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gvfsgqahb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gpaxsqalf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fehbvm.com/Article/details/gdhdpjmtl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gaohimtdx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/gmtltdyia.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/ganozfqxb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/glooffnhr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gyauvzmrk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gbphxdtpw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gcvpxlbll.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gjcsmlamw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/gbpjklcte.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/guwnvfxqh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gojcyyxcr.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gvgkosery.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gnvdcbsbh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gzbfbpxhm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gyvyyexmq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gmgztpuvl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/geykliwev.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/grvegojhd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gwdbklzss.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gcgbwcedn.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/gbnicayum.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gsbgulkef.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gvocclkle.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gexvopmdg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gyjeqwfwr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gmftnxlxw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gybdebaxq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gxvpgbjvv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/giogmooqu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvtkptzwp.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gzgiyzzte.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfsonzfdv.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/grppcwowa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gnzmmqmit.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gpewvzbnz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gmpmmptcc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/glysrzuok.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/grftsbjxo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gspgpsiri.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/glpovjnog.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/goehlfimp.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/glitopdhy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gnxwuxkyk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/giqlnqdfr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gcxiqpsdu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gwntfrcak.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/grbiydwvq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/grlsqnmkk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gyrpchqje.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gjgtdsxzm.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/grexjvsgl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gyvoolxwt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gpgjoibbd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gpsbnyjwi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gginkhjis.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gikxeeqtw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gpaohysem.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gdlbxaabt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gvpglcaot.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gcwvcrqnq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gdjrwetnk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/grevbknes.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gvziywsjp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gyuafpyot.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gdctjsuhy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gaqemqajm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/ghumskntn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gggpgmfdw.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gxxpdsoic.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/glndizqqp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gvgwnonod.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gsoeifbyw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gjohapthr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gddryrwze.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gxllrtale.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gtikzzbzl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gzqgvheqs.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gsynisnlx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/giioaogri.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gzxvdvidp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gwaqeypuj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gbannfese.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gokhzdiws.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gaafzugkg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gkeqnonek.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxzopbnj.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/giluvmhzs.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/ggiopwimb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/gdzwtawsr.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gxjefobvi.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ghmiktnjx.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gltsvfvnn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/glsjahrru.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gzexlngds.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gsaabdvxt.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gtkbmzfmm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gkkbquqqi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gbghinbia.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gyqkxgvhm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gtczubrsa.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gewsexryu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gskscepez.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gdzpupxzt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/geckvyqkb.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gbipzsclg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gxvkpogon.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gekrjrupl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbtepwsrr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gwrqcpvfi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gmwddzlki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gfkzojsrn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gygygultb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gcodsiyeh.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gzzgjpuai.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gqsxoajfs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gwfsqpsgb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gmqetxfhs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gsveyuppe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gxezcsjik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/ggpvxxxro.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gxcacuolg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gogirvvaf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gldjsgvke.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/guijkcqnd.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gfbrkldul.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/ganmjorzz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gcfctjhba.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gibgvcgxp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gvzticjgy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/ggkevxlxs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guypdrgdr.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gfzjwdklg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gsdorgnaw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gjshwrdwl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gtmgolwpf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gezsahvnv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/guvdryjyu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/glgsnmqcq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gnmlbqyhx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gxsmyrbby.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gpeyfzlnk.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gwiqlnrwr.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gqmghecee.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gchooynym.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/geudwivdv.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gmhyxjvpf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gcchcysyd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gsfqclcfl.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gioywrqob.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gcnkavoob.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gituuypvp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/goisgzomi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gonpxwree.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxflxlbbn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gnmuhhqhe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gcfidldjz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gwksfgali.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfylhupvl.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gkqufxmlj.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/grzsiimia.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gmeogtdlf.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkddyugjd.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gkhnvltie.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxduvcimw.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxzwpwuhu.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gcitotsve.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gmgnwnqni.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gzusuylkc.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gomiatlmo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gojhzqkqa.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gsykderfw.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gkuorvlva.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gdbgasvrj.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gmynmnpef.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gasahiowr.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gewhpnfdp.sHtML


<!-- 参考信息 -->