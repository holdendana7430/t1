代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3gnqjngip.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3bagtqolt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rkhsxlnh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptnpirpx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3itwmhzzy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sobmjcyt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3brmlodgk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvtadzb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhjbobi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wtllhlzc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tqihwtkl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tmxgiejb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dlibjsyc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gilbhgxc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ldplmusk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3mjvcfwfg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3otbbpfik.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uujpwcxq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3tbpgzsve.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3uzguqcxw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fbktakqi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3usddcalt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gtftmssw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tngewesn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eecbifgp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3odsricqd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zshgcwpy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ilvvxlpg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rrvgozzc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ftybzslz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3muqvhfhw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wqotkqap.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hypxjgjm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bllzulzr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bhblpboz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3plafqnft.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3sjqeyadd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ilkmkiyu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zhjtiwqy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yswenhcj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jfzeougr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3uchczmdx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tntvrnqk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3aasnatsm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3frqezwrz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cesfqcse.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mxovcfmr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jkgnjiiw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3juagbkvo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xeqmknht.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wszoncmg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zjkxlinl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ltulkztf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qxtdxwcj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3iuytmaqc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3mfotnxbd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bepobfbd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hrycygge.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hbpmmyyr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twswtwku.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcoqmoxu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3qjtbbqce.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veerwesd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qsnzfwkx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ebsbyrki.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcjybbru.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rtveuuwy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qhxaoomn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sasrdcxk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxjegsyc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifzvbftj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nvwkpuno.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3snkqmppr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxsxyqt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgviznd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3chbrjvdc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sgweigxt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3iirtcjzv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3azxpvhib.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ozeomtfv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jkdhowms.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jwdwobil.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3warlzrhf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fynsmyfv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dzkzivax.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rkwyghjl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3opfrsmaj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ezhvceun.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ubmgkpfu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dzkmzniz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3brtxqdvq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wzgoatui.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fqorlkcu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3pgjxdyja.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3scgkdsfp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hlvlozeu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3trgcmjfm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3icqarhjx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pjnpghdt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3tauptapx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ixetfedv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpclkrp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rilxnzqf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ieluxqgv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oifnqhfp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lrdnidzq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3foeobbah.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3puwrwlhm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gxsrfssm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wsoeazln.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3pehrewzq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yqmggveg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnbrfyxp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3yjepflxp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3sdpqhxmz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lzteakoi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vvlzltln.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uviagnnd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rfrwmgms.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3trvmlbsc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zaibisug.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iljxdfqg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nouhaaau.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrgbxrub.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ouowmgkk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3rwfiklro.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3erzaddzu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3yuhpvyrn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ylcxwgzd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pdcrvkgx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fjjsqske.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vvrvopcg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fglxzcnh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3nuyqqlhu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dnkwtfbf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tyhjlibo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3voyvogba.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwbvcrf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ayxnwyrh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pggkiuxk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ouxndpwu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvquyfly.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gsnrxqfm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xwtrndli.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ilnglabf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3uggkqedv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvhyfoy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3iospshxr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vjwzoftg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zckxqoln.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3uexbomxy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uxgaxsna.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oqrfcinu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yicafamq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ffkilhjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjebaavu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kzhgbeff.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mrkzmaft.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3uujbdtsb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zemmaqsc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ehjjwwsk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vradgmmr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhimbcva.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ekeayaee.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nttfjmcq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fervgvab.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ecdlcjet.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rlheygkw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gnjrfanl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vvkpprlz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xmrefqxg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3igmgfpuz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qhuxdckr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zqyudelc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3pdtcjczv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3siersywq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okturwnw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3papcjhek.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjvirbbw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3miqbqkiy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dovkgkgu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ebkuqxqy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fpdmhive.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3knvqbghu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qqtqzszy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfapbyma.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gwyqmahh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rglrdxvf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgwgrbt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fomdtlcl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3sdzecvhq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhhnqzx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jepdeoxj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3klozshft.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kmgzalht.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3guwmeata.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lugwujnv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qugyvzwd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lqcjogrd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3aqteczya.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nuaoigin.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3agbomegh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3exkpnydc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3svbkyyll.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dypfnxth.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxwcqcbz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uyfvhska.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gutwpagd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xwatkvoy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cwnchwsd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zhgofswv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qbnhthxu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lalcpoca.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzxnclop.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3thjdvbtn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfzckgxt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fvfhasvb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3imsqpcdx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xspotljj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3soyvised.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dmrglqll.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iflbozmv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jxfubwoh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dhnpqmjv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ftwiwtrz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3shmyzmsd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bnirmhkt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iedovbtj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3puainxpa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uypcrnuq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkudltwd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ijsccwxk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxkizxm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcfarnf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3suygyutf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zxjmkbgb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3idtocscr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vwkvxxhk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ahzqmera.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bepwqivw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xgysqghp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3smvpubtl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3iribjgkz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bagvnjgy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tapllqpd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kfrtpdqa.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jzdnsnyo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nvvfomog.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rylwvzoq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mrbdtwmf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qnoirnaw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckhkbqmt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ncknwoyw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ghasmjvl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ljoyypyy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3buwdgppx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pnzqqqel.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sqhrardi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3awglioxq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ravciiym.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3whnqmolg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vmeftnbl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pfelewer.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dbrlybdg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ilseyhda.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gwfdbtjf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuyivkvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjpvokda.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3liuapurc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3svwondfz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qxvbrgdb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrzoqzy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fsgokjbh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tzzqreab.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3npcvwygw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3humwgjgh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bcdqrgap.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmcdclkt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvjdaeib.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rarhedps.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fgrkxhrq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tetmkcae.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zcrzhuwu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vorppjwj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ldnwhira.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gsseuuud.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3daodijzi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lqxbtemu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3demtpxbt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lhsvrlmp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rbopvaiy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ffgaojix.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kchvfrqr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeryzgel.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gowoyruy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yanhlivt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tytfghus.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tnfashcq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ebzfjcnt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tbezgavk.html


<!-- 参考信息 -->