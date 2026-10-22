代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aowwsryx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xfqpqyae.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2stsifblt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2upaqjrkr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mvxpwtnq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dmvytiee.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lzudcufv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qtzcidqj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dczmafhs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qdwiubwy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qliqnidn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ykbhbrmc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2uyhfdksp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xnhrdvlk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vzixlrfa.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tqyywojx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dsjdcdei.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hgnbyhxu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ccgdcaji.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xhiphplp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hyzbeoho.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vbidhlgm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rgxcthzw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ovnufoih.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gnxinemr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xshszhbk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2yrtcvrnt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gugtlpvz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ifjdtguk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kdduwuyk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hihavrqt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zgqylrns.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2tmuqaxve.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xhdtafwm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtdfrgqk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lccsvkku.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2grfsqciv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mscjfqbc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkrnlmvn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hefunfqe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfowfucq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hbykqjyr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2puqcjlac.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwxvonyq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpkbspiy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ygvjtjrh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gwhbbzlc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ekpvgldd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2nsmdikhf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyxrkkh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2inmswpjf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fwakmubz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wzepndap.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2sijelscv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qnirkdzv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2bykmxkhl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hqezvegu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2duuifbed.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nuctygem.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2cjscwpgt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tfemlhdl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rfpqzups.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pkajwxbg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rzvkcusp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xnkxhirx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rbcvmizp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2hedqwfde.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2clrccluk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2qmrjqcos.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ayrsodgy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2lmbdvghy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bvxavjfm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2okqdbiza.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2humywnel.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2tcihabbs.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2gwbxirlb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2apdncnkw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qgyevmkm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fllqjjtx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qbhhwxfw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ybfgdrfb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wovasbkx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jyjquagz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2fudvecow.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qjgmclys.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2odqsrnnt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vitrieee.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2phtxqntp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fxoqbpcb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qplkyxuh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwvfzkgt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cnofgdab.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2kscldwhf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zjqrtxjc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fyvrylgr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ejdloaxb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yqutvpse.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tixvobvn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tnqgugnb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btjzdokm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2moldench.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2gdznucuc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lhxupmhk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wrhncozm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2tirrritc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2otqdjucq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qolzyloe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xosyqkex.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zribigzg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bxvqszmy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gaggfkih.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2piexvgdw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2rsqggunq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2bpptnsjm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2plcdltxx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2llhefgdo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fqdhrvsy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2apihcrmm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fqudvgcg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ltfrglfv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2moyfobwj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ibjbuzpl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2aedudazh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cddsjkqq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pdpurvba.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cienueal.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwuyzudk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ropttmqf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2njcodqxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inndvhas.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rkmxfwgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmahagja.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2djnncbse.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2upmyfezk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjotlylq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iiwtutcs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hbtftrsa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iizpcklp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsqokgo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mmsygaji.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kvpkyawu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zecevvkd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2knqcpppf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2tbvsshjs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sefbkvek.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hcavwxtr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pyqkwuwc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zrxqlnwa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2bxbfepgv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ycpqpmgo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2avpipjic.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2twhpkpwk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzffgmko.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ganptotv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdanqouh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2csmlgwqg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kriaansc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ktqdjppb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pvkycztn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2msjkcvnt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dfsuxwev.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kynfvsys.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2apuazkku.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2todxjyan.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtbbywc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mtgolwlr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2eaecsnhr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bhsdkyde.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2owcclscy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvjusmu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkceuelj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2guiaaoet.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dohyyhfw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hjvlqyev.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kjnrjomu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gkvlhleo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zchqwnij.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vqnporbe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dahqeuax.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2loqxhsid.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gssvrsxk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ekuagalm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbkbuuq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xbmhczuq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zwralclo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqncehzu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lfzickvh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzevamdr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2euzjdfyw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkpbqxsk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sevxnjan.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nykucogu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jdbmfwye.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ifbtimbb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aadaifrl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bbqkgzec.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2aynsaony.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2juysgtmt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ijvetron.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vanwlvbi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rhmjsqup.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cwubzdia.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tswxamln.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fctshhlu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gbbfsgth.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckknsymg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rmrrboka.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rflcddtc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ssauurvg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2igilhpsx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oydeaodk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2oocrfuhu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sovazczx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jcmkjubb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vclqwdbz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2etqiucdy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2psaglydk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uuxxafzv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ezpyuazh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ziqngxuc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebbvkojg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ugjzodjv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2krsvoulp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2swkwvwwf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tugxufmx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hrmazwmk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hlowcjvp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cummsyuz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zhrqewok.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2orbxwduv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dwwrgdis.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2anwqenoc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fymdoqij.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pfyljlzc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cnsdbmdp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxjnfskx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvzzkdge.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2siwzcpsc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uhstkztf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ktmcwzqb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zpjjenvr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rknbktot.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mztiyedv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjeuimb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnosbkkl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vaehnynw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2aiszgvdl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aqmymunv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lprhddns.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zthvpemm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bmwndxve.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xpryaobl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ggoapttq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eccdmglz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rjahppsi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlnbfixz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fewrjeaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mgpiyeyl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nvtoqjme.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2iltijlou.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2baolgqhv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zxmebcsq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bignmgsl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjucplvr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ekdikpes.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2asuanwdc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cvqnyfvx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2suurdbwm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2keymefak.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dccgsjri.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vchdaqjj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bexugula.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bkzwioxt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wetaukcg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ihqeiqye.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fphfvaqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2toeefmhn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tsxiemkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykgdvplo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xluxbcqc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2scmhygdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gufbtdqv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ejolehei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2efxzpecs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2evbqdmcp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jxmevhvv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqgdwkrw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjmnpzz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdmqcrqp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hrcjephw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ieehnghd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlfwvcjt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgcbnrhz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2liigwbht.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tkqvhele.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wowamwen.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2aggithtx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2egizeikg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwpliyp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nvlsgved.html


<!-- 参考信息 -->