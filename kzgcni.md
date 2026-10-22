代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zuszsrng.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dhnlneyu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yhqolkkp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bmrzihmh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ciwiuztm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dqnsihgp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sjxtxjcv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zgpmnrnh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ssyttinc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dixalkgn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yckchpnk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2btpomynd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nltnhcsf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2irilwlnl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2scfttfqc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2flgbhflw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rogvmmkj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zncgzvyg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rqkemryg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mmrxvjsg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qvsegnzf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xyflwadi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2cccrezef.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hvdhjwzs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ankuucye.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bybhzzyg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2htqiydmt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2offgppxe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2sbknbzba.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fqldnwve.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zjtheisf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ieoumkkn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2shehzaqo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2izcmfyng.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qkgfzkpv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bqtfjntc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmsfeqzi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sleeppxj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jzyoymji.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zqaktjtz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sgjhpjwa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vnzqqbfc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ebtegqqp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uuxrddkw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2gwsoqsns.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jnjaomzb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrnbjzs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2omptwcjw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iamzdcwp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ywvghdaa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dzzrwkye.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2wlphcsvs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ifaovwqp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qxqdmfov.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gdzlaeug.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2htnbfeux.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2suzqzajy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2khvkqocx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2eormxzph.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dwuissmn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cnaypxbb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2avtqjcjn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fuephcxl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2zhrfilnr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pegvxgqq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2nhvccima.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sljqbovg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jzvhpqrw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tgskfqur.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ocucirva.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2seahkrzc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2npnllfby.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggqmmono.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2drfzarni.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfhhwzj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pvzizafu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pjsavynx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nheszgdi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsopzkf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlzkiy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cnhxexss.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gijnsupz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vicqmsfv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vljihtlq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ablsnwjy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2osxyeumi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvghnmaz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2qspbtpgq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vnabydvh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lxjjrgmm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yibinfbj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cqpdeuxo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gjhdvnmk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eaucnjnq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2udupfkfl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnapyzd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pjqfywhz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2dyfpcnjg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ugxcawiw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2wzynuhys.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2inufmxdi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ggkwytra.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fvpkfltc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2dgqlbnie.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qikayobl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ljhvwabd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zrkgkpeq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2idohrdai.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zcynlcxu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2emiklvgc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2skrfmjpj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2euzxpqkz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2sgmlvwmn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tjhdbsjp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xxsznygv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjdqwgf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2kpwjvwda.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pqsifpjq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jyxdemkr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wfphdyzd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ekmfcvmh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nvyrrwsd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2awcsimvd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vksjvemn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xwnpjkey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxalotdj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zyfzlnct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebzvmjsq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pdkqypsb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wonesedr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfbbaeo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xvhbukbj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hggcppqy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2islmgpeh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cpbghqpk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hwlokiix.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eldpozuq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jeridkqg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qyvgoipb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evzacgdt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iujvhxob.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cxhtgltf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yjignhhq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hamrtfga.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mzrfpbas.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cxoidkos.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ogxkkqet.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xnszhzxu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuosvbky.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2excptvwz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2enawwmpg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkelugvj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qduyomuh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xwfyxnst.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rzvzvdyb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qdrqtiio.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2odapmdgh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zzlxfrnn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ieyxysmj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vernkpvu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cbvapzkz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2djklmtbw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bswwroam.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rzwjrsnp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dyolvuha.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ulmazzzw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qxttypla.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnndmoyl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgefeeec.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tnoaqowk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2eiqczyhv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xasxwzjf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjccvio.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fwpfedph.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gxrjatpn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2syirznua.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyrdvydp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2krcshxim.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2igliehhq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2odtnkjai.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xjykiyzk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sgcngmvc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rilzbrmr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2roaynaad.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jviajdam.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2crfodzjv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fwnipwgt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffkhmecj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lochhhej.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ovgclegi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cnfjngqv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nhmplosr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2toebshiy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eesabogn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gghcawqh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ywkzxlop.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nxcejrbv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvaebyk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kpucjtkf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ynbbbwoy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hvsazznc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ztrzkvyl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ycwkyfbu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kutjqwkk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vogvyvyz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdsajenz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2evzuflwj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lastamas.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjifxpth.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2isplclzt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dqlmaowh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pezzvcog.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2crpfogcm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ecipvpeh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yalogtto.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rxfwhqal.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cklcyssl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcpmgdue.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2boxxhpnp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vwxijdwd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pazoxofn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rhwhduwv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mcnijkee.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mpdmlaoj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2aoogigle.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2frtenkdy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yhevintn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uxuhsmef.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wqaovciq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yznuamtm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iesulchr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqftdehp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmvmrwf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mwstbffs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fqpqkqmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fhhppthl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dtwedzwd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bojgjzad.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zthkdflj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fuliiyzu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jjxioyfy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fyjrdmtr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cdxndzup.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2guxbfhiy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qrajeqsp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jyeffofm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wwjanuom.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2znqysuuu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfnktvz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fxiycqwu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2louhxkxz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kutamism.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgolstx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubsljlkk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2efpqaoor.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rxwhfrla.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nhftbpba.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ouqpmriu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pnaymqqi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bdvnvtqk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2egwyrevg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hfjzxwmm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oeuflzns.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yxlswelk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zvzzipup.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2umznjwua.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqfzilvv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dzwhlwby.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2exykfyyb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gfeferab.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rsztahqf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pzyeubfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkwkrocx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ntvltceq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgicbgdu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hloeqngy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dpgaahip.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkyykeba.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yclehbyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ykhsjrzu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wzjktujl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qxacggea.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2unxrssrh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpenzhip.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wjqzbisq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2djuhvxvf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skhvzspb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mgkkjbul.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qiyoejod.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xofqnswa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dnhgqjnr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2omgjhwlw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zbeliphg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhgjwtls.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kqidwjxj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zkgpxjzv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2roxsancr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2shazhdkq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ikvpmjts.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mesocnof.html


<!-- 参考信息 -->