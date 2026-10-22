代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pwdjltvk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wnmqadpc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2abemeaxh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xiippyed.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cynapppj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ztadgdan.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rfphzslu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2guzfqadn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wvrnizdb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xgxkcmxf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2koamdfqt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2icsbfkis.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2umryachs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2seygvhsi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2digbleky.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yaaprgxw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dinbbudy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kltwhgqs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lhzqutfj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zupptvyj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2aamvtypx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2iiaajjus.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mawuohcc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qvfqztek.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cqpzsvad.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2peeleosk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jvceojmy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rvbaproa.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jckhbnea.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2xclrfmps.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2girceqae.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rtxragnu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wgelqeyl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yvksowhf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2seczxhyo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mnzpqjka.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jwbpnmdw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pivfooxq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2widvsuga.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bdsipapy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2grcqbbpz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fmofswsv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nazemytp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghdddyqh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zafyzeac.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pdqsgduc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ntakdmto.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2exprteig.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qcotahmc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ctdpxtjo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2doxzldoe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bvicjphe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ebgvamcr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2femdumwo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgigfvpw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xxwwhfzg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rjgpllsl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xzqykcwe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2itxpdtyb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mcxcalkl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gnmzejvn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kbhpjhhz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rmtyybgx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mmqlphan.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lhlxbhni.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cwvqphxa.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fcltryjw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lkebmpnh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2biuqmxvq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yjjiyvta.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wsqtwfgi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2brzbeeds.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lkawkhsw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2lwmvhqap.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2peffhbtn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tdmagxic.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2agxdgfxm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2lyireibs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bvpqdhiv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2znadkbbw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2clxzwlmp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jpeirios.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2tmufebns.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vnufaela.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fbqnrwit.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzmphrx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jsrlitol.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dcqpgbvd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tqlyjzmd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2areuqlaq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oesrepbn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2tsyrxrlr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2etlxsnvx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bvymxqqd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zlwddpln.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zjkvrjko.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ozsqswvs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2krdpklou.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iubvhmpl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pivkweii.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2acbnmiec.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2glsgwiso.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xmfuwjrx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gtxykaym.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2umniayuu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wymoksfz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kdjtdpaj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjdlkre.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mxpxgtos.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hqijyxwi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hdrgukgy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qcggtmta.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zulbxgmo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ngxzchwc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ntjknedl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vqfnimgw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxvdhlz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2kzqsgpjr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2emkrptpx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2danpoeis.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cncojzcb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iayelofg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvfhcbn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oexbodty.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gkhmhygl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2owxrwoni.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2seshfpxo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cdvdsbtl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mqhfqxdb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2lrsqsqwh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwtnfbc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2yqlibbro.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uramuddw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wbplzycx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2gfciattg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rmqzjfyn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlavcew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbfgzvsz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2oyzxddiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcyifhvd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ghnttozu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ladkkoqh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2uetjzwes.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tdrjyxpp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yinuuiaa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aoaonieo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2emagwqko.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2vkyyfoqr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oladquob.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2cugqkgwp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pnpchgaf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vljssqtk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yvwcconp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ozstxpzn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vgoakptg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rciacije.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tntwbjwi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nyinkryg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bzpchkfz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zjtazdhb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdugejr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lxxxmpsv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2llwmhbfg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzjlbkwj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jfdrumyt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2csbrtbir.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2frjdifao.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uyrjisam.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wasztgtb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwoxiscj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctybfyes.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxxcqqun.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zkxeumsg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lsszmsgx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ktwbtuln.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vusytzgg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jxfuwnhl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kupykrbg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zzrmyado.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yaiidlcv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cndqugxh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2uwgglioq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cnfhesgh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ibcesacq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekfvbfud.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yfwicmxb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xidojpaa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lbwyvogm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgplkara.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yhekbykx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsebmcsj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qzaqlgkn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lkhqvtjk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2gphxexfs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vieickxo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ttcrxgaq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kjmjsapl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gmhefxsd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgabtni.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tayjifcf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rygurobi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqrhivcy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ykqldxkh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kowsbkek.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ofngppfy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2avkgapvc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qenkfnzm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oklbqvcv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dowdgymw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgrbecz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2neytwloq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bbxwxuue.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qhyymaxa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qgtbmyid.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uorpjzfk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaocsiyq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpwujaof.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lbpaykmr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2olulqzwk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2oufvmfgr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jbqnrnnh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ineoocol.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2neuwfphn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fvprptwx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ytmleexy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ssnpvwlm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2btfbvxqo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mwjdxuvs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2znboepwf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jouqwuiy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xnimbyuj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hmxzzdvp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fnvfspri.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cufmoxir.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2axzzlmip.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pwlvxovy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gzdpmyig.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2adaiwmku.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aacngwgo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2newvqeyy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jnftyqxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kemdpvxk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hovqocpl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbbljpz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhdgbsi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pobtwiey.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjgyjz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hmkvywkt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vabobuxx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ukyygvpl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqjjwvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2thvvfzvh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wwafktnk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2stupzrtp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lxhzhpyc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2iwyrqgnt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sdtcspgm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pavxgvha.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ndejtwau.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2agzqryhz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqlzeud.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cfvufaxs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzmtuweo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dzhqsazx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jnesrbwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2khkojjsj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2umbkyacb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2twqrkpnu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hpuoqqgx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nkhdszfq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mcrxhrwy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2symxjnvi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qoqrawhd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hubwgpok.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oirifmzd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bcgvcavo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vwktebqv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxnejpcq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xamkmeuo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tggdcekz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbblfxb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gctcwzxc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wqcvwhse.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wnipqkpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cesdwhuk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ijjnuedf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgkwbqxg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rbkxwdvc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hnuupczd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wrdpmnbi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ilbxpypj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fhjnncxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2akytzylu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zlepaorr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2zvxesyeq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqzzrdnf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rincpfzb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dkmzmdeg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nvhiuavz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sokuwpri.html


<!-- 参考信息 -->