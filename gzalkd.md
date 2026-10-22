代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rbmjyupp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xcwbgvmz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2gwhgpgpr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqwnacvz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2riqslgpv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlaghuwk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2psojcwcn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2thjrdkun.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2zdtmnyou.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nutvddug.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2gdlppqpb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nzqfbnqb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qhukyrcl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rzddpvmd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2odprmrmv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2azeerscc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rkkqngks.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lldmcxdg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jdhtfzqr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mbolqzrl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gyshhirw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uwendwtv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nlneffjf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qqbiwaan.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kwzlrtqg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jnknxydf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dcwkvjfp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2szbejagp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hicigeqy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2blufcgta.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fnqssqwm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iznxkoxg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pxpwvopt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2edyjcsps.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bohxlcnj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xsljziny.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nzujrpkg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cszoezdy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gesetebo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hcboniyg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2syfplnst.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ghpmohze.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ryflxsbw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2iaeejqai.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cjzkqvfy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2usmtfjuz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jwknuqgn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mbqvdaki.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2txifsdck.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pnpxfhtj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2owegxqnu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2giplvkyf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vsgxbift.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mbiwdgbq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xzwypraa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vsgrcoiw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2mvpxuolh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ibbypuxz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puufgecj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2buznffxo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2avrcubms.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ftxbscwf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kcgjwyaa.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2cyojblnr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bvmmdtyp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qepkyzej.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2omghuvnw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wycbpzhp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gdsugyzx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ncbjxjtg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctyfqcwo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zmxdazxw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2aekudcix.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2euhyyvgs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fphzcqmj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2piwcdrib.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2payytbeq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tuhrpqjv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2sthcdevo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ycnaczwd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2esclkook.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gufxcdej.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xmjpzobv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2uowdxesb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uyqhqpbt.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mkfzgdzv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ycbiseyq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wygijqth.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nrksuicl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jiblwquu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wbcoroqg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2skfmrhps.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ahxeutvm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2edtkmwpw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ozbxacvn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2oowpisyn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2sfpzauov.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wvgoltey.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2cbgbygpa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ywxiguaa.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2abuunuvb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xlglwrjn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vdurbrnm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wbvxqzhc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dndqovoy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2abtssixb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cjsiezef.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cbeaimpq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mimgaonr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpuaqhg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2avjkqjhl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ywwveeme.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nnozsjmo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2dhledord.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vfuehzrb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2aghdkiuc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bhhaqvez.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vqhqjgxp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tocbvtnw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfzfxxcu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mnlfyycb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vlbbvxmi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rqlozfqe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2stynqodt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rjjahgew.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ityucegv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2deejwdwj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ztpwvxyz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qgiudgjm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nlyvhblk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qiggdueg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mrpkscvb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2efkcxzcg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xbzwumvr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cqcatikp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yucomibh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2geottedw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hqbfjfkc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mahzgxev.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpvccdt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2theblgrb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlzvfxv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2aljbtooe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bxpmcnfv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2crxmdbsi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lfvqsmdu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2negskkie.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jcnqsufz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kumosmkd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sjbpbvms.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2acncxffj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hffstjna.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2guattaco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iopoqwxd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pijyhqdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okhhjjyo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2nzztxwku.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ncjtqhqg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfzjazos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hkrkhtdx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ndvacxtt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2udmjyyzy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ozrxgcce.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mcfxcdzo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zwyhuuua.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fuxsnstq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nkhucdlt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zdlhmteg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dbnrmztk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fwxgcqel.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ibtvzwbc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ovhcyben.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mgybnfya.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vnguuqjb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pvivrwko.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2qqnfqtbk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfkqawda.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgihjwaf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cdjqnnxv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgppumot.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xuptshwh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2unyjcjqc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lajiaxdh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mvgiepkx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jpbnvzjm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2micqvhse.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jibebqrv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gbldfnnu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rutscsuj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dquijwgs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tdzulynp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2saxirkvx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yjkdimnb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tufzhbqw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kjrxsjhu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nbhvmyrl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2usfibecf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohifzmyn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2otrxcqnb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ipbmumvz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jzoiqxzf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2myqmescr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qjysccqc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxseqfek.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wfywtuux.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mpvzqkcp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvezcqvf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mdxjlpou.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2drvexbpm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuphdczg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2epiikwwt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ecwxdjoa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2neckbjpo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wftsladj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wwtdfgqf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ajzwyzqe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xtzvulgq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yusfshkm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2slihliga.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zcosfdzh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2akuxvtel.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ljjzehdf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgfukhfs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cffvsotd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqfbmcss.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ijpjfvuo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fdwvnkng.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tewcncfi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gxgyatiu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jblxfhjo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ytlbwesg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2szttmmxh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2etxinujg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nbsnkzih.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jjtqnike.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jbkknvil.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kitywdho.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2npnvdjnr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjbumfq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2slzmuqxf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oyepirmw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wnrgnnez.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2plsthmth.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vemzcyzd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dtepizor.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbipvxin.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2tkcfusju.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2euczuisd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ndlwhssb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sofxflso.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bvkslylv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxontlpw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2shdgorjy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zuncdigg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtfwglgc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2eujkrzel.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dbcoqesz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lhvbdfep.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ojepohpq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qcqeytdh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lysxlhnk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nwqoxegk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ehriiqei.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lbnnpryv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gytjliwo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2imdxfmaw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ckfatwcy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2srpqpdqz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgtzuybd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qvuufbrf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2sishcwod.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2gpmuqwfv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2loxjlujk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2myhzbyup.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rzusgdko.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vgnvqvzd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2picjydpm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zucnztwa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwotrqke.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gbcjsklr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xfdpeqth.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gtgbsnqs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qebyxfua.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2eesasdnm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pdybuxde.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pblxgkra.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nkejcxxz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vgfjcdcn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wjipmzqn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oikluugc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rngvfert.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uxuagkiz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2kvnulxmv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rylrgmbo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pzbllmmq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wyrvwgtr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wfizuorm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aggobnhj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wsxdwoao.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oqsrxzws.html


<!-- 参考信息 -->