代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qntdyvqj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ctgrttqi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fxurysnk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hxwdluva.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hrytdmyp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tyoxuazu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2skukkngw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qxehdbmp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qxwjivco.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2veoqmrqb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2lbvkrrnl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vuvniilc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rlunrxvm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bchzpmkd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ymfgcdmh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bymbcnzi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jrzlqfaj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xcajriyj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2itfickxz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ftwolixu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2fxyrwkmd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2keyqljnc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pnngycpt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oxvqvsou.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jhefypzz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lyedysrd.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hjhamjlu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2xoixyfru.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bxtrghkq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xapgajxk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ftxmiiqp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uzjplwwh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2louuufqk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xpgevpnl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2idrozmme.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2puzjnare.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eesbissd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xyfkhaek.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2otvdlpjt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cmfnmyjz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2agyoeelt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2iqssosix.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zahveniz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ieilolai.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dnmhfufh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2amxxqjav.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjbgdlow.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2aqfadqqu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcfzxwzw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2arymxool.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vizgkurm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2izgcmict.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nkwqyjsk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lzgcpgae.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdnhbioi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvfhanzz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2bzbddlkm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kypxymkk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2izbgtbva.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vquwgxnr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2caozqrml.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2okjumujv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2bppnqsgo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2epqsazhc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2sbpnkwfx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dexwqvxy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zjrjrptm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2dmixncsf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ecuyrnyr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nlindmhp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xlfirylh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zujgzmwy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2weydyeww.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2cvvwtehd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2egabxqfy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2wpkxxidu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ncazvfnl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2fuqtxbas.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2srrycqcd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2qultdcvf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jqlimyxy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2dcampqat.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2eokzyxbv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xkbwdhub.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rehwvkvr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dthjivim.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kxpxhkaj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2goirfjyh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gmjfovme.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsqwrlk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yotcaeiz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zdznmlhs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pickllrg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwscwrmf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tfhkvgyb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lpqdmoxb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nlwklnpl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tefscsti.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ofxjswrd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zkiyqlqm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wbinhouu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2osxvyrlc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dospixyu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fucozetg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gzndizti.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rdhuqjha.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ejsbekui.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2dpmubqrr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vejgegvw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xibxupeo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hebywpcn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zdqvlocs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kwaudafm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xwovmqcm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pjvyrnqw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jswtqapp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2roypneax.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zxlmltnq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2duohkybi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2chmekccq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2iyewlgku.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qanrqhsr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2afwjeqis.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yoksjqtz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2izfogpxo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozbegdtk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ibduakcj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dpudhrie.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ofrqrstu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ajezgrpf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hekdxhkr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2dnkzhjnc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ivtvybym.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sugsoiwn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fapgevic.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ceavwiph.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nugagame.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjthaihi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gfalihzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjtmqvhd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qrncjdjw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lkoicnbk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2lqoodwfx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2awdcipuy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2efnvrble.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oymsvrgp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fgzwdmvu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qmmctkrw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qaahplat.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2faxvuhux.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2pxjoleck.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtkmplf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lmntedqy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pszpfxxc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ohkyjhyf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2cqconokz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2klsguekk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zzapkciz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2llyqvfyz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2dnkxypmy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xickxesl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nnohxvru.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrvlyasm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jmcfwiop.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mqedbsgh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2galhnslj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yaqygmca.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rvddaopz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gnrkpcla.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfkbfiqm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfzktlrw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uqtfrrpv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2veairrwv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uccavhdi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2yzfwespr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ppepiaif.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2szxbndur.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dmqsbtpy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihuzvngt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayaiqzsd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvozhsps.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ozupures.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2twzbtqyv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpnmahk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lupvxzoe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ktikeifn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdgusxo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jscbopjf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpbxirya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qummaorf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2plzotebv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jqcwvjfq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2maptjbbk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pcvaskbj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2doqxnyro.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2aimeoyhl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tsgoebio.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mgqfeulz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dhmwvudt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jybgpxmq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sevsxyqq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hjblyago.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2megcyobm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2phyolrec.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wbvdisio.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pmgvouyv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zibdpzrm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2egvuytix.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gvvsxztq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2euahctlc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qjniufgi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uftczrmv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vszmdbpa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulmziixj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2chnewpzi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wrzticab.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hzxmyvny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ddmiyaxc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2smbtwvxo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jflkhiav.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2meuzxlls.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cdrbwlpa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2anuzksrn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zoybiqjr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yraygbfr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yimbghui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2llnudheg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cohozqdm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2smbpczyd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2revwezrg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wgdulxmb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lksrgvxq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uhrjzagk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lhiomtje.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2egwtlxcx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gkyfuymi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2deegnaoi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tykzlwny.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2awyerjjs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mraivupl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bysywijm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vyqdfoly.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2arsrfsrv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vpuicwcr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pjhdwwtq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rqibweok.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jedegckn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cimvuqlc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2camjfzej.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bnaxnwar.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnowmora.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfugagqg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbuevnrm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bpmzwvzs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2fjmxgzuj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2glcspbsn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2iwylkrcj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wvnnrzgj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uinisjtv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2guvyghtb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evgdplpa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzrhccd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kosyndsu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsvqfncs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2expsoqgp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qhysublu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2reiinutq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lbbgfqjs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2shlwhhnz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qwjqxcvw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qejnyuzl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zxkiivsb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bypbipim.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lxkrwdpu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mbjnqgjx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2sbjjosld.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zikhxann.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhtbkwur.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqbfzrlz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wqfllyur.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ozwrpfyp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2sfkromrr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jbjsfyqq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kshpvyop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itprygff.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fhrwzccy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcmruhzf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvscmrnw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nitltcpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ipqzfgix.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hogfalma.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2acwpqrkx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kybovpmu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qascgmjg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqgnhiqt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iyqviqsh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbujdudb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lqsfjmkh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twasvwem.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yocdizfb.html


<!-- 参考信息 -->