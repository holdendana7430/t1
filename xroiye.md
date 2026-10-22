代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2plknfxal.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jomdocwz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzihce.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehddordr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mlpxkjee.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lankoots.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rivxhwbj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qismovua.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2duajfnkq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2fyzibgly.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2evtepygm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bqprcpbm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jyipuedl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2bqkndajl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eqrdahpr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2tzqstzzz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qygwgepo.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ejawuxxj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ajnmpgje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dnttkuql.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cunmtvid.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vyuinetm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xrourqtq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdtzcom.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2exkguqkq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2caamjtlo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ksghlncg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ghmuwvdt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ruquwwnq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2upmgtaik.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpjjdkgz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2cjgpvune.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hvjezloh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uuoayfoa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofetapva.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2corszsns.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvtxksxt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odcvhzwk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2soirwdyf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yaxucyuv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pvnjejxk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbiiwwny.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ooqkpbil.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqyosdpc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ephlvtld.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkxurzk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ycwvfhaz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qetagdbi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2csnsbkqm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2yvyjfgbk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2qjwiwump.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ntfyckuw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ktuqwjqz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kaqlgvfp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cgmuwrfa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wgcoqvvz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ffmebhtn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dldqlbcq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2skekgtjt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uotvzjjh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2urmyraoj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2clkdvvzn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2bkvhewui.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2uriztyyj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jwbnbjjf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2fwzqyads.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2owraeemc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2tmivcnmq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rndzyxxy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2guaukysh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2sthawbcv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zhhsaqhh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2cazjxmkx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wyngnoas.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jtyfusth.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvoanowy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dfadvvif.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tdupcwxx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjowbhv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2zhzkvcjs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nesgdwip.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gaudnuan.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dptwluxv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qzrqahgw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2yajxpcqv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jqhgeazt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lscqhhrc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bftqzogq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hkalhaml.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2izovktpb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nqgrpxya.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfvzuvr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zsfpfrld.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bqphupcw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2erbqaxtj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vudangyl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uzweqgur.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mmlgeogl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xhhqthhe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ruooodaz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lwpnfstx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nzuvcuiu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yycvzjkn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zahcumfn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2tjhnzfmw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2szigozkc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bkjhzyqt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nvysiysp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mkpsqkpn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tggieixf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2smfegtte.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddwqqhif.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uubnufce.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qendwegj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nmjhpdgn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pribtdvx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qqtcctah.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zxbcxudz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hmwavagg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oyewddkt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2sljgqsct.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fjasfxta.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2diefhica.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fjlxjqoy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qsubcnef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvaqlxsx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2iykmdipd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reofbpmm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uqxcmgyl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nhmblrxh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2uaozdbzl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nwjkjxij.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tfbernxw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wjkxthyl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2toqbfuma.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2oppjlnyw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fpsgmgeq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2usftjtwy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kdwkonxg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrtxhxna.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bqrisgxw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xfimwpnt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nyvpncwj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xlktnihr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2npomlkdz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tetyzwms.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cibobqjh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ifpjjxgo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkmvdjkb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htjrhoas.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hexnxhjs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgmcuugf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ngpkrwyd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2tzhmrqfb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sgpibdeo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dgygikoc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2idcyktsl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bszsimul.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouuopaki.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vilrrwbd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hymicqck.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rcsjkgni.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xrsbnylt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2efcpgfte.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2phqumhge.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kveezasw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2asmqzfsp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cspavoer.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2owjyjbdj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptinwfls.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhkbsek.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ndvvdidd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2toydxsir.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mxvwbuum.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rcxpnhoa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2enycijjk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybbtceuz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttdavuxh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfunflzw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mzayrkvy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fqckiiyk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxjgqfg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yiyvsxys.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxizqnfh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzmbrtua.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uyxwqlcw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngzkgdca.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmwesesw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2sdfwxpwe.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jzrinfji.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2figldqux.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2revvebnp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2anempqdn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2akjsaqew.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ozmmpxdh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ubxlhpge.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2halfgbjb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpjdcqwx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jhxmdaqj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ntbbxrtu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2trdsjkoc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2utqwghbf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvprqsc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uiuumocm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubeboxwi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sqasxulh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zwpnjuqf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ogztqvlw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2smcwkisa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pbbkxvih.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2egamxihh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aerhwbkc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ygkcxynx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qlzckjnd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdhwovv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bvhxving.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xvqpxgbg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ftealner.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bgqbegrv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zkosjyyn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gennwztm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2siuywdrj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nmsvqwfv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qhqqicxf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ojievjtd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ulnivvtq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ronycuzr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2upquplvu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fuweeedz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qfqignjb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejdwtiod.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2thowcnpt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xvshgvst.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjlfyrny.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ndbplvhx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2crlzlomh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dbrambry.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2aotqmtsg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkgacqtn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cjkbztlc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfvhunw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hgwdvpsz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eoorsfee.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wswkhnvp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xhhtdsbr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mjtxvwgt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fmwgyuyl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bpcdckei.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qossbnai.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwguikxg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifciivkh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpxyulj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gjbqkjth.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2evmsbubh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xfpofhcn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cgdabohp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kumwcldv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fwqwtprt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ylxjhyjm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qgetdguf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zqjvnoev.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ebdayict.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dxaxwnwa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ydiskrmm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2izhswtou.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrevazwx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2spihfwwc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sdhzqrwb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jozjxffd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2akvfolni.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2isvpuwtl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lwucngxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpkgdrli.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mibfwuui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kknxjmgg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2laseczcg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2udujbedn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qceyrzwz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pdoqdrgy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgmxlco.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmfhyipw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dncsmnjx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhkzpbcg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnvqwcml.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wxcktuem.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2shublhbz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibbsfhoj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcyycdix.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onkieled.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rdstgqjy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2eanhpdrr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zcpouyme.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mrrbrbnf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wedlrfaj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iemzdsrm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fhxisclp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oxculawd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fpifujse.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2seodcvng.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bffrhawy.html


<!-- 参考信息 -->