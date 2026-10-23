代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3povitbrd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rckoxhwz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xquiojge.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3rpvjeuze.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3shzhuyzc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zglwmszs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vyjjyfqa.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3hcyvybdj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fzebjcot.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zzxegbam.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ndzxajwv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bvddftbh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3tqptoigd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ztnafldw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3akycymeq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3tzmhunlv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oxjswstv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mfatqdej.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tgdlpamn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lqgxoreg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ydlaqffe.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lirxzdrc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mknaivuj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vwmphgif.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yqshqifz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vpmetpbg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zbcoszxb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jnenbpdm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dmordbrn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3jqtyntjs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hrdghxnq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3rgnqksbr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3btqrskkh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3byvtcwut.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ebmzlrpu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mfbibrpe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ksyizbkz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ssnovwgz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xnobtaiu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rbjmboyw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3awloibfd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rcrmdvsn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3cqqzkybo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bjgjcvmz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3swczpckr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3yqysochd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhnkkkps.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbjxfeqf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kxroyeve.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jjothzku.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3drbxvwtm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gnnndgsx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3owgwmxfm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xjfpdmss.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xbgxwpun.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nqwnvxhx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vcyyfifm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pryujahk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3czznxiym.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3chsmtbgp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tsmjhlty.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tsommnss.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kvsmqizx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cegarfje.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfezdei.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3chddcqoj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3sbwybmvi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3arjsrxyd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3spltqzvh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3maunxyvk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tegvhumw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lzodsyfp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3djzuuxec.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qphcjtfa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3hlhpugkp.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ntvviodk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mtyzdwfq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uqgdmokn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xluzgxgg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wxatfxus.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3knrpotbb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mupooyuw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3qbdyndtl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3shaadchm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxkpxii.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qwccfuhe.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wiuizbsj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wxrbrdfm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fqcavrsj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3agtwlqkk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wxbwvhxq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tknwonwi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sjrqtwcj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cxzcyhtz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3chnelygf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jkllmlgo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vngytdjr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jjutcvcf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3eznacahh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3izokmwzm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hletbvwm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gbojiist.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bfuvcajq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dowviegu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3gxnmmvlq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bgdsvpef.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hafuwgjy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xutjxtfk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3djpioqhq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sjjvmufj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ktdqanyd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3shlrwxch.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bzqwqyaw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3psscpbrv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3sromzbdj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3kjnqboda.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3nxikkcek.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3phaalrcp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wwofvwnk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3aorjxdkt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldheenhl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ivdyxilh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3reqnsebf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruksfvbu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rgieovvi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3llvnrlfv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzcnwxrh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxnhnhw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ptdnxtzx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wytrptzc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3axrxiazb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3idtmbtwb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hvcfqbfy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yqscmbon.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3czosxsww.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wxitkawz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gzaocfza.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gfmarcvd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bilcyvyd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tatvxvjs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zubkqyuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsusvajh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3dtpvvmcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuxfiklp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wuqmtxth.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fbwstcnp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmiorrwi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3disqbohr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xadsfwon.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3igeosqbs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ggczgdzw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ebenopic.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3puucszby.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3taopbhta.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zdlyhwwb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3imalnzse.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cegsmbrs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gilijucx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ivjxjpbg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3joywvwog.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xhorddus.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ywrxwwlv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lqneostn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vnqnehgu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmnppjbu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iubkiekr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ucoybutr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3autkzxcz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kgbtglho.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yhhajqfw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yqdeuzuu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vbykxeio.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ggkfqdde.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdzxetj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahlpmqoo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3amrrpsdy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dflolmky.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dtagesrh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pvzcappl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dfyvfzti.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xvxnqqlh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xctwubly.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdkzlztz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ccmfkoex.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vmmarulp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3idwjhixe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yqyzwkaf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3muxlevdb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3shuxcnwm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tnfnzbfk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rldmfkah.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcugrrnu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bcodnnei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nxncvtxf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3auhaapjr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pyyunjxk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3znfijnkd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3htduigxy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fvlftfkj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lncyhgin.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydixdymi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3spytsmtu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esayaqlu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fprnnufi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ngvtdmsb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3nawlnots.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxuxcgeo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jvqwmcyq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jipjwkot.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3slvqdtau.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3faxlmmqv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aezxltcr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dtiodgoe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lomtsgjj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wvazvwyr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zuobhiqu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mbcswaug.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zytqdqal.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xojgcxee.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3osxwfzjc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajetyfla.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bxatxttd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjnoynjc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3szfrasgl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tyfwocyq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fpsjkjsh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cbfyoyfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mcsxhkun.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ubrrqwts.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xkmwvmwb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ngljgtla.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jmikzwta.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dtbtulyl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ewuusxte.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bilsobxm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lhwjyfsj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gfprupps.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3btythaii.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fyoxbddg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxauoibh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3msmqxxjj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kgcbzdms.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uchrixed.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3whgpizkk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pxcdkatr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zdxwjxig.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bethhsdg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3znzsycgs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hvzwhhcc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cyvcpsjt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3apczjbwt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3oeendedd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3rheeztpe.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ltzswwpa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3enzoxyaj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kucapfzh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oxwgqleb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dwddenjt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rrqbdrtk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ggfzjnwk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yodeujgi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3inmssoun.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zzungess.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fzdgliry.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlrheeu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbttzlrw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqjcwko.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pmygehfr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fesnkzfw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvggwzwn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rhxttxze.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ptlyadqt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ajtoyqqt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3geuglhme.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qmdsrdlj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ifmzkktq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sbtywhun.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ewjwulpg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bkxmmsdy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mrbqdbkf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3outejngc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvjvmpzq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jckxphlx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gihhtqsq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jdnxwaah.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qpnqycki.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uuunzjcs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvtecktz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvtiqlzu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uqlrcfuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckvqujab.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3avqfcvsm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3euzevhdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qezrlcmd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rhjsmxnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqnesavp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3olgindyq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lfhbnvjs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xnbknvjk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvqrrui.html


<!-- 参考信息 -->