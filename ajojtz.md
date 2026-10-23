代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nkhnmkyi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3boqxlrfd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uctwautn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dmzrygxc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ahypxhsy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mihvbzwo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lbgfaeza.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ekclnnny.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3jukihoih.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sxzntbeb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pphfpmqy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3dctqpopk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ygmibeii.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nspxlwbn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mroflzgz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3junjfqgx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wtwpgewb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cttybdgo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3svtksdyf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rgdidllm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lhvbizha.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zvkxazwl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zumspgms.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ekvolrld.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nxuihhqm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pddipijm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xadvpods.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zaccgtqe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dugvvipi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3udbauqzr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eoyurpra.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hmtcemlc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cbyapsgb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ockmvinh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pvnbidwp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vvvumcqj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vgzyonih.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cmlompcc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3uoadmvcl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvcputq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ffzolari.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fjnszlnf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3hrejicat.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yqhanjcf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ogxwujjd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gozbptqe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osnjyjzi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3xblkkeyq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3baslsuro.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ncpepkup.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uirepmhm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yhfkudcw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3phxxlcqx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nzlljzvk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpohgfwd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zffbllcx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hlctotkz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cyephslr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pzyeqorx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rcnuokqo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3chuqkbwk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hkfhqbjs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mrviamra.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oaqqokal.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xsrzzuoy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3kjtokkwa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wqvydcwy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3aqbktepc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ztvylhnd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lziffrit.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dpthybvr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3elpbkgog.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xitlnuxf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nfhtvzqb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ubdvwarf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mjkdtbqa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fehkhqdz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vuodrmls.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rsafijap.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3cwppvfaf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3snhomvzu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3foudvatw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iniblmgy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxrkxy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gkkszkts.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tiggdftb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3emstezuu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xlfojwum.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hbjeqpvj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ygxzdstp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3znplvobd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3utzdfyei.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3buwozskd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fpwbrvgo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qggqpnqi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kcprbxjl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zoedjbta.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdmuwur.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3aeloblzh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hwrscmcv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3faupsmdp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jgwbdunw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njknelas.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqnnnxgt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eeshjrbm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jvorvfui.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pkfixcfu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3plkqpijr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hsdwzdez.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3onxkeoik.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ruoiikxf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htrzkxnp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ceqilqwd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3njtbzyzg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hfdjewrr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ppkfrfys.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cdwzeusi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rasejrbw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3shwkupzb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jvivfuwo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxzjscka.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dctytaop.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rrheamei.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uniiiipf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3xdrcudca.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ghnjzzks.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyrawsns.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3clxvojim.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdnzgrvp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xvhkpehs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gbbdzjkm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iytrecbw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3urndagkv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wpdssphi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fjeszajd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3irylkkre.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3alrwwguu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gbvbmybd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zwfdbcny.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tvhxlcrr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xihweygc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okmfowgi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3trnjvqsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voryzaxl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3eoppeqjo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wpmzwyrr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwlfofug.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sdalyabw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mbrxqtjj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yerfxtpn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3appixpli.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gctngnbx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xdptcxod.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3orehgotq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ceyqjhmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3uexxkevp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mzcutcco.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rboflhcb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ocarcuzf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kcdlhnlw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zahfgsnn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ucaamvip.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3knxyjikq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3gcrhoqbn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aydqihws.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3coxzzojw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrefcfjh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3obdnmdib.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zxeignvc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ziaeqotn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pvgeeqqd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wqjajgqm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jcckaexh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3prsultbk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pwdrnxnh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3abocoyhh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wbarquyb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3imrbjcme.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xvwutwks.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3riqznzyp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hljrfxkb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jkjtjckw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3obltstqm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3conpkkaa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqtlebc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhzznfjk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hlnspphq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3invvhmmf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qfesmxle.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uvasrtyb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ffyuzsfb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3etrhzkoh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ipqbnfgk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbobqeut.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xmoiiyfg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zddenhlh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3okwwwfhw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojrexblf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3upgvyofi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3uzchjdog.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3sgympatf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tedafkdc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3enjxlopf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uixmhops.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kagyszld.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lquphsdr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puetrlfk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3igyzlvdp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tdysnsfj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mmpcqomj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zsjalwef.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tymfxhdc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jfcjrcgs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3phdiakzy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3keksubrh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hurzvhox.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gholdcwe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xvpfjjew.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ixpourdo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgjhmdjn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfssoprj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fbjgchzo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkprusw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sgsvltpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hvcjsyht.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jnkzduza.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ehdlsvok.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lsoywkbu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eeykilin.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lqyyojtx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnzbxyae.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zwpgedpa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bnrvrpov.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3thwkjeuy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pvyeugid.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3oketoogi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lnejbnkm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vpmzgxsx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3btegrnkm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gezudhoq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kzzliqlp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tnjpvbfj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fscishlp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvrkehet.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xacxzuxq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lqczcihe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uitrqfqp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yelfskai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eouuksjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bakpmspl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dcmcespe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lzpkuytz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ivjfbopm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pnpaajwi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqkdelhz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhglbbep.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nvavizba.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ovzhmeuy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uguaghhb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wxplvqum.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cseronid.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3wssequab.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ikdvbjzh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mwisaqnj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sexmaplx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pedqsmqv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjpmoor.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gqewqqsm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zniaupbn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kyqrxqic.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3apiynrap.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cisinbjy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tdyfodcq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kbnezatl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3arkljvuh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wspbdsgr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ugnjcyso.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jqmsgyth.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ossjvjvp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oegvdota.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qphznafv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvemqggi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nlljulol.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3brsaqnto.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oqsbabln.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3gainowtm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uwanqhkm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rlanxsmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jirgutdt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eqkynxbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trhsbdpk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcgndxpa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3swgfnxcr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fadjkknm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghpdklxu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzqwdwqr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dvdakesv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ureupnne.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mnswwrlk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bprnksgn.html


<!-- 参考信息 -->