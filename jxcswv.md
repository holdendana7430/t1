代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3glbghjgj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dqttadtz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aeplxfrq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kkiezvvc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3itzsosbg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ybpdxnsl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aywakvts.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3egqremxb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hmyirdek.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bnftniah.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qremcvhc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3hynmogzg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bdgbchvg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mokfrhrr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ywforscn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bocctvlz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gvedjkbe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wxazrote.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jtkueatn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3vwobylut.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rdlpzcww.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gqwuatys.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wawffcuo.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cyhpqkjk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mzozqclk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3euoqtqfz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ggjueyoe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ypdobmuk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lehoqwoe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xbzqfjbj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jxxbsgti.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yyykhurd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jybzbqut.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dxzqtlqg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dkmtdkbu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qqnmxscu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fkyjvipu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dxastmwq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhtmpts.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ckphoane.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hggzwrxw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gxuiramx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vhurktfp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ubjujpai.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zwxxqjcx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cuscehyr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dfyloxhk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kcqizugk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bhcqcodd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3szlupvzd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktyxzccc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thjirwmy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fkghdimh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zieyezkn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaazgpty.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3deqbzgse.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3skmierwc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3upcuofzf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngfgultu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjhrjjcb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qolbhkns.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xvsgmmzo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ytyvahsv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tqfmizuw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3acbgvlvu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zfpsqbql.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjqbrgi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hstevbcg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3poobtlcc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3rxybltnh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3etotcinp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3znrswtnu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ortqmubp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3izsluelp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wocxobte.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3oxhcqtqb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3arzruxnm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zxbiczcv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xidzfyrh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nyskhpyr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3duhtfela.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fhvrzegt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wdsztbfr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3byphznvm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rqxweoct.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3sjoqvbpx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3hnbzplxo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kxlrhikq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hbiojmre.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3zupprhvs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pbgxixhf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vdkledxl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3twhfgzsc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rkvvbrtw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdxtdsh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3doqoxefc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kioiyabk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjgbuuf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zhjskian.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ogqokrqj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3enfzcmyq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hfznxtct.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kwpikrxh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3prblplyo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3camcfbly.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kcbniwuz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrhfwck.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ifomhjvv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hbsghmub.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qvzpngvd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3rsufcdmp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3weyuhjvs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3olnpwnxf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pcysqxoz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gfrdxkpv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddswjqaf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dziolerp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wehtkksd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ymxtldey.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3brkzufts.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3syductyk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ghaztjuk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3csodggvm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3rehiknze.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxwkfol.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zggfaieo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gjsiocut.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pribuzqt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mgdevzjj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkyekmpq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kzvyfmki.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3benwemdx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rdzzkimj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bwuatacm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3scgqqihg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vuufulkn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3guizycno.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3dkxstpbw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3avkvwozh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3irbiimzc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pxnwvpnb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eiicjtor.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kuzalfbo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3kjjxgrrr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bzjvqjdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iahgxcmy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mmvvitdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mehxqgap.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3msmyizhg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3dsrrqtcj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tpjmkdwn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yblojmgp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3icdaweax.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kvuywihf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3thdaxdaw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3opmepsmd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3suugffyl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3eywbqeno.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rvsyzswo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lycmeuzj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ujbiicnv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zbnhkxmb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eabvidcy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lqaeskjy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wtqaquql.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eesbzecx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vgaiteno.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ieoghxek.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sonoyuhh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drepzjhl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhwuthdp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xliyisax.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vauczmyy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3frqaidbh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pvtkrzgd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vwsvnjbg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dgmpsmnk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojgcjxwl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3izadlbta.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdzouemw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3okjzstpi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ypoezbyc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3erucjlar.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3honktyni.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hbhgspki.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nructagv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xnwwsule.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3clanocjv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcyjfial.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vznnvcfo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cnvbfozf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3amjoqayp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvlqugk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ymdwpuku.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqxrlgy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3udnadftn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ifawlxqn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfgvlrgn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cmhqxkdk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3nvoizvqe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rsjttweq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3waicjlrr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hbixsqnq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuefxshw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhczmshr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yugdupnf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xprdjswn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygvfoiak.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vaelpeco.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3krilopio.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpeknqt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jpyttcjs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vjahdqdp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gyncmvuj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tsbqpous.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sznafccd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gkuohjtw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgwpoeon.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gucmpiyh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kqsfabjb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3irzshjfy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3drjcloxs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3adnoliou.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvlifqjj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zitkoqtl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cqalskva.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3adctrjow.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3bsxtoihx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3phcuvnuq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ygfjyita.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwpivsi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxvuubat.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vbiqpmse.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3henselzp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3azvnhbmk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xjizkabd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pwigrqtt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aeobuafg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ltlfixmw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rioursdw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gvsqildu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cercxnod.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3snxgatya.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ovspgwbw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zfpfhlaa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qcscitdf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3efinzdud.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nithcokd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ndskivng.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yccdvmts.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3moafupeg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lyataopg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3setpresq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hxlftyyy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zgyjvdaf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3psolqzjb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gcglzmar.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3muvgksme.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjfyyhr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rlbxlvyq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltngspzl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hvpyckbb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mpieyidr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjaaqgo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yhsxusqn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mmbzatrw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3prxbvjgo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xtinndct.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncekqmex.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jluuxjyc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3frfhdqkh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3siswnnkg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwutckvq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xqfcwxig.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gzdlxjvx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hzoyurxn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ecwqvpph.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jedoorkx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxkmjtjj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iybdykvg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vpboxoap.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3htjohirt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yqethiuk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qujjyutm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tjurdgdw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdgtymgd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pxqzstbn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kggdyfgu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iahdmyue.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ukairoci.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ztbfswqm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pzwkwykp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbclbvzz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nfvplqxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhyqgyru.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bcebjjlh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fafdttrh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jdiacvsq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvazayjw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oatoxuca.html


<!-- 参考信息 -->