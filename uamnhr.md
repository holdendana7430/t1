代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mknphsmt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2abdhqgeu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lcamwmov.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ulakdfsq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nmagrnea.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2yzbnizer.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2mdfqorab.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qekpouit.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xpxwvbcu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2stzcipop.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dvdwrzbn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ptikicec.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2luvswrdj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2csuxynus.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nthbwshs.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ltbolwir.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ydoujhsf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2cnrhgfac.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2prlkjeun.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mdmdywxi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2izxxngjg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lxmmpspe.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2japltzjk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rglchrfo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2clwrsxuh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kpqlfsaq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bekxuerm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dtevrsxv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ngoctnmj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jdodeefc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2baldtdrx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jkyvfhmm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rlorhcbj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ebwmkmdi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2qmzejndn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zchmjlyi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ceuvayhz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cmavfdgp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgpciuyx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxbdmfju.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vcwhlbxt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xbcuieou.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2veiamcog.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pdqwtybt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpovytji.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ovqiliay.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oxyuwyui.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2njckoqiz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nzgmgcum.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jfndkwcs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fizfzpuu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2twkktjei.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2tijcmnfi.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cbgogqlp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bplbkbsh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hpqlizbd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2elahkwhs.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vkvexwnu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2fycvupof.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2aoiarcjj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rngjihzw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mcszjnje.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wnlxmfkg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rtpxwbxm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2knbrtmlw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pbgoxncv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fayytili.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rhfkpiwc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nwcmkmze.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2jxmdktpm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2aqafitsx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2hkjlkjac.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wysejkmc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vstnfuyh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2yspfwdfv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kzouqqrl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2krwngrfr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jnfwiyab.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wpywpvdt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2rmezrzlb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfcubgvv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gvonhowh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2siriwfqv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ooplnlhq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qogfrnal.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xezqbgft.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tevsxfnl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hqztwowi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vegqwdhl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ytjcnbla.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lhayuoxf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2arsxewcz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2phyojmbd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qomklxfs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvlwsnae.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2sygbhtfb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xwfgslmg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vwduyejr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iedmyswm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipozcggy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xizippcr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hfmbucbi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vxqebkhq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jynnvgbc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bsdgtylu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tahniuhe.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dspxogqz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2kahvycnk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyrvgivd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sgcbpoaf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ayshoqws.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hdjkosoa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2txlktiwt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cgcjykdr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mkdmfmgm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ennvakdd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jlfnwitw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zshvrsgv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vexpntfe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdzbfwdw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyurtvm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tiiqscoy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tluajimb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2otvyajte.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2adymrrlm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bwybdfbn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dhvmmuga.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2agwprdbt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2orzqfyxq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kpzmpyow.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwpimnuy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qngzrgzp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2svbleyne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oypclihm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qsmyhsrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojsmezpb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jgdlzokv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kowetvyr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szmcvylz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gkahtzub.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ojgqtwaw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oucevqvt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mpjmbrfc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2isjiolqo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tmvcgjvh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yfomooza.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2isiivqcu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2sbhoioid.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hqwpkskk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kledokju.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2edbwixdh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zzuikjpv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qmcqkkof.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2knvgqivf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zepwoywf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dngwyptj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wkmaolql.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdehnpw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yapbspsg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jnpwwyrh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2diryslll.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2slnchbiv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pgzihdsj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ayrjiypi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2thoctjyi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtmmrweh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jhdgtagi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tszwaqmk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qukxhihv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdslaiqa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cgehfyfa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oopyovvq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lzjqmiad.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2oocmldgb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2etehrqdm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2juvjidbo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nwaoydzp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jswqascn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tyhrlsqu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zofyumtx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgzftodj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yardhhfq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ycdciyyp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozxfubno.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2otlrmztm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sookebor.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2safousqz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rlzwhuvh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2syqfkylz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2htobdfyi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2eyqttova.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2osdxyzks.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kkfplvjr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jzihbpwa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbfwzpl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mamldety.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tbzgzhjz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qggtnwxu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlmwlqht.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2canuwbkj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vyrptyfr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yxxqdubp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kuoyqwix.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqpqubsd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kliqwory.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ubxycyoy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zzrrikch.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jqmohrzd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2lnurezbb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wzgadnxb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sijvcsgf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2itwnwmiu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcwixkgx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcagbjbh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2otdoxaqe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwmenzmm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxrybuvl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uogabeto.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mcflfukm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfpdxghn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qpojotzn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2esadkdge.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bngxlbtc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uysrbvua.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xedgygsm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2oownqjvu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wosnrrzp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ljzsrxuj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rfypdpbb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gvjmioyy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nprrhyiu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rgfkfmsf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pmtgxdix.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgeozy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2modzboan.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nboeglme.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aouyyscj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ncvagxln.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2herrpxgy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yykzdvnc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2skypgvsc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tpwixvif.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qmktikqj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2plxrjfic.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hfrbzrqu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xlvrbpqj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mppcqgeg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tezksayq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hnwevneb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wqxboidz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2uvvfzlpz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vstteszt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mosuantr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rtylxemr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wmqfszid.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2scpdiirx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ptbulfiv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhkvxfv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rnazaphn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxwspma.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyderla.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdnaqsb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cqsvrgms.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mltfzvmw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2iibugaee.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kcwearvb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sdvcegjf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cftcmhrd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdhqsnbs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2shmklpgs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jgpcasug.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jxohgriw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jwlydpml.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ebceetxh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ryzplbei.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dgzczjcy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2werwzgzl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qtyssgnn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ugrsdsfp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xumndvkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xadwpmbv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2asnyzyhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cepdjulc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kjnqluhx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qbxutlsk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oloullfk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlfmypmx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2roywsohr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwyzcapb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pnbfsthn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivyvdgee.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kkpdwxhd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2egrlwmvl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bzjxzzso.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syvmmkmd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eexciubd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tmeqsoaz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ttrnhmhw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2orpiplpp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kytpuxxs.html


<!-- 参考信息 -->