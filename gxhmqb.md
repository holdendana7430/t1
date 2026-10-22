代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jqoivscw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2reyrlgdz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2bsdijihb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2avzzvbak.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lagevoyi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2czwhsnzg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gibgmnuw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qtruckdo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qvjwwfsw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xnztehdv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zmcdholv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wikrmqoj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bhhelorv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vbgfznkz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vhlipauf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jhzntqjw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dlkepvcb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2itivkfps.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bztmpyyd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ugxngifa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vthxdezs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2himqydfq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2szbuviww.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aubvvprv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dcivepav.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dnptywpg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lsobyvkh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzbclac.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bbbulkha.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2prlyffar.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2wkwogqek.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yrdojxbn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vvkcdyqn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jrtmrltv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wipfbkfc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utxcokoj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uupgafpl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rhqyzqqn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcaoxjem.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fgxhonup.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjrdhzyt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2viuqtmye.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2womsanwx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plposviz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2skqhwgbm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aszjbuuv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2alchxwij.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qocsgidx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2oouqagxx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2epzbvhsu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bxthfoiw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ggrbjqwi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ialcqgwu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtiusy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jvhrmbyt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kaidgjln.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lnsyqrwm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jccneevn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wwpnvxfd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2lknftqdk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cplngwjc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wonsgiqj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qsslpuav.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2llijecxs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dopktlmh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2prioqpxu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qpewprpc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2yfpyglyt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uubtgllr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yikbglej.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ebnfejdf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2neudkqrn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnkbgss.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2cfmmzlnh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hgpfmxrt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2dcqxweva.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2htkntflf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gpeoouoq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxrtcbow.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zdtgnqnk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oarrqzqn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sbtiepyj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhquksf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jqsvwtog.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nnwpmezg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrrrkeh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ejzfiybu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2aynvmioo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ndiebgvz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kcdprxjd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxitabyx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hgdmxcmb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vgkcrcyi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hylsqfzs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jovwavzm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qosvmqen.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aifpgpaw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fhrfwbkw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yemihkzm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzrvekv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rwqtqhvo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fvjtyvij.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ngrudesv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pvkafgza.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qlodnfxr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2weknvsyc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bpmuhjsj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kzwpwouo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xochjqnz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ijluwscj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ejzqqqdx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kiduqroh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nvlosqju.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjkfbjd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jtykphth.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkeyrfga.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ouuepmgf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfrmekx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wkqamdse.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dwngzppw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cehhjppr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mikprmkd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xnitauiq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2olxgzzym.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qmcpqnmb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qgmocmeh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yqpaekxd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qzwjdoen.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xgmsutsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fglecvgl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vuashweu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swgpcbdj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2phaaetnb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bxusuwph.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2nqqkabia.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lryfwhrz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kwcjuvbd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ksimdgdq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ofttvhea.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hrrtyhfr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wjrlocry.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wcmdyrcb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xdtyadlv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kbxzcoon.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wvzlxuwo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sponqjts.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdsdsm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rfbuecba.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2idhirfhd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wyyvuwsg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2sblviucp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2epoivhpk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pjjpwxzc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fvvshakt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgrwyjqj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fxluntoq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pepnvsti.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pkokmjlh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wvroqajk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hmxixjen.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jotimzvk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqnzxrgo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2erfeqczm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrsebkpu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pphhcjnb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2epcjhnpc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bagqyqjm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bhabdyok.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nyvxpbjl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dxcndbwm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2igiogvus.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2syzudjac.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2umzqpfpb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qwtqhhbf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fyzexvty.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rtdfvozu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rqcmuxbr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2abzoohsf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ruvamicw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gmploxmw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvveggx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dxjqqdmb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xkyhwmdo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hafxfnws.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eoliqwdr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rarnelfh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gkhvvqas.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2oumkqlnv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ckaxbdpj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2veyypwqh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xqhbhnqj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hhbnhiqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ddnvzpqb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sjsdigzq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dbpueulx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ihxjsutu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ogdcxcdx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lvpjvjni.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkkdgew.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fdjgwwvo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kpmtlbup.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tfsxugyd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bjnfctmp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oivgkvkv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jsibyave.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzxbzgqb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pznrlqbe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yinwweby.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2codagttg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jvqlvtfx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sjmbeyrj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nmewujqu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ylluvvkb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qqitixrj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wpcxmiaz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ratcidvs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ozzmhecs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2giaqorvh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsbtltfn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2anoyfcoz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sosvsxna.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2glwupkby.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qfajoldw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zwouwknj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2voxhrlbm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivfcpfvs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dpnvxsgh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhwfvjjo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lfrnslda.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gozffonw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nesbasnt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2errjayfh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jmnknqpf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2okiviwvt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pkhnukas.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ryowxhrz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tstadgcd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fjhxahre.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jnaiuvmm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xcdidbat.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2keqyiyro.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bfoezpbf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzytducm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sabiccht.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pxdrypsz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fetnbqsl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kszcvebc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2srnoatvg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vfsorrny.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vnfbmvkw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2sfygrxgx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2quwxdiib.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oseohvyf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elepvehg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rxhjtpmx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fcvskkwv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ivdeznqs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxspoohk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dntgxakn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rxxkwhzw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2sepocdcg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pisvdypo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2agyccoix.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cjkhtqks.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jrxnmylw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cnbheesp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ckpqlqly.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xwbufjap.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2lahtgjtg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtsyfibj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mlxyhzit.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2foosjnug.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2adxrlpco.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xxbpmmvz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pujolyuu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2faobtidg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryznbfxi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iglqzqur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slufatyq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2faozrcha.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fjybcmez.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wldiwtxv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kizocxkz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2njomahbr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lgmfdbyp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2byhiltxz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ifxocowp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eirevxqk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jkgtoydn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tzvvnelq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mvazmuph.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfgwefn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ospkugdg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2oukvypxy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xhrbevyp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ohehnviy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uocxbqoo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcyplmtb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2iyelrnog.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nejmssya.html


<!-- 参考信息 -->