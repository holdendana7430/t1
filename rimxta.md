代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emxftsiz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3thlrtoet.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yuzkrewf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghmeshni.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ziyggwwh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zciclxwm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mttapozq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bdheopyz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3trarfery.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nbtibmrk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xlrebncs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zmyobdwe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ufjkunbr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tslhkulq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tuozhagd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3indhgwxa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbyppxyn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yjtxvuqp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3brvqkyen.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hpwpulvn.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bnmtsjdm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3kkxtzcoz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kapqxcjh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vabyvsxh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mkpireaf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gvkxtspz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tnavpspi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3moylimml.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tdnhfkka.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ljphhlfm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vtlvbaeq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cwrkwccz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vgrrzflr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qswgdjkx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mipvmkyv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3sqxpoybg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jimcljta.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qigmjnll.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ppnlvgvg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3otjzrgni.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3qrcddreh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3chdwpcjk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qxbdctgt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3sbruylfj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3pokimlam.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3osymyvtr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wfvuzvlm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bodnahpr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zjdnrisk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jtdgdcqi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qpocbfdz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yyzsgzip.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dzlakrka.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3siqwgksg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3trfocxoy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdneaveh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pygiefgh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3etkfximt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lmtlbeki.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ulyiabsl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bmknnkqv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dfdwpfop.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hiyolhod.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3gtekktpr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3iuqlmfmg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3avslmxju.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cfhpxmaj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3oddvfnxr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tfkuwiil.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ljluhuqj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fdphlxyd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xtsifbws.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xnekynsx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3egqmnvjv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3anjzwtlw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uapecoaz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3kohwkpzz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3eqkroimc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rakpbnef.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3thfrglvv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dfeoshom.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ozcuhytn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3akxolntx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zlnflwph.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ediwcbaj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kyftprze.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wptvaxqb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gfwwheth.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aitekinz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ykzusftq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aihuovrn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3wjozaldu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zrnxcmre.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtljrnfu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bxknrxal.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zmaoseyy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zfakowzu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3afraezhg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qilzxxct.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dlibgkgr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3niwrgdzr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oyxbzrbo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3baziocag.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3bxodutam.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mbgtmjca.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hcskewnd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kiwtsseq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3uqefszjj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mfzkqgwu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3uweohyfq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mawxpjvz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gugrvmvb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxxyhfl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ypfanfzd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tsugltgj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jtyfclxq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfqpkhuw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3xddrmooy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ktjwvbkq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3odkcuvkt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3wlrzqqyv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3sdxdvqmu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufysxmeh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyphrbtd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ozlwwcze.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rddhjnrb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3axxonrgb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3grkzvfmw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ovlubhbb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zhhhkfvy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qknbbbod.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3najdbimk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mpknquzm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qqznkmfk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dwahtadj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rpbqilkj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hfjrsshc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgfkrpfm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jffxnxcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lopirhut.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3odojmequ.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kgyffkaj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqicqylb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xykfuwgy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rrxglxnv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jsdsnmxu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3kwxitcfc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3aamrhigk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3slnifraq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vyzgxnpj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mhtjgxfb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwigvucd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fypamzlw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3unavctsb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrwwiokq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3uidogetf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zonwkyth.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jvcrvurt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wnuvyzjg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3loakyvxj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjgmpyrw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rynzlrci.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cimxafkp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3khouzdcf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wtmaygqj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vcwosvwx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iudnmetg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3krldwyuu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3obebuzax.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrximvru.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vzkrojjm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3btofmjmm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3klseazvb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rrhvknbm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kcoacpxe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydfeigiz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sjncgwlg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ohcegsnp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tglsuygw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfadudrv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vhxichgs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rygcldbj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vmsihexj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3drzkfity.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlihhdsa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vmxckvou.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3aynaecfc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rlfrljpj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qidxynga.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iueeebws.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qzzquuei.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ijbmyhvq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3enefyspd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3grmsvcvw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ijvjofwo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ozhcpvku.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cluofwrk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3acaiwiag.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aqzxgcqf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uzzkgehz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mrktiaen.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxkceqgv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zedvjird.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bismkakq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3suqsgqcw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tzjrikgd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tpofkvoz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ktpxjdgc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wyvopinw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vpwsxvdi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3chzaanke.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hnezzste.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ysinysny.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gkzbfgtd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rnifeeil.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twgknpak.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qhgqljaq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qvrjzwxt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yxzxrnnz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mhtdujje.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zfwiaxvm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3pioboszu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uagnimxg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zapmzaan.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bwrnnzrq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wbnemloe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lldzauuk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uequvsfi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uoepexdm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3evvozjbe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3efadtluq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cgxohlbu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qpfkqcye.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hwkyhtuk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qvjtzdos.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdpwdphr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3btyclach.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iiftnxbn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gstzfxdx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lsxlrkdt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3syvsblub.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xludhias.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xzucwdsg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mzuefjam.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jnrdoimc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygfbjspo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3atwgoriw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3sxhtfmgz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uxenkcrt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3aijcsupl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwuplme.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmzntuio.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rmlhywaj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3htywjxhg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3izjpcpii.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vwkfcicr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3buhesguo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qhflqnqg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qrcvhsnr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hkbgsfdz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmjnlcz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sfmyisyn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qmfrpimg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxwxiwvc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjwaiqaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oxlxnljy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3skbfjrec.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tlhmrlwb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bliuemyb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nnrdgbjt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wpefytoi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3upoimhmb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oqbeecev.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dujvdpcr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hrvwnwed.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xbppvmkf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mjifdnzs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zfjkstyt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jyrmwpyj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ghqxoezn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pwgtgnfk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3unpbrogq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gdsobbwg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hffvagbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqxhobvs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jgozjwge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuwnjiqf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcuwvbkh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uglikmry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bdblgwzw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mskurqwl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmzazevt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jfurproh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3agcrhxlc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mjirsbmm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rwdssqlc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jbxvhfdf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3uawoahce.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpcjgkvo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3buocmxdh.html


<!-- 参考信息 -->