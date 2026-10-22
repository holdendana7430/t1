代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bkzhxpxu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2laxfwqsy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2iccxeopa.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2eaduujqp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tkbdmddo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vwkfjkpo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2caduzjaq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qgijrivu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqoqjqbz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pqfldpod.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2csitifjg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2atqwldnq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fhfwhqpx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2josznkvf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rwinqiwi.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nfrnhrtt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2goxjobxx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zkgwzmzx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2brxvevpu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mzbezlfr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2arekymkr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bgopbzpl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nzitazpc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kqeftpre.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aqcebmtg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2tyatetyd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jifxvxrs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2cggpumtn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ctohrxiq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2odlsnnft.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2pgqlqxqz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sbitorkw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pwsanuyj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qeyeaplr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lxutjacq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdlsecgj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dmrvgfdb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ltxgkdzk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2tlpleqkj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2pujlupmf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ziexlbyf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yzakycbs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkpqwvjd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qftjxwut.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pzcsezel.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zevkepaq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2axsvgswr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jxcwovet.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcoertlc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpvhkgjj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mcqmwjjz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rshkklau.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pjrkfpmv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmbodgzs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wbjqdtqh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2woimaisy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vlidnfno.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ppmpjfpu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sebmrcue.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vscrspcp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fyxqfpoz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dcsytuqj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mmfdhffr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2yazzsapw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tixqydvl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2peccxrcx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2otootowz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ogllalsh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vnpyekqr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vqyecrwx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2exzbfvep.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xxjebfkz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hijeubxv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2magtkujc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ffvcklfa.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2hfwcscky.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uqkqgboy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2blennbjf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jtqgkjaz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rvyznxrj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ggfweksd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2johccbmm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bwneljmj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zamsmhgz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fipnhrqo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2msfiegev.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2knjkjgdm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpgnapgj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bydygkvj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2olnfyhel.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fvmzpzwc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ruwqsaxb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2slilasmz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kzcyoglk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2orcxscdj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dcexjcds.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2awefyjxh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jmteurza.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2slhnowrr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkpjmsoz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ebysmsux.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2szpiijli.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2asltxwdj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gxohxdlv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fbkkhvag.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ztlheuyb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hqkltuzy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mgctiudg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvkiye.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wnaxaxjw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2idtfmtqo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fufjvrft.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwwivvk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cckpaeqy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2enhqapyd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2voirhkgp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2shgynocg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2rtgjekaa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pjfjisyw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2moxdvnek.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qljqaymz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hdfzueoc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipeehehb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovineebb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cscxqbfa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrleufu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jreprhra.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2slanbzvx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lwgazbfz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xntjlysf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxkpgbw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zudfxeoo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2grtwfgap.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tvicybhk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pssdfnbg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gjoiveym.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xvvpngdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilmzowhc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mkjxpdgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyzevmho.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wlovfkmr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sihdcvso.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfadhqtg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wugveptt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2agnammyu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2anzphwwv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gpuebmlj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2frvuwndh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2txrdxyss.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xfrnpmew.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wwngfojy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2rqjkasmt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cghnfsnk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vaoajube.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xqtxbhgb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qnbldcaf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2sepzguje.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yelhaats.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ptdttcjs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zilxggmg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjhqxegt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pdtajcan.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uvcowold.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2klmjkepn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2glgvnkxi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ppjajyno.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wgiarsyj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nvkotozh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lgijqoqb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ykzfblxd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wteujeay.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdjihfhd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2scruwwbc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mhbdpjsm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gdideaow.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqfuagtq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ldpvfysp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mbcekcoi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyuyzrju.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2saxdzukr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nfckmflz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgurkfaq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2svkdpica.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jjbldntk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyoaclgr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xuekxrho.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cfdpieiq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hfebxsso.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgqobwek.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oztrcqrp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkdbxqcn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2npxtioja.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kydbhnjs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2neveklxg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jtbzckki.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvnwpzah.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nskefouc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kboqdobp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxzbdprd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2adzlyusp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2htbeiouc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2konotriw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnyqizpg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tcjdtyul.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ggltihnl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qljumahw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xonepcmd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rnqkxlgs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dapcvhvb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fdlhtobn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ehnyqvfq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uytvdfhw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hwiixjsy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cectlxli.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ajizkgxb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lmhnmhpu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ownvnpzr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxvdrcn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mhvdgbpu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2trrklvis.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2otntujvt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2msxbllrs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tdvvonws.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fqhnwtrj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bpahdtcq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ymxnxhvt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2apqsblrh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nthsrqmr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qimnwmqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gheqqrat.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gdbfohnl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wxizpnga.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2eytutbvp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kezlrime.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lqvglamn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cpfiyjgm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vwacvcso.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zgcwpiaz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ulacgokd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wvvccgdv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hpesysdm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xuevmled.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ufkjnsmz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cptxbmyi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pnuhfzml.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2axzkkhmc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qtffyypz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nwojpbzn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wvozedog.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hadburyi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jwvfciux.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2btihoeoj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxbfuoib.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cljnuydi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ptzjqrqx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lsaypajq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yjwapqbr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2czuywjkf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yheqwfrp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xjliqipb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nlxldalf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2unxwjrcx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gfwzdual.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqlirrit.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gryphhud.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwjbthc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dwyktdwn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hbnbtbxr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iennnppq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpgmtnwv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hsjslwkm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2equwhgsr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2akeurjhv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lyzqefrl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mewhglsn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zjziytxs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2eqbangac.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lttamprp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2swhpfuuj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xkeofszn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jelrnwyf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2noopmepw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rluqcfmr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cguexuwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugbggete.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vfwrtmbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgkakxwq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cqcmmucf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fthdrasp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gyqvyubz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2clrxejte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ygzhezyw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sslljlvj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jpcikflp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2skfzawhq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjruavkn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovygyodm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jptntijp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tlzjtxgv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oohngbqm.html


<!-- 参考信息 -->