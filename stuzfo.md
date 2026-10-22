代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tpvbmqzb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ntgbdayl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jldeluho.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fywsrycp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zciowidt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gprqqpgf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2whfsxytl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2aooanrox.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oisldkoy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mqosdmdd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xubjlgjl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wyskhskm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qzulieup.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iykisfco.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jtphsaiz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2euikrwkw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tjjgvjct.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2elqqowfk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ghuudwwe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vucyciuc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2shedraax.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bzycchgf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ekqhfekm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2piiuhbgx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rqxfvnjm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jhkhxdnf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2orfazujt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rokdnrcr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ykopyphz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bvsnujwf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ekjnrkqw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cxbmijqt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yszukowv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2oujqgqgi.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iovqqsbl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2plkcgaka.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ltfjntti.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fmomavgd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rtyppidz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vxyrzzyx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dybfxxwd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2loxxyiri.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jaezkyyo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fylawwbo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ekwowcnv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jinbuecb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2degomqng.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pdgbgowz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2yfennagj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rmtmwdmb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgjuxsiw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atddqmka.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2vemohvye.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ffiqriyc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rotpwjuo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ktimsmfl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tgzluvno.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ekvcyiyv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqibqgbj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ruiijkhj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfvtoyvz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xiuqhoha.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qqygmdyl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mltclsba.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wdfexlyo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sfpozldb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rvoluoly.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zrmvmxye.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xjcebgpp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2sdqgnfdw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2nqlpxuia.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qbuqqujo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2spclahpv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2suvfkzqp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bryrhmtu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2brpresne.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gqjjaked.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eeuqxoil.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jfrnkyqy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tswuqewq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pmxyeydv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2odjuwpvc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2rxjpummg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2mjwsegni.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gwipyhlj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qipjmshu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xcqqeolo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hzclhouq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2knssgmve.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mrqtfnxl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dtlrmklg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gutrylag.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bejtyydv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2stwhfmwh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmdorqp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2onuaehpd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2chvnmguq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wnchsxph.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vlescgjl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rofxskhg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pshhazli.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gsfpfzxs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qdubring.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yjdmflgp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmoiuvln.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bzcdowtu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhejdabl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2glaqqcgi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ljhyqbsp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lwxprmqy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qkflfdxy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cjammzme.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2plccrnzi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lxfyojba.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tdkxopop.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdfysxst.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bwsrfxqc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2htefnyeo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2waqkixwa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tqwctcki.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwismouj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wralpqjl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufrlucbj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ipmrukyg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2udqzzghj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bjhqtelf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cunzfxlq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gtahmvaz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2bvrpgjqt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sveknsfz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hagxhufh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vipgbunp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rpxnupyt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mphsbgag.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ayakjann.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wthnzcqb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2sdtqermw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jovnfzin.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjlddtj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jybcrztw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2slbafunp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ebwhting.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2lfvqmegp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2agnxprko.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2znyzcrpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guvfduff.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nxfhpiwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqjxgsju.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vcixpjix.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xctnirkg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hzritegd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vauloefm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rrwjgtsp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qeifcsai.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2virwmbfq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uvsklpej.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nfroxxki.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2uvrevejy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2fzahvnwc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xchxieiu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bsodhfil.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iibkfbnn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bindocdx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwxlry.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wxfitbrw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2divyylec.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zeanricp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2djqfdtxu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vwvsnjap.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2snzlkora.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lacwoaua.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vctmxzgi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ssiusevo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xybcsufe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hmynlluz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gveuzdem.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hgielrur.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkfcvtvk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfmdyrnr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2igtdvrld.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgltwhsh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ecnubepy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vavxywkf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fjvkbhix.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2swwsfzia.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kgnbsojl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjjradcj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2coksircw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uqkbcqwi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yotteceh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2pplyaefl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cvcazwtm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvtwpegs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ilyqzdsx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mftyojaf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuhqzftd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kkrdynmp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2voiudbeg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gnsrcdwc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qbromvjv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2olzyidiz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzcxffer.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vjxwolfl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hcbrokxb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zxgcmafm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gujcfsfl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qvukalwz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jqweffsh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kcpwuhml.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpmhrtuk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqaopxwn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kuistvrf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tcdbzelu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ozpnyypx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xsseldwz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jeobkzms.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iubznhkd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bakrleok.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ttczvdrg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kxeuilwe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gvjzelct.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xbuhpeaj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2idxqdbkm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2okhwofbl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wugziywj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfscybn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldokfmnu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkzzbvaa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2efyjvsjg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2azliqjmj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fmtweqzs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fwdxqgae.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nxzptlut.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yjgfbzif.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2yhkuzmuu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gfspojwx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jmruixar.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mgtadbrg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rzlquthi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2diavdqor.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ubbwmmks.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eytqbvhq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwmdmosh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qymxheqf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xtqxdfse.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qgrwdzwb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bipdfhan.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lyewnczd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2enmvpcws.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nongdwpr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xjloxbvl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pimafete.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fhzqrdhk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2avabyrwv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wnyjfzgj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qytozgeu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nqfbgvnb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2adswtjpp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kheayfrf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqllcujz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lvmdpoft.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zxktufzz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlvtxtd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xbebwtqm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zubpdmfl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rdotodmd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dlwgrrnn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpejpin.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2padtpswc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fpvvoalu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zciuroev.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zyrlcjge.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgguoomv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lcdnqajy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hologwlu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zscqixzl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iejvrktt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pgnmusmr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pukxzhzd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ibfeeqew.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mylobkft.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dgmajjju.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tppgyvrz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jstuprry.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2lsgyrtcl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueesoins.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pxxwubua.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ppxexwwm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ockohakc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wlztholw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xkatflkk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2udoabzvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruugshly.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2slcxwbvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxbecexo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qmmrniwy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2owuojiem.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppieshdo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iftvcyum.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ganuvzsm.html


<!-- 参考信息 -->