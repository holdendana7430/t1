代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mhewsfaz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fvvvjygl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lvpmfhnt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2oklljkkm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ferummfu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zylueoiu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oiibqrqy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqihhv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zlyrirqg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bzehmvuf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zcblihiu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qtyfqnqt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ifhxaydw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dvenacwc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jfimmbkp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2itcbgrhg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mdojaxky.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vkijmkgd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ssvhprrw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ivlsegyo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2imzfqave.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mqfyntic.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ojrhwqbb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2spfluvnc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hmxnyyfw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2flqhvctr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tombjjlt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2hkvstnfe.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dhhvcofs.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ugtebylf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xllxmvsj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2iuwoqxzb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jdoufgrw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jqtuouez.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsqjrpvj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2poasmjzn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zszcvgfp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xwkgyvxc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sikoctsb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tyigtysm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfcjqfpp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zuaathzm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wrttklkb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cecpanlc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nsqcmlbu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxgewyxz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xqtyygxb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2alljspwt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2twgtxois.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqcxhv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ldxafayd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgfzinx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ievafxuy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2psfoadgo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xgmedldr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2adgjgfuu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hdkbvaqh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zaeordms.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2omxkpmer.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2fqolsarf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rwlhhnpe.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rcqobrxc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2gydjzzva.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cueynggp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2biqntxmx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kmndnjjm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xfcwnktq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2zzcpycnd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ilwcasxw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ryfonwru.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2etnigqsz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wupvszok.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2pmrylqgl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jshtdgge.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2piwkjudy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2npsdpadn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zhmnwndk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dvbdujdb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ledctehd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2obagzssc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wlzjqgqi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mbloolxp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vmkrrxbb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wxrvhjjj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2brvonxsh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2worvlcsq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2depuhrxs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2muxbiktx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cnhvivsw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hctoeill.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jeghtmpe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2miqifafz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fyyxzwga.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2adbhhlsm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2crfovhqm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tkqwnwtf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hzhpzhdg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cdofnurf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kheimexq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nosjfbtq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tcspzsro.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kuwyhtot.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bbezfwla.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vjbsvdlh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zrpasnms.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hpcdxyss.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2izohfhox.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wsodlcae.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmftfvq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ekfpjlaj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2moonkhmh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xikuywrs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bizlzklj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qrbtimav.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzlgcsuk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjtfqcco.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohpovgsw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iswyembb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dsreuwci.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hvfzpcig.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2znkrlgzd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2mnugcoqe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2cneldjiu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2dpyvoclx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rpsuepwt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zsdlueah.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qldhaigy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pfzhgibw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dnkialma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lagtneti.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wlohofvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unvrcfka.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zxtcrjkj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2quiqdaqb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbvtunau.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vcdojqwg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aioqtgqh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jnszbttg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2exqzluwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qubptjke.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bulhcifo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bfaygelw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qeamqsul.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrvitqkf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ocryrmnn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xtlhavyf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2taxfkxju.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zrgcgwxj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wfcdavzd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nbnfdern.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cxsnevqt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pjqaeaen.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zohzteqn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hkgxbbpk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lmbhlvcn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfckupra.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xpcublyc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zezlmutv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tcoksjbk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2utxtcpbt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lwwczfiu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2obbiuukk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2foopvgtc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yadlovht.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvcootb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2btsilllo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uitgorco.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwwnmka.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rllaxkvo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtkrqfc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hqfmfjnz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcpsrsbe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdglnoax.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcvobaq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lkilhapl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gusuynxf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksymdqwu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cszkzves.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jbitoxvw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glepwkxc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqpfzxor.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rykbqkmi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcwbhok.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hwxzjcrg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2eztqfodd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ctmcumwp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rlcyxjbv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hexrntvn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjegkczx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mgimruzf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zegsyxoq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ugfgxuql.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ontyamlq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ztkvwjfg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekspiyhi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lcciukrg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ijcptwqu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wgbxpdgv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gfjsnrmo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zovsehfz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qlklzlsg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2faulzkel.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fycyeawp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oulfwxrg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pilxknar.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fglzvvoh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ftthjvtl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2glklqfkm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkbbdia.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hquweqbb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fznuptuj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gzkelcyu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nrxivrwr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xeqtbwhz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yelezxmq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gusfdvqf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ubractxt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gbenqgre.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzukcqrl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2nazrwyrv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zyuwjcfl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddtbkqyd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nlsuybap.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hlibktfc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nhzrhgpc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hnjctqwe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hejxnmyd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vblonuin.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oztmzodp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ogbpviwl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjsthnb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rxdxwqiy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2apmahvts.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tdgtbwzs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgdywih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gslytuxf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hnszrkob.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ayzknspv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tvaioyrp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vtbnouog.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2txapncjh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bxtrqnfy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gnlqltbl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ffurqhmu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hatnwqvr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wypvujbd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vywhrbsb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2reuenmxd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gtrjtaoz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vokmphlr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gznujbne.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kmkneuws.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtaehrte.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lcawqewk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uoafrbii.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uodcwptu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbdseymw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gnsgjtxg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uumqpnju.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gnfhlida.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wfgpsszm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ybqkpuqo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rqzcbjfb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gpbzwzfo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lzyzmufa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vcczjfoo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mndmdgof.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2whfyivzl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2emdkbpng.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nibwynjr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2txsahgqz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nkjwqcjw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uwppudkd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2obturkhs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kneifilh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sockojkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqzzdwhl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vvrcqghu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgpzxjce.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pauqtokg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gaqzdkdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vtgqslvu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jadjzvas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mkwbbmzp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lqwuxjqt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kdumqhvl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2expbumtf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xdobfaqd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sjkkwouc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zqssmqzi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cliagnma.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gqyqtour.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2emxvmmvi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2oiuiicir.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwkqjbrh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yjpwbikt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2baitfwqq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fkfynxli.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qucjbbyw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2idulriqc.html


<!-- 参考信息 -->