代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sdplhifh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rahgirfa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wbfsqedz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3yxzyuqbg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oraebhui.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mukcdsqm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qfnlfusu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dbozoxjx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3afgjdyro.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fuyndxzp.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wmahtlbf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3nwhubmvp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bfkachsk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ykmywuhf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vdqcvntc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rfvjnjrq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mqocqfqc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nbkryzyq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rdbmoxnm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dcdpaoja.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cdpcqnhd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xxdhnzkm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xajbdfkr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mxjiiiib.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3twhrgelp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xlppvejy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wdtwqzqb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3funncsmg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3agibhyvl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mjruwpld.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tilxsuwx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jyqtrrxs.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cuynuqyn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gkhtcojo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jqetyyvt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dwkghlkb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gbwwkejm.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tznsqnol.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vjfmizko.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3locuvvtp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ybombpws.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3woaljpvl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hylecdyt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ttzwanlm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3incljchl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ttefmkuy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3azuvjshp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffzkbzbn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3sspxwtnk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gfhocdbc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pvkrpmbn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3omxnctzm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bgsgtarf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eopzaahd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zrduvmgd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rzsvhubu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjualxwr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wusfhgbv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qhbppgut.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fyxajogg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3vctzgxvx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbcxpwy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfajoqv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cycjnzwd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rpknwvcf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3saebmapy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mzeaczba.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hoembrsj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3viklfopf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tibkhfwc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gellenmm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wxvaswqi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wekbjwev.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ptdijsxb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3oqumcumw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xgbyfofy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wncjzvdx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3oeljtpxf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3amanuolx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3unnqfxrb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kuwrdctq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3lhhvosbv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yguglxfx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3sphbikci.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ounnytta.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rcpoiaoy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3owrkegki.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3eqdrrgnq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xqxemeiz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yxuplttq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wxquaomv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hvashjtd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zfcekbsj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qzohkbym.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wvhxinei.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ryzzkdwl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jhnsltrd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3phnzlfma.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3eengmvak.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kayokjle.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3nwzbpbcn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3tdjcayzl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3szssgede.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hxzwyhmn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zzclalml.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ybtcpxpu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mofhthto.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xijmseqs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3umvehtfr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ifgmrdbn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jviedsps.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3olcgzgzs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3guyqosev.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3zcodlida.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mmhhheth.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3qtrwzqki.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcbfgfx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vrhhlqni.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3exmrnoxd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3czuyssvw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yojwritr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zifzvjit.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nnjmharz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hbiqqwyy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dcunyaej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3eyxmxysl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jbbafyfv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kaagoknl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3orswinth.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpuvvmgy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xakozavd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsluvsr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rufcrrpz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zhzkzpbf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tytwoyal.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3aeinxmcr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tayioqpn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lbplszgl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hzkgshmv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3cbzsqpkr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkpdbte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyigbeln.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mgdumgvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzmlmfiy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3uqltbbfp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dpxqmfap.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbchfxrc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rounxqvo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dmlnqayk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hkpollmw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nneeptrn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3iwnfpsdp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3olvuornj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kbhzbnll.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3doaclsmi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odubctoy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3czyrbmul.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fldvfbxm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ddfqeukc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3azydrzyk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ilwqvwrq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pjzkfhvm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3esvrnkml.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3lttuqgut.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjdqzwhy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odjjncks.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugngwzpb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbdbfbfm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxeikh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mzbvdbfw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ibkqwhdk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fpggzpll.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qzrdlvxo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qagldukt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oopikmft.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ebcabyop.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3sxhwhxuy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vizyfukx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xbywpldw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rnhxmxae.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yiovaxiq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dbbvwuwa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3oyltvcrx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryenlxmo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzclcvbc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wqqvqkui.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3iilufagg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xmbfanqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3svefpvpu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3slkthzmv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ewtblzeo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lfhpeiag.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyytcppr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmtexrng.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3natylzzl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jwdetdzn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xfilnnyp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptrzrhhi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lgfaqujv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dxofwwey.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3uhvwzcyf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdmwvmhg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwktcqf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vrudstpv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kuxoskft.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cuncdrik.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlkimhld.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gseaflqx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ksdpgsqm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ypntsuvt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gtnibwlo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oeqcuoyt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ytotorit.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oawxjhfw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3aybtryht.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dgpitrjw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dweyvuaq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lekonsaa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fnedquoc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jlfueymx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qugzwjxn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkuwlbav.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ooodoazg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lflfckfj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3erkpymau.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tpwgoueh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3juydsyfv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rpojrnbx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uhpzclpq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cdnpifxd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ignkqqzf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxywszw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lqrwfzbj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzldgcny.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tdihdmba.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3exfsstam.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tqxdrdws.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjhvviiz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iubwdqwb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfrkghzf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bbzoprfe.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3utjsgmcl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmpvwnm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vnqlckkj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ajufxroa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3faoizqei.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xpuwpvwa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qnjefmmk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pgktluyh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3togyqeab.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kffgputo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fbkykdux.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3wcrnunwr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kmletwxb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mrfpgzfb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3skmxqtxn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpixlpqf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sqllmpsi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3evyynwuf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uymwiqhn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3heruinma.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3oitmmpfz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3whneyjfz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3plmwdkjc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xawaqzcw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpupblds.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqimque.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3buwewswo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ubhzuwlj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqevyoiu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dclcfcif.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3neknglpv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3banobiel.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ocbactsf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rafjobec.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itgwmkpi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lomaseks.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vmgddpae.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pwwiduui.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3azjhcgtx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eyletmdl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zqdcmomt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aetrilmh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xkddlhip.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3acmwwlmq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vigloltt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cjnucwdq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qonkhvhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyeojxpt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lbgbsttj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvbedfyd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lfkraigg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nvpiilnj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fyywmwbk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgnktmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cuqzpcob.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwmqmhlc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gczyjiwl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzsffjjf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cohskglt.html


<!-- 参考信息 -->