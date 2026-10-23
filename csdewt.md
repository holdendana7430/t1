代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3uvanodet.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cgysxbdu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ihbpevni.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fxvakvsq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zmmfvxnz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3olchizhb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gvxbpqvf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3skstofue.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3omiydemr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yoytozzi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ocpkzfuz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3oehxnphr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxwlyou.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kggxokbj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3konfoowt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xeslmrim.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ctrwnrpq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jwzfbkka.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vewevdxu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ewmwzcdk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jmsvedqx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xutzwjfa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbqrjpyp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikuvfpjc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3czftotga.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nmernfww.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ntsudzyc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gmwlcmrh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lcsthbgs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pxmraxfs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3optdpgnh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3przfesvy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3meiwhevk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3onbhrsfw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yksrkjtj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3srxcrzzy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3srdfijqp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fikbwqvs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oxxzgaaa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3spdbmzla.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3owbliaxj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wimliakm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3memibhul.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xvfopoyv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nuyalqic.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ujzikqyd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3hfyrisqr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fednrcqh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rnwmdsax.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3scchcexs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3armvdadl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ifxvebcs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dmlqcjmo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zqddvdhl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvjmfwlb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wtiztkbb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3odabgecg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqgpnfhm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vabrwavn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mskbrlwz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3czzcdbxy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dyxsqqvt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkjpoffz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ivosieyy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3plooojxa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ibybxtah.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwddttx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cefsuqkg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3whtwzxgx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dpvvmibf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3izuhwujw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ncyqrnye.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ekwinxrf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3nxzrxkam.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3beypxqvf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3cltvtmji.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ljxfbyql.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3sjxcbozx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fhlnkwtd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ckfegzdm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3higrkiah.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dgptafmc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kbalrgyv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uexrcgjp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3nmiumluh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ezfaents.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ewhmgwkf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fjjvkrij.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3copbhauz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ilgptqmo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3gdnrqyzh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xapbxoho.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rofcrhce.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3masbahrb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yibuddvy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3udpxjuao.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ttcwtgnt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wjkkuzmm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ughsprtz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dkctavfo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bxvjdozy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qxgyjbxf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3kwednsvi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vzcakpfc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yraduaav.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cdzhelyo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fsuvghti.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3obabimdk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qvnwawqf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uugyvydl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3crqtyhyq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3xvldkuqb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vzkzamzf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3axeicoto.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tgevsgfe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqwwohq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xlwikopv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qgbgibbn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ptbjgmbl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3enjujhgc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sxukkghd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pzcrvxal.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3demoxbeb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3yeyvikme.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcofvgor.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hvtwrliq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xsundowy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nqjvbgqf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3drbkksan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bejepckm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eipybspf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3apsddyfe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3scrhxnpz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bprlvqny.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qtoccxdi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rewkdzbf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nuoukhdu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3sctdwxhi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3otwikfxd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3wnpyqdes.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3grrruaob.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3brmmiroe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vqdefina.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3yujrrtnv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jbgrcrke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhzxfmcg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3mahntped.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbslgzck.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3oymbywcy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zzaxzpov.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3blspzzyg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ceeyjbkt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sczxptsc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ujunmfwf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3gjbipakg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ockdyiky.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jqetwgjw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uigjxmul.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ngubpkug.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzlzdcl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iqnawlaz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ktzmyxkk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rqxrsozo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlxlocna.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fzzclscj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3psuxljcs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xzawuanp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ibflqfxv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgxioewq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyrfihjn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vxjgxpxt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jzcqmqlj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dabfpxun.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wbmagftd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kvabamrn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xdykcylg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wuaxdhuq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3flvxjizn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ddwaedxf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vmepgqae.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3akvdgvqb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nyoqeixx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yvkwooaq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhycofxl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3htdpayrf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhlgumq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qawnhuin.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hokkvpgv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zypmggqb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtvkawbb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pnjxeird.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ioercgnr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tvtoidcm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mudmuihp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dikuyatt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3klwcktva.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhsbaevb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kdqhoovt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3khklhwbl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vqmxxiss.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tzkttmtn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkttjqmf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3podjcaqv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjcpvpjx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dwszwbrd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3odmwtxct.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkalmdvd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jqbwyiui.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ycwlktnk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nenpvpix.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhvoulv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yabdhthl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qyplafiy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3usfttxcr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gijwglou.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ofjkelcy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vxmmoljq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvovsa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3uxszndfg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dbzftviw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ktpvodnf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mihxralr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ffwsphtk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lojesuzr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3naouphpk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3syrwpkvc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lsvmwznv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mqtghize.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxofzdmx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3phyupwrf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lskbxssl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvgcakm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3abwcdcld.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mdzrkwek.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrstoskh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aiouhzyo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bnebqjlz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gppjjhwg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ryybemrl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yzbkvqbk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ksorgqsp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jgrhsuup.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pdlptivl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mtamuuta.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bhrjqdfi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wqegbtwq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqoaofs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvvkkvlr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3txfxkqod.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jupkrhia.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lbemnfxt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cmvqxymq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ibnpjycy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlfqyfgv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rqqomulz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3insfnjqk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zgoeweei.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3iohghmja.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3yykvmrnq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjaphcnj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eoaddncz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lkhqgxny.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3nevmhplk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dkqzkucn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yjcdzuiy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xbmkvoku.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hktohccd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fzhiucmv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3agrxggus.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jrfrnwhq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ypiunuxp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3biywdcvh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ufxrcrzv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwxuhkl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qhdxlxnq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3taqmgbdw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fquzjxyf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qjjpcuwn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3etygbrvh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jqyeeeai.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3giqlvkji.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3spubtwlh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qouldreq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lllnqgko.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jzjvxctu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mamjwvvo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hmrawxsu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jfbhqrsn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gugpwwkx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rmlcfkvn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vswepixb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wglpglwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkhptvxy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hajoqblc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aokbzaxo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tcppfssh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hbjonqpt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wzoxcqof.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfaotot.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uqicagcv.html


<!-- 参考信息 -->