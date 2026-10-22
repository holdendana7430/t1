代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmydxkse.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2orcrgtbo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jsudwwxa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2irsttlwi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qaaywlfl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hgvahgly.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dsnenxpe.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gicgfbrk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xyrspbih.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2npagvvvg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mcixbial.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gydsbdhn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uexfzaei.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fbccnokw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hcsbssmy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2axldlyeq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vhtjgjwo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dnhcpeuu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zeihcwvc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhaaaji.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ebiupkxa.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wczebtcx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jyngfbcm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vdyzwdbk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2otoxrvfm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eiwitgai.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qqbguect.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bkqsuvox.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yhtthtyu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ybvxwoit.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xtzoidvq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mafkxbao.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2mvmoacyt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fsswkrrf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hkmifmyb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qtokhwen.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qinwsjyh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2fgiinpis.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2phwahful.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kymsfjmq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ypnefoer.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tbmhhqsz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2snniwbzk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vznoffbz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bolsbzpz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ocirxgtu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fzhshvpe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2otismhrq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qalcdggx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ndkqawns.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2wrdefbtx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2bhzilgae.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2oqcieauo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dtazfxeo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qcngmniv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qflvfwmu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yuxapyxg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kfnzxhsb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfvicoth.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tgdbtfaq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhuvgtyo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2isuslsbk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdvxtvzl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vaqnhmso.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgixgzlo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yiyowqvy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlwphiky.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttvntkga.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fpxijkso.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jfkcpzcr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hhbfwibv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2egswmpvj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwwnjfb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2qctedsnb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zhhpktyu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lgiwcbls.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2noptxivn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2inhpalno.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eykfnqdg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yuetfjxz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ioiheuha.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cntgqecd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jeyyebeq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pzaoreal.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jrtlcygj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2nrrxmcnd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2doyqxbfj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2geklhxdo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fzlsgejs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yiygehep.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2amoaotqj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wampcrlx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vwpgqqyr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ayruuahj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bkjhqjmq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zceqzzpw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lfukudpa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qmhsxoqo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqqdwee.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nmjyfpni.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mxesuknj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kappmmqx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ippposne.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lcoleawd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vbybvrxs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgzrhrkt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ijajjaon.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fkthvzzp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tdrsuusc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2umelbzsl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdgzxpdk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ucatruzo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ckncvemz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfqqprun.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aezgrmqr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2aeqohwgh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ldrqugvw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xniqavjg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2budhlyxa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kxprxtwf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nclmxdud.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2lzcwpaui.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2kibdarya.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2yaxxhiiu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nymtwjjv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2multtdwq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pnwqtjvd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cynloujp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2oewdfqvg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hoyblpmv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bngyuila.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bajprfqw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bxvxuvzi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdenjro.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcaenhpk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzwabvht.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2saorlmsn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iidjrzjj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qdyzbfaz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2libwvolk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2kofyuair.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2nwyapjvo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jkkdsdqn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ryiyhoef.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ftzvvaqg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vayhnvdn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dhhlxeop.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jaybeoyh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2docmijhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxtssfvu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2bjheatto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifobtlbx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2aytamsxu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ddvhgdii.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ldbcqdlz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uwotsway.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rqadbwgs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mgilcpjs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uakanbsb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jbdpccwe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2scrbgmlv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yjpwuzhq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ejnjjffw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2binhbphe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2saytnvzt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gubhoqoj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eroohxjk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2aeaftjhf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2skensgjo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mxrgjhjd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hsmrsngg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2stndauuw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2satqoysq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvdnjhx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dmtcdslz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iywzaems.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdqmzaj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pumjvukj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hbdqvirv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wvixtipu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2putztqdi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2byijaquv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uuplpizx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2larkdykt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlalbqel.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mlznpuxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hvpjgfvg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2evvngnvz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ydfnpdfe.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fdtqqgia.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2paxphmbx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjkgswj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2udxzmfrh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygxyonif.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2oinmihqk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2orkhhbyq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqzsbdrj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2efywxfhl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nutuekgi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrslvys.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rgjdnuah.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dwdcwuio.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2frtjwnms.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2oimrkntz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2stkeuvgm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2azczdoxu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ueftjudn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nnkhpurn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fproylof.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tqoinnti.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejtcguoh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qqgqfceb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dvurltsm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2luidyfgv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2npqowpze.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jglfqmea.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qxfbqixy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wnozhdln.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pxkzzrma.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bvdzvdqi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmlrkpy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gbrnocmq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2suyqsdma.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gugvntta.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2skjothmy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lsfyzjik.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eslbtoal.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pjmjuqwo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zxtvvzku.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uepoclxy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxohizcc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qulbquig.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsthwfm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lqximljb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nasgtkhk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bswmcosp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xwuchzra.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oncsdsdt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejaxauof.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ncqdufmh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kghxqsmn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnnmtcak.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2iuapkycj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2iakrnbgg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2crdfghsc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ogwnwvuy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2peglbcnz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ppyjvaug.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2shvtozbc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bzjerubq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zwceyufr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bttbzeyv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fjildusb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pvxpfqkk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2predlglf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2upaocgeb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ahgzjcfb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2exvfhztr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mhbwkrgw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gplstrei.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rgzfmzsg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2lvuqnmia.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hijkmggs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pbodixtd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bifmpzvg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gnwosyeh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2krhvzypb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2adlltiqm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dqilvhsu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wsexhree.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zfelucxw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zuleymdf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2clhwmohi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cirdkayb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tgpnbkln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vtpxlhhc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uojovbul.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2poagwccl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uirqbxpy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zqiuphkf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hnzsfaqv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zpdrvror.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qdzqcllu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iagnfgdn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ddynpuhj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sgydkonl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pyattmbf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lrxjbbal.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2moeqnglz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnfncrjt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2joesblfn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2icpdjaum.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gavuowma.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jitpjwxu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2aimorzaw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bqgsgshn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hurlgnol.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qzgdrwgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnevuaiq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gbhduwdj.html


<!-- 参考信息 -->