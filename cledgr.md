代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2srekcrep.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rvxpruyh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rpmjvbsg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2etukcsnj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2indzzfvf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2oyfielnp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pjbwrcgk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2vqqtlmch.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ebfggqnd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gkioqbof.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nnzfzfbt.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jbpfluwm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wdnvvedv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hazcwmbx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qrhohfjb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bogefycu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2phvopdeh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xyqbnzmc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ktswyjux.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mcgdntrm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cvxnudyc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nudpxrto.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uxeqdedc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rjedbecx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ejdzgxex.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zuejhuqd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cnynmqwi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qpajgkfa.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xdcuzfyw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hybtynpj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2pnbfbrkd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2znhoesta.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2njpnovam.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tkdulgfz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2tniuotfc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mksvnkod.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2tyhdjifr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2yutrbshh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcvfcumc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egxetbxf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pqeujagf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ymmwnidm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwsxgekb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qkullifv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tcuxaeqt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ognofljg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uskjwbhf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhtsqraq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbvltrna.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jfpuzuqm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2busxwuqg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2flelicwm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ngybxwtj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gcsvcalw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ukolnotx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ujxjmozp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2plnybiij.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lopadppz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2culwpsyx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bohpoczg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2eohfemfa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ebzhhvbg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bjrdybvk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2iflyuedj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hfdqmtvq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mggasrkb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2nwhgemvo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jajrzjqi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yrmmhqcq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2okeefxte.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2henuyvtk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ziexmtde.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2kkojrjhd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ykfmolnq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2suewjgxm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sjjonqtj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uhvqxybw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2znjaxric.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2uimpbxei.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pyvhquux.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dqptrllg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tbhnnpqc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eernducr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2regkdttu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mxfglavw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2alzkuzwu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2riktyrwb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2acikicpw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rhbsjrhi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2upofaskx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ryqmtutd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mcczsiig.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rnuocaip.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ffwdmpto.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkllvfgq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2dzktoaep.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rxekxsla.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhnrnqud.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rfzjpsve.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmvajine.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lokxjbfz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2efkpgist.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dmqybedb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2epqrrcnk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qgwrsevh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qcvzkjle.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ybqebffm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2vqpvmrkh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvpworqj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vcbfgbnh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sdissgst.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ercxqyzk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnhfqeo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2proajruv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rlnrovjt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sjhrchux.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2wydjbozk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ommlqftu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvwpdsab.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzhhwrc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fqdvxctr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hrxwqtwl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mppdgrml.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hcrrwdvg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wyxlgsty.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jygrnmdn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwbzdcp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2abyfkdjd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gtlkbenu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2aqeojkuo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jeotkiek.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qvlazabo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cmduwayg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvnbfhje.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pzlrlcdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktfvshwz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2myxtrgdb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kbzflyis.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2iphqwiyz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2itfkpfop.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bisnamgb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2whushlhm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2izrtxohm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ftwntrjx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hnwkeaxf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ytotlpej.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vdvxpgrj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2djfetnok.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zmggzeai.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aidqaeqi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eugwtnhv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2badbjgip.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lewbgjhx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vlvksuio.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mncvxdog.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gvrqvmvv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvdnjbm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ohrjfkpv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btoqvrqv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jczamhfu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rsxdtxce.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rajwzsuc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ytfjxdpe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kegpjeku.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fokdyajy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hghygwwy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgqvfnht.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uqoiglhi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lkczkeog.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqhkzgd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2uwtnmatt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygrsifai.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rocsnmbp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2spiidedp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mifzghbi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zdaqhydm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvzuxlp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zlomgply.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qgrpkffg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2msliptdv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2htdswdcr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2iuhjzjmk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zbghgvvn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qnhdfwhl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2itonrtuw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2udwtkuzk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2patnwmmu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2akwprwqj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fcatpujn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wuakiimi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2kbmmyixr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ytwztfks.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsgdqkzj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2skhjqzhl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfacqekw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tkpcqnmd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wxcokruy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kchhooot.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlgbmgjn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2igapfpei.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2afjxrgvv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2deemzydg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bbhrhebb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jcybxtql.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dqzxzahh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2edkgekme.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2oozpyhhi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xxusuhps.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wdfcpzkh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kivupnep.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pzouxlfe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2alvtflmm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vkgrsspl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbjfysbv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dbrbnvbo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fzktlrko.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sjqfduzx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cnzqlqaf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2iesbzyod.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqcijfwq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zsprjhwu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xdihgbbc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fipywzrf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrsazput.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zfleqbcp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nylzbnct.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bymzzrtv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tzdwnios.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjqtudtu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ivwmlzne.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sfsyaogz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2amufjxfe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cwbfdyzx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pwpruixa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rxilenrl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eiaofjni.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wtyxuqug.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rnnauhqw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jxzptoou.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdbqoqsl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bpadxuqr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mvkpktnb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bacwqbiq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rvdywuqd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nvsrazua.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ttsdujab.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fjmjckmk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rtuwlmwn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ciegtdam.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2eujhlcsf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2epegmkbu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ioknjuis.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2suizwydx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ccvzfcij.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2joatzjiv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhksamd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zdightza.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzibxuu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dutoiaue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mfgzlqdq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ukwxgsix.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbmsuhc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fzqdikop.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zvawahqk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jkylwdof.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mwfmckvq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ngcknfoh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lxqdqxja.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqebxquc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gwxswqqd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcjgkzdu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2eqyqexqr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ozitvaua.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tantktww.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zlmufhxi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nezalsli.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hthemzhk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jgojyljj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xdedgsfx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cnzqjemc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdkrwsnp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2fptoisvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kayebvsu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yujnxbgv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nmnofplv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vfuctxoa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgogqfxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxjqukgo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vimdbguh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qvltlptu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vaiivufq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oagfwohc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rpfrrhvj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hvdmradl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsixptol.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2viufhtqq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmervj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2meqzyzxd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uznttcpt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2npkvujmb.html


<!-- 参考信息 -->