代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zevuimre.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xcvfkvvv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gtnevmmp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rldfbsjx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2njrzhkub.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ehgdrysj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sohutzea.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jstdaqlw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kgqgvpoy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2jpqpswcp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xlbvtyoz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ershmpct.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eoovzpop.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vfxkcgkq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kyeuaxss.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2hycakkiu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2klynzizh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2pzceuupn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bfwpgiqo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aufjbdpo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bjskafie.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mhpnpcxt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2okcgpscv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2pnmvhngx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ggbyhkne.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ofwwtsca.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2uveekfxv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fhfddkha.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xpkztspt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2iqowtzov.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkhdjapu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmzatpwy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nvtkdccm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mcqdxmtl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkudrknc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2avxpeguf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vhohhtbl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jerdfkfg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oyjyoysz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uftwvlrf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2enqfahjw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbqplrhy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrzfdksi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjiqpknd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pshfqhqk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ywtzmfij.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wdyojqkk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2egrmcejn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdnxgyk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lsndfjfb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dggkxeyi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rxnkzpda.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vgzdhqgu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mamltlbr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eyqpdlhz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2xevhhnss.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dskxgumb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kavpxvzp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2tcwtzbdu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zfyyvyzt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bcitagvo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2liclrict.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jcsmsyrh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ieeqnbkj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hybnwntw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2csosxydc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mvakjmne.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xtzdzodk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2smshutba.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2igqwqaxv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cuyarogj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hpftjblk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xbbhybbm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vynblfbe.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2txqyoifu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oxpvtlvv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzpueqz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2znsddkik.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bctydhmz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vwrzohcg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cgtjvvdm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2angvcacg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ouqhdpcj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2utnjllry.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2gtynmorm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fbmwfctc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jfpaumxy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdwvdxhz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hxpakiue.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjecumns.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wzvsgzgx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xyaetvem.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2anuwwrnp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nfwhwnwn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sxaaglny.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2migddukd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aziswypb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vxfpgnel.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2dmubxwsq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2oipsrioa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2oeiruage.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mobjrkuy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2whciwyeo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bjzjishq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tighyjng.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wkcffoia.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bvhevigi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2swrlunua.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vnfgwlvy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2okhdwgvf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2igtboyfv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkhmbusy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nvjqbhpb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtrshtjv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bhdqikia.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzxctgj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2byxdnocx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2itclhyas.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2csigtzjy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2gyobhgcr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rtphhbry.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kxdmaxio.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2nskewmrs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zkthuxzt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fvghgcdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsejhivh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vxmxvlxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnvoxfem.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zrmacpue.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fgaouvqi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2voewujjr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2quabuhyc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zhijfuak.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fjxwqnfk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pamclvnm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wuaypunr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ueefvqel.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jbhjbmwa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xgmepywq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kglulisf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ubdcbort.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qymgcnkt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kyiitier.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qjrukiwy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vqceexbh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rdivrwvi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ujmtvltz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2cftdqijz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ansiggrv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhfhtiuw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2duwqorvu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chwulhby.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jqnijsoe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ckvmhnoq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vyveixhl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2drcllmfx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jdqelswm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2efjlsbeb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rlfsoksq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfuybuuz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuzmemaq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqyfvkc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xqqstlyy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxazksnq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2czyunzsb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2igthgzkr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpodbvba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lbdqueje.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2itbwbmrr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2crrtaqtz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsseamdr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2stzsjoqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gwhdibkd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ayggoqwu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tdjqjyun.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsfuhr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yltbodku.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxssocmz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pwtnjibz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cjieretu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hmyvmpbf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eigtgsnn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bnmqzmaj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zfpleazu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2awkkklsh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bniefnet.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxpriamf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ixeqnghj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2pnvyelyq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zrgeenek.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsigtujz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pzidzapq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dysnhajp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pfxugdun.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aqeqvutu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2npwnpktf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xxhsetpr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2requukru.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zmqkafso.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2azwdonln.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ajfbgqyw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fbudkoso.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdaozom.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgfjehkk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xvuxtuut.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mffeawnr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nbldzzha.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gscwbtvl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2flqyenzn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ybaseryk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zagyuoru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yrtueovx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ackzpbcs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fmgccdjj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwxjacwn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pewovqpi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ntwksdnu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dtedbsbj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hfackcfn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wjrbueey.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2eopmbpph.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hbkoisls.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdbufucr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vsgsbzfc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ijyseuos.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2sqgxkhrl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rwturlar.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2skmozgbu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yxtbhslj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ecgfttxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2parjoytq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fcldzydn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bcwtfksf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vwsfknut.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rjsclrpc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ipqvtysz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jkflwibh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yuhjgjzo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kystsfvr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vicrquyd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zkiwqedj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rcekxkpq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mrktxkyj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwmholx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oeircaer.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2azjoavtg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mfatnpfs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vfskimdx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqygucn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2agglrfhg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pxjuyszt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2idzfycoi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjlzyea.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eqlfqato.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ahnkiuuq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2expvzojs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pasebufb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxcalxpd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ejeeaxwy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ejdmdats.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcijvjdw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jjxhppcg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xjjsnlhk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gyphxrni.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2afqkyfmr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lihpyxlr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wnrhuzps.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zgxapygu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pwqxlysp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jugltccv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zpuncoag.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oikmyjzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndhjfvfn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mqgqmpmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjznfygw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ybjjijug.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dfarcaes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2blrdvlen.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qdcmvpff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtyuifqk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lczwyekb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yykgdlps.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eshwvncy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouubwnjl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcwwtvuw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jkxypspx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yzkdesiw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rcoxnwzb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dgrahfos.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dzcikhrz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ymdiduvc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xnmubsxr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2beraicer.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wduwxwvv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wrfomqgt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2etniuwea.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2opdhrqca.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hhyuhmrd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvyubrbb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2svbedlfm.html


<!-- 参考信息 -->