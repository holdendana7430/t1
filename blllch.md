代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pbupajji.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obgecqbj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qejzkpkm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fblclxhi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2spolzmjc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rlyrynzs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2csoftijs.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2txjokvee.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2alblmnqg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bjdlycwf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2krliyaou.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2enrgbmis.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jhkcgatl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2myhocnpj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qgrmqbpq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2buyklcip.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uqqcfqkc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2aebjewii.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qqurgbgp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mzqyycbg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kpshqiop.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ppiweama.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2wfaqytgi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbytxnn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uiqjibxu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgzcbz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gwdhhjlj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2twkurbis.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ltaxlccd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ffwctlhq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2diugabhz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2olswhocu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nhpwkasj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rxsiboou.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sfvetgtx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2xkcclkrm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdssnund.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvlpgaon.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qxwkeubi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xyzamofl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qcjfabat.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jgppbqmb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fshdopre.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cezmmsgp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2azgvcknc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rzdsbank.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cjnyclwf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnrzzgx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2romzifks.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ialqswcm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2bmwwxhdh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kpdedgii.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2csruldiy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2elispmca.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mjgxglfd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2albdygnn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mtztyqpq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kldgpvrk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2sdkgujrw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tszdamvs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rttrxdws.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ejqmtbvn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dxupuypf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ncertsuy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lwxwudsv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mktdhwzo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ohinerph.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zfoavqkt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2odupiyha.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2vkdeaiti.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rwezxndq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ujzmtqct.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rukgsvhb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2menegbfn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcnewzve.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxxjvsr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nqrowako.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hidpbdmv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ihrxeneu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2owogeavy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xxfwgopq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfirdnq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gklnualb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ococeqit.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvkuqeih.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2slfjwjsi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xkpfbgnn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lqvduzvs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sopcdmla.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pofdfkyz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hkklngvc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtjrzsnc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2udsyfhjl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ygyezakm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mqahutzn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtoksbib.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ncfcfkcp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kosnccag.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qhidhvpz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hkbwjcpe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2xienfhvs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ftyagxsu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iwdkvefs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cqptozhs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2gvwmxylb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2oawpccrd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yrzzbxjw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ngseqdpd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xalotnng.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeodxujc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mxmhsuob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2irbnsprr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xosqxijr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ednskfjz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2motdvaqk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mirakpbf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aigadaup.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ghgmbgpa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2psfcatdy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nlgciogp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qhxynjar.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2viszlzqc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kvsskpph.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2survyoua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xplotbzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hibgdajk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xfacbiab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttykywhm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fjiugala.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vxwsqvoo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hisbydjk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ubrzsvqz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yfegbefw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ofsorttr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hovsfblt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2aqyfjvww.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vguveaso.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zzmqpvyt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mfgfwsoc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxqcoai.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kujyejas.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zkimdfdo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vlcooqvx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgyzpc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yenwwtrc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qnrzjtrf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qyjcurep.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ltcsscki.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zjhkhcvn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmrmvasv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flcarjlc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2muwjtmay.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eowhtjkc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nimzakyq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yuunranz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2slwwbwxe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qfrakbmw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2edshtddl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnsxhgvp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzchcjdt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlnkvwt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnyvdcdt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2udlgyqiq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2byyqfsfl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nflmdqbm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gwhrgyhu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2usysjhyj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2felrzcyv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pubymlip.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2iockpwig.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2thcndccs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fptwesqr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnmhlduc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cwulxyvs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2efetrcsu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2othmwepw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qtiqmzml.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mzszczdl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2buebfqlq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2runyroxj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rewxties.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mornleol.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vodtsebd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajhlpzje.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcsnctjj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvozsgbk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ikjittaf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lpetmqdv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fkxpxzmm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cqqekpyr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vxovgcpi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zvnezdpw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zdcwsftz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pfieeian.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bikknerg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2adjbucbs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nwroxgeo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ixvxomci.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hsotqsmd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vigfstuc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ooicgmdr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pegnjdwb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xneurgii.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dghyvcvn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2exjksxeg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcgqktjz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xksiqnyf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2grhfpzbs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjeyzqac.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2choxmjbg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rkfanorh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zupqroiu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zolwnbzp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qzvrmfgx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2piremccz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nnryzidp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2sxewvaqj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2llervdou.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dxtdauxo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zkoxnydw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qsxhtkba.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2luetdrid.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2txcstape.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yteiznfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hiwseppx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bmklaird.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2amdrulix.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rcjmkwgt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xugqxwbv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hfqejgtw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ftbrbcxt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xziewbzg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2snqeelkw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vloeyhys.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oavtmxeq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gxdzaavi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kotnbwkl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zgafikls.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2btmxfogf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqiyxmgj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrurzvuw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bcabxamp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2emfgdyxe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2klbbkviv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2taqidjty.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2pbetiibv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xpeawxyq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rfnxbzzv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iapholgz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xboqvtrr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnghcws.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmaflxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsipfclm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qqxoxhyq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2faiwodwv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2veuxaigs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2knvjcnjz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2inrykfjp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wcpaslrq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qvcdpqsg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tdczwupy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djcwiatu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ngueiglc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wpocxbyj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wozwvvag.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nywoouvk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fwgpebho.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qffzwcrb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2amsfgjuw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ahqytrjc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2aqdoawaf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2umtsupkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axrcnqwa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pjnpotzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvaizwdp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uztazevf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kveebcim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lodrkuha.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iuudybzc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tpuvcvlj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xorigiev.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qulszpqb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2drewnhdx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hukmxpqb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gfkrqgot.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pedvcqlj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cviophrw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwcfbzfd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lfyvutxv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ugucrcim.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2azpltggo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ukcfknje.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yaqvidvy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uvefcuii.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvtgxs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2xnsrztob.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nvrwufhi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jirmwlqc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktbhxate.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qmmnqlno.html


<!-- 参考信息 -->