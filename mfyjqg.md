代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mxhypblx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yxglpewf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sjepqvaj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2acajcqon.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yoftccht.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bqgjwhao.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iaknfica.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gmzlulsr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2oecqmklc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fonwlyvc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tvfcmezj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uodyxjjh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2izfmgzjb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zrzfqwhj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qpzrnomh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2iupdaidj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vvyjqvzd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lskdyepf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2daemzxfr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cgfoigtp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pyoazjhe.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qkquocaz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mjqrosom.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mzmhffmr.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eqojvpru.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2npxxqifl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ewctxark.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ulnsrsxg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vqviplli.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xitjatln.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ergiqijm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkzytbtm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2lbisowwa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2voraflmv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivnrbyqr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2zdiyljtk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nhhgeokl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2woombslw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2owkpapqq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tepoaafc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2azluvuxw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mchygxnj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2csubsznk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2faxbzvwv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dbngyeyz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zyvqocee.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2epzhtknv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ayyrouos.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cbspeulg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2skymupqt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ckghmkpu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2urhwuata.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wgcneozd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ntlwybkm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ldalydcc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bsjgcyri.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aychwivq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ynihyknc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2skbzeolg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oxqfdlmf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wkldtlvv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hmxaeoen.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2lfrwrqfz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ecnqdube.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uviahrjd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2gtlxuhgt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ggkaazin.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2sbxsporp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vowxsfix.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2crpngsck.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2nnsaeqqj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2yzuhbjni.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2merygesf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2meoxxyph.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2klpwnovn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfxxsgy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ylyvhebo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nxsyacui.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vbkjcwta.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2oumfnkok.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgzmoivx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltgtwjjo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2oozobsgq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bwmsaznv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qlyoduvi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lyxhbjjr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hxeeoxur.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ujahqsft.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xdaniscs.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uyzamkkn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xhwwrciu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rqdsbiwh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yucllvkp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rocldjmu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ekdnlauv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2qppdmzxo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zgaorwku.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rldibsjy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2bltncxar.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xghqpvlh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bjyvqpmx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mbgzmzfu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vtxehawo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zoyzvpiu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ddimzoey.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2iihceaok.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fgcrddpx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ybuutyrr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ebhcaidx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eldlyqtz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdidcmex.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqeqnbz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ybenxrqi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkjgkkt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2oonoglff.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jujsylwf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2teeqxyiq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qofqkihv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tqolepue.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zqchopjl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wngzijbu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrhitut.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2mxgcehbp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2byppgoqx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pjxdxzpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hailruhr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dbfgmddc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gomtzrhj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qlwsotgy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kplfxtuc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lumrqzxe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qvqireef.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xfgtqsbm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oimzevtg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xnqefayc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nymgcpej.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bieycxwo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ezmffxvc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kqcvozpk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fqmgjeql.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ytsusryl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2defijzyv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2puuconkk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jtmkkkpm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qqadgofu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oqkozrbq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2utwlwcly.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ohmqwoug.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ybwvxzfz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qroloigt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukrcuzzt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zglovyhw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ekzjhgly.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zzunrmcg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wwkbvnqi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ttkkfpyv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnjoqcb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2davcfign.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjlwuvi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2odfhrprl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2upodozji.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ghokewuf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2trmzmpxq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2aredxmnf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uqdcpjro.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbibdnd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zosbvaip.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jqoyrnym.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2saqqcouj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bbdruxip.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ssjuvaaa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gkstkrtt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2amuvnjds.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ghcsdmgz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xfonqxtf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnpsqtur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ybvwvreg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zxrxcerl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2moaghzie.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gldubrjk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bijqcwyj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qxrodcit.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynscococ.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgxpfh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvoiyye.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtgqxve.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kwkmdaua.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzcokfkb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ityrifkv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sugkchxa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wqcnknha.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2usfgqueq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qlseohrl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eqklodza.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2atuvbbnu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jajfgrzi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ebnsaohl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cxepnner.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2taxupvzf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2snydvedd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2eqesmyiq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekethgrw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhjfjunh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwquqtm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2omhrqafa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pavjtfso.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqejpcn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2srecsaht.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioifnwqv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rvlehulv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dylknihz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hviswmjs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ypblyffa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mfiojssj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tynvixlr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pjkwajhe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cbnsnsin.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dymnjxpo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2huwrauli.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2chvclwdb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rcyvwjrn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zrnbtjnt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zkdvlaas.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2csxtssaj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rqrsbyfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ichmkxkk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mcicnttq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wtqdsjtb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uofzygly.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2tmskhfqn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hjnacgko.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2skydgiiz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ulbnjkwv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hlffjftr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xkshhytr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2meirjdth.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2kwrxpvln.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qhyjnfnd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gchedwql.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inausvwt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jonsepwd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vspgxvqp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vpbubuye.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2kfsknsky.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hrpdxdst.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lkyimrtc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kwgvonyc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvnoymy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2diqlgkml.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rveonjbj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rbdxgtcf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hylefezn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbjtdxe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvckyass.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2udjgzdng.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2sowejqli.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2moaeetwr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cisvobui.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iuaaacsx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2phcpuaul.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2irfaaesx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mqumdenq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vkjwutbl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fgcoqqnj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2upgrdhbf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2uqhnjmdv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2htlxnvii.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fesgcnep.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fuhfendc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2sbjhmqnr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gbosemmq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lnacgjbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqfrpdyy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2arigknwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyravkik.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxlifxot.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2llegdvin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdspfrpi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsdrixdi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2spqclkwu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hneoopuq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wyeigmdc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qoilyoes.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzlfzdrh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dohwtius.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wfbxbpjo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rfsfefue.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djwksgih.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2priwxlkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zhaqfqlg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbdkwqle.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tvbqnccu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dezfelyb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nzgxfeqy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jvqotqbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2spknkuyg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2knwkmqup.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nidcylhm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjvyxasz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qmwhtuyb.html


<!-- 参考信息 -->