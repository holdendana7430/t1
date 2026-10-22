代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uvfyhhjd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hdirsswx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zvvtcxec.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wulktngr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rcdyihvh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cpxgjwsu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2dwuugwxm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2icalsfwg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qhionkjj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2meoajmle.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xlbpqzmn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rwpigvnv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uqmnjvhu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yxpthnme.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rxjxqsle.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2anicmfdx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ladjpeui.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lzxdpcpc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2uemxvtvz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wvesaavn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2okwilkdb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mpfquafn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kdioftzk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pbnmmjol.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cnhrniip.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2umeuefsx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ypxfrcyp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jajwgjkx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2svhmaaqz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffckjmlz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ufmhpccr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dojtxpmk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uxopycih.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2omeeftaj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2isiylzfg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2djuktgnv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jsueiqzs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2sfpjgrap.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zxpkanfw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lncrylrw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lxxpfyfx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kqujxsrk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2impvmmjm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2aomkxtre.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hlwgozbr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hhuitylj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cjwdjbtr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2domsadtr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fwgqopab.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ywjbjphf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mpuivjib.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jvbvhony.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gfhobinl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lravmmte.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nrmpyula.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2guvxkgwp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wzkhrxmk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cebsvqdl.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqtqblau.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2bvyhtmkj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2abeiyxag.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fzmqdmyn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kgkeklqx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2snazscxm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fefdhdvd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgnjhjfs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ndmxitpw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yaypitnf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tyahdwsc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bvqtaszz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zddvdtdo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wucnzrvs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dmltdvyd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kynlklmb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fpewetna.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xzhtmlri.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2paqtgusx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vwypreha.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2eznfnkti.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dcwaeabg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wfsmocyv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkejugyv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2carwqikf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zsvoqkgy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cknbpihl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ciarucll.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2lcxnkhqx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jemduoaj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zkmuysfx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yaaxlyvo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mcixnqhq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bfyjgyyw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2egstztsr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2kjpdqmii.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gayvhwby.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zormfuno.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vxeaudsd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nbhtczzo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ypyolfxz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ojzbtoml.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2odbsobcx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhrsrxz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2enudrsgk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oiuwqiax.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qcnhiuhe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dicwqvcd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iwupbrfu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rxwbehxb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oukpkdiz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nlhufyzr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2snhdqbhx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tofyyswq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hyxcxytc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rcwpezca.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hokrxrze.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jvwektft.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dwilpzhj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mbnbimbb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2sznqafbt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2abcwuzvl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mjgtofpf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rrmxnqgn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2anolrwfx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmppiiq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hheslkrt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2kdifzdrc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2paijvusg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wxmakrmq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zwmcikgr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aqhcvqgu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wfjxgenq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gonhdlum.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hkqvduqa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tmlsvabq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ebhmjjdu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mjdlbbkp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vfkjccpt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxeydxd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzndprzz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqyubvo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2iwiefuux.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oiyevkkc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qdrkiikp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cledvzgt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2czuczgfd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fdkxantg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bryanuol.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mcgabzyp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2twpuefzk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bospqfdw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2lgzpaeoe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2riymbuhm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2etjetrjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wukkqpjg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uvuxpmvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiblquyo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bluwdvbh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2boozkxuq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gatejdpj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xerwvmwm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2glolddlc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2goqfrrpi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uqpgllct.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2urymrtfp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wqzypoiw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cqbtfwcx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2oqpvwaab.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlhhennm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2westhdiw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lnuiesbf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ooptdzke.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fqrscxos.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2peavvvhz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2avjldhis.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bwauiehi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2aelfwpwu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fsxksuty.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltvrufzj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdhthsu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmtrzucg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cswncbov.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bzphmxgc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fwhthvgo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sjfyiabu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lpplkygk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmlezqzq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdkrmjd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tepdlcxo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lscfgvrw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xtyzvdke.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qtxwpkuc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmoenjnj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dgdhlqtq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vquokmup.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkdbmbq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlnorucz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntoyxfrg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oiktepmh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wrfkbcft.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qznytkvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lctfcqfh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yighpopa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jltjuxco.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbhvmamj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2arrokfhn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeumezrb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ykpkwsbp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mczdrkjr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yazcsjmh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vojddazd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hwpyiwge.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxylzzon.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhykkqp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yyornumx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlklhsfo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2newgbrkj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ahzfzpyt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyamccyl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ofbwqwij.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hcmpzqsg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ckozjpsi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ntmbfctl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2agcbifjb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2usneonbr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ctzmeyko.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2syppjcay.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ogzvunat.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xmvwpqqp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zalucojm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gihumsmy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnemrdlt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkdeeegd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhnhckrj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2evezzjqo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vvotykkn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yxjzsjbo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gilfrfla.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xuihpyma.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lpparojz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pfbnrzdx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2alldrihy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nvvutbfz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ownpudtk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pptuvcwn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ygdzicgd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqjgwque.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xsmaudjy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wljopjro.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mzytqkuv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ehkobhbn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wivjarxl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxlkavrh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2sgyeqtzi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ewmxllux.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iuepcfeg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vtaxpbxf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ldlsxbcl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gzfoyvjv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgorzhwk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrbzjlf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jycdhzns.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkvueeeh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2sjuwhkog.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nkdhvmbc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vbtwvlbv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gilnhzpf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jabqdgnn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyhqyau.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rhnpzsvy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2otydhfxa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bdnlqcio.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2isfkmqvj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2subwenlb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gptonhex.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yilcakhl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ycdzcdut.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqalzjll.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecrohwpl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wzkaogjj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2uimixqzf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uksibubc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dugybren.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2etmrrzkd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nduftsvu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gdughcuo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sntghuss.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nhpwsfmt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cgyqlvqm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pquricdr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sscthdwa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emblncae.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bdnzrmmw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ucsqrwjm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmddbpjq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aoegegbb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oohywjhv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dpkjypta.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nnapdjbz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2akjrqxgx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hqgovwnf.html


<!-- 参考信息 -->