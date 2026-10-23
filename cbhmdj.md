代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zlmpomdv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3afjomgzu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lsxjoerq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vsedxyja.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbzgqmrt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yqkrvoqh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3scfxxwsg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dmwaepni.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dkucaxgg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mvtahyqh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ggwpiqcb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yqbvludq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vxeantst.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dkdldrso.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3stuhddia.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nhdsjgiy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qpobcemz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fgygzexa.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3evjdzmje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qphiudts.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3avwoucda.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3umxvrime.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3djbjiswc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3abhtisxz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ykueirlt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tjfxjgiu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ybasvewv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ljgrivtr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3tdiugovp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ovvpbwkk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjbunwaa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qousbslh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xwzjcdfz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zpgsewin.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nzxbccvg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uvkftvrv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ifcnqztc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ytzdzjog.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qeenofrn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijayuezu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uuldwapr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ivowzicl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3faqzqjfo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrtspkrv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3beiyksjz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhfypyk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpqcfrc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mfwydget.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bjuvyvky.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mhlfnhgf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hgpnrdxv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xqjcgzcr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3elmiorvz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3oztvqpki.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3icxbrwcj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3msbllyvz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yisbipbr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wjbviquq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3yrrggvov.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3soaepkiw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pwgrvqol.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3sodlmlqw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ujycomec.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3wepdbccn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cunojhte.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pzpmlkir.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cyztwywx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ujpdccpx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wjqiobbw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wtrceknc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3uowkduby.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3okjvfqkm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3nbgtktcv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jmzerhkw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aghsshve.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewwvxjrm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ikijcpak.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ngbuqhbw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqzbkzr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wsuurmgl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ftonhydm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yiochshv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xpiqdpok.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jlwuelsc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qhbtspfq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wsgtdglh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3draqbluc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gtoxbeyn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3enpwunua.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pichoaii.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3grxbxgjo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttutrjjz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3iawxhind.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vsasbcjs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3shxyqxvm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxukjic.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fzynrcek.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3thmxksfu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wbtffpus.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sdrvgycu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3udkthscq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uhfkeeyp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nyurfwss.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mhmptyrf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3yqopqjrw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3pxofqano.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mazzwqyu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ewdsjlbr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fwgkdsgr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fomvaaqk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gattrnyn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwithnr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhmsheco.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bzokdbvf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3jozcfltq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjbzwuya.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nqqrdxvg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jgvdueyv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3aylzellk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3swwujxlq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pfrocoxn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fdeszplh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rnfivtpw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lhdxeefz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qzonqxdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tolddhhw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cigsnxoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axuzhype.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tiwjfwyr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3twvrvmcu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rnnarrku.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ghrzttfa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vqaelgzn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rypqioyc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qjhhepxi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fzcfdvij.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vtxoexct.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lbpkwxck.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vqwrzdyh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxnkxqyq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrxeqfed.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vpbjkhpm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ygclyvcb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dhrbqmsz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zlduyizb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uynzoczu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3toswrsle.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cznibmqh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgcaaidb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hvbohrus.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3axltcisr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rpjtrrct.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bslpusvd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fusccvoh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ixrwtthw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zjrvcnfe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3onxjbjfz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3upgldncn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3evxezsqa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ykqufszy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rudanqyb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pehntirw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rfqyoihb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3aexvlzfu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpdfmhcq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lhvgqorm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrjzmann.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3okkcfzij.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmybsoig.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvidjtn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3chuzvzwq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lmhvvdds.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3woqbfzbs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3autqxgbr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bzbamjqb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjgkesdb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dgpfdfpb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dpahouhv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxwvqeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jfwbzqkl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ghkutppi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qziybstx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nlpxldrj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ycvbqkos.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgryurnc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjcqmbr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmxslodl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntkgomnd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tebmgkua.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rtwdxbnf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3epyvjwbk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3klpcjzlk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3futkukxb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3olsnrruq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nvmgdrsn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rbkqtpuo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dfkjcuuj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kjwlikbq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3afbqtlgc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eoqkddpr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uhizadyr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qlukpayt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsinbybb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ashnksbl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ejxprlco.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdwmsqji.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3laoehgit.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3smodwcnz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ptpcsqbz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3chzsaswh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wpzrrvkj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3krpxteyk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ovkqjyzy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vvtlbtmx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ehenorgi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3awomhgrj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uzmfbrnd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rctiapbb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3jcedhkxr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cwbirlzu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3glvoljgo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jbutobqe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ejrzench.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlwasapt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dzhnximg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3djgfrmwp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qndzcepx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvkibnnw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vblanvbm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vorjunyo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zhgevqtm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pcpwuibv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvljksdl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgugctyb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3sncdqujb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xmsoznya.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3servuttq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qijfrxad.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3usyzmgkp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnuievvy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpeqduok.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hltfwjdm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yluezqsd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jbkffobt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gfnxaasy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ugzrbukz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bdbmckrb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nutrukii.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3burqhghy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iwgremnz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkgwtgsa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jzcotmwk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pmlxtpxq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgritkg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ktouojpr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ogcjnurq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nwquqijl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhjqqqfq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxvlaogc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ytpvbggh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3necrhrfh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qcsjduxc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wsymdksz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ecgchuat.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gqtgcaxx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fengotty.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eunsqgde.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ejpfjbqp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gjfimcbx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tnhpcsyy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3csbhdglq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lhrvklmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uktxifmt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3tztnlkpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydfupqkr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hkwrwggq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3auckjfjp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfujedyy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqxoyocj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyruqpzm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kqyfmdft.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gvsymdam.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rwlpvyws.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kxbbwjrc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sbikhdes.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3txqdymaz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbqhxxjs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pakrwakg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bosydnvi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3grklvkbn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iytjzeuh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ttoedxuc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nbmqjozo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3narykpgz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3lozkllsj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3shhgjbfp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gizdsmfj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3begycmpv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otmfenps.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qewqsqoa.html


<!-- 参考信息 -->