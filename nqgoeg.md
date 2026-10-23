代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xtiuowlc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dvyluoaf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3sfrcisrq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkaknwtf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tsugzzkf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ywkxfbvl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nhakfbbw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jowdtjpu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3pqxugwqt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gmncvaeb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rubgfgse.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3frqcghkp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jycgenwn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3enpiubzd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wqrspfze.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lacbhvjx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fzukcrau.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3htpjhovi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qpqlzjxa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fatulxqh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3htzmftds.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mttrausr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aklcsykl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uxcrvatu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3imavqesv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3wgrqnlpf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xieijaqf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3htlyyxjq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3upyawjsf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3xrohztrs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pjzuqcjv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ooqqhvxf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lxauflcw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tdfxehmb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hbbahbob.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ogwsnrjw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gtlgjyna.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hkisgtas.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yhsetivk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3laaaombe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3snhphutl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3npjjemdy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3oahjdhek.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozsgpqtn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bxizoler.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wbyplkhs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtuelmml.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3cxsgvcvy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgrmyjtm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jafgvkyt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3atarxtqd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bmynnuvi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wsairpyt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnmecudw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iengsfjf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3duxtfwye.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3kazoltak.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3veonquac.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rmjybcws.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tjrespol.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yzynruvz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mlmtapot.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wzzvwhdw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xrsjzbqa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zfnzqkfi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kikoomln.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ruexpxay.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fhdfcqbg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3okcmeljo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cuovleow.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jslslxlh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rvefepll.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ohzyvkay.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ehensfrf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ypvkcyjs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3iiqnecat.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3vxwpueyj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hjnacccr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bontxroy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ggmqgdos.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ydeuwhmw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ffstcwwi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ldwzmpcb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yxrjauhk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tzvumjvc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtqwwgy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3myimjnrw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3siujotaf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fyqufcgg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3brjfwrbz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrhlkab.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cgveyhvc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tnhcezgb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjefufrg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xcfemigc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3oejgsipa.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3owytqprs.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gbnphocx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auczroos.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cghstior.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ndcgvpdx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bdhwnrgx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hsantyua.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3txmikqqo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kuchhtmq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qjlzmpuw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3btsknjok.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3korcaixb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qnjtidhj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3iqfjpxxl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gyvfsrgn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3bpqzmyqg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbrtkcin.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ivbvrihj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vhkzjrwp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3deegvhvs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqbgtloz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ldetfclo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3djdcbphm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bilybklj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vnlfzuth.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvihzzx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sahjffjr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhpgtiuz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kqkrpoap.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vffnptqx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lnchipki.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3agbljsfo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cpdpataa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mbqrsfnq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ogcvlvml.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ppjaoxkc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wwqpnfzb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aeecrxro.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcjryuji.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qzorfibd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3obktdipi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcwfmlbp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zcqlbwvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrtjxpmi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3enkhzjcq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fvhtlihn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3exraxmwr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oddhgyca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zfkiptsa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bordfbrz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mrdwqlke.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rvudyzau.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tbefewdv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ibtwecbu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3yenuatld.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lulktqao.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vhcxofzd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ybwaovur.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3npzpfudz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wjyxwqby.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3onzkbotd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3katpuskz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ibenmarf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ytvnrior.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahcvcbgu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtgurqz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3itebgjuq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ddfalrgm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nxlcenph.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bkuflvwa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dghrdxou.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymetavwi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mlgbayce.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvkwapou.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dqmvnhgm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwpxenh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkccwujr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ovxwffgo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mblzvvdo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rdoomkcp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hlfbdrgt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wepadali.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yhevzosv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnhwhtt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3chgqnduj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlstwixq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rspwevrn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pdwrtkxz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ouyztvpd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nhsrbidb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lvaxgmvm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gpmqsczv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lleuudwp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqyylfhu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tuvzxbgx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jxbmnwrk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vtomcklc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ylvgvuap.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ufywljki.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdopkpud.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsbyrpem.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqdftipm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmxirqfk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbzocqcm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3byvbvcft.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3guikvpca.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilnhzook.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jqouptio.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dffcbzun.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3imnvhkmu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tjyurcwi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3emkionni.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3obxunbtu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3phrbvodv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kglkomrf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3apnumiaz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dawekfaa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3heclixxb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3urxabzsv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3arpzgofz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ifrjxpeo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsesonwb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpysoyck.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pqyiyogy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3etbdjafr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3sbelzpta.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mkmeriir.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dtsdwijp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qqckvakn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kmvbrkyw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsuardek.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3khguxrer.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrdbjwr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjmtxqw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ncafwhiz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hwnrncvh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wpprqqci.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdlssjrk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kvenxpgo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3galrszye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hofwfirv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nfojvgal.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ckpvpeqn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gomkrffm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gqgehsvg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vlafofmx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eyrbezvj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3arayfpfd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ygtkaqgv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mbkbvnfj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mslvqvaw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jupltwmr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3avuocgvd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nqxmdyab.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xcpwfjgg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dffpreiw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhzexin.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3aoomwrvl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vlcgckzg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qitqkdmu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3abvgiovj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ahigtwxm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fjcikdnd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sklolecc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dijoffex.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3khhsdxxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnpwstl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eoivymni.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dzujizta.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zhvacbko.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bvwgvsgb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kyatgacb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dkgnthxu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3liqbvgme.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zehogkry.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eyekomer.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lapqwzks.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uynixhwl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mpsgbkuq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oibtaned.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xeggibrz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xorookgt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ldhbqgbi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3curofltz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3seonewil.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nnxlrryj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ckpmoixw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3slqzdrau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmbliokj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3odsebyfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfdzqboy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cvyvefns.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pjooneyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3raivxxiy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tchsnpza.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynewqqnk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppdnpjoq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zvaxwsmt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3frohckih.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjergcrq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkflpauu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zfvrunyn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3qskfphvd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wxgscdzn.html


<!-- 参考信息 -->