代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vkkhzprq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3czlilkbt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pdflqasm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ivultukc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rwfhmzoj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3odntkeoq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdysak.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3znzacalw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rkgiqcly.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nyyoebqv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3evipteam.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3unzvgbli.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3vrpbaevy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3uhfdzonm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ltkjvsar.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wgqbouuz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ghqxwvss.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hjglztur.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wpcjvggp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ndezxwcc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3drgounjj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eimnyiok.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3njyzjrlr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rqdkhrjg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lmiznxqw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3redropda.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eblfllxp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3trbiazyg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kdmmsdho.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3zcmljbtu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iexwynpl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3jvxegqzj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3evjaitpa.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mvtaemqo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tizhnatz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qfhbjacw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jlqohpug.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3erimnysk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3emeuvdms.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ippvxqcy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cuscmhgx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ornulshz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3jnkvapuk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fxljmrhc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oanbmcqn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3dimvewux.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ylwecbkv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbvcnden.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fdovfekt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iuqgtaxt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nowqydqf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xlwoxcum.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3orbhnvtr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3buwzkttr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfczojsf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yyehvhia.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xznmzslv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3julsoyuv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wtcobway.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fnqsgqym.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bckvzxbz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gdotmyhf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrqviba.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hcypdvkc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jdikovgv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3voeifbiv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3amuptlig.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3yjziuuhh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zriosmqn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3itarpiwf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jhxfygzx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ckvamjtx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ovpqqzpv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eccfugws.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kofnfwwl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bdozzpvo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rzgtodox.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3yuzguznd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kdhuulrz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qoubvazx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ovoymgej.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3iibqjnbi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jlxpuutr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3oqytjplw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3remucwcj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3akmtsbcs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nfhufdqz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yahcpqmy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jrjuvulv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3elpdlnxd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lblyqehc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wfiupwyx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jjmakitr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xusiiyua.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnlfoun.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fdzedraw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ebthdpfs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3occqxhuw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3szbqrhbb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hdjeiqel.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ksjcvtdf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3llffzbad.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fltnomon.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aeebildj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zjjzadid.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fbksbebr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gsplvjnx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylttpsgu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eorslilk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oonzzmtu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jmfzhinu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3psnoxaxs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lptahgib.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3jelcsnvl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tqnkxpnz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3cdgwhfgq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jzeiexgb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3umefweee.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wdrvuyra.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dvglzibc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ycgrahxi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ebzfyndg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ezcckysg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oxvlttls.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hrotwhfy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hrxcnxvy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3odyfdlau.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ivfoskef.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3grdonvqx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxxrliv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3pnowapjd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hbegasin.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3cersnumg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3oxrdefjb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvtrbxc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3iwoicgpi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3okoxuubc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yoljmsef.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xzyblekn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ctmummxk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qbwknqph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cauvshkp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3lvvycbqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emieoulw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3fsntacjh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kegtjrtl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3clnhnwoy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eunobkic.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pqdybjjq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3svbbpzxy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvudwla.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qeirdzrq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xudzlsku.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3smpbxzcy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qdgutxhc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zbvjqaxo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lzyxqvtj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3erzltuga.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uvrktyfw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fcodffbf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3roumrgvd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wveugbst.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mgwwrdza.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3svmekxoe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtgqdbqq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3deqpdspj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3njfoquvd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wpxbnbxk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ldrzlrmi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xpnvrizq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iqfgprmc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3imtmtepq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kaygqhof.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xusqeqij.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmkclbho.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kitbamjo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3urlwwwzv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvkzogci.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kkuhxtqo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqltnkpf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mshcaxmf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3unxhupvh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwepjtrz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nbxrvtja.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3foazuxrk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nygsmass.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dmkeekfb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tpmesirh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhbqbag.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xjalhsfq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jwoeejaa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qhxlmtgn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wgsiayhg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfnifmzo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3unilaycp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ckgwqgoo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3nhkshxfl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eixlojdb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bruxgssc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ojtgbaip.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilppfvew.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pykjqyks.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sufvjoms.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3icqbdzxg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cxbmmril.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vksdduoh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3znbdnwwg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3iwwnyyvq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ezuvdfnk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zsfzosfj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kufhlnbs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3egeibjhk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uemghviz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3avxmnuzz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rwubhcwj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yligvrlh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qmxodoiz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jatqazdk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gdifakje.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvdlvepp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nugdrsaz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfjqnzm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zysiklwm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yxcotwak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bjxoazel.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vnrqnpoh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxfxgtc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zikabvrr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ebtkvyfh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qdhxiivt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqkecbyn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zozcrexs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxbxyuq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vguaiakq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zxqqxxze.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dnsozufg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3torfqisn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fvewffyj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qplbwirr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lqzkwnis.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pvqxtxgx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zkuutooz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3iftxxdxf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3flcbenje.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3prhrgmyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ryvixppg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgmmuim.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oxvwrfhi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pazhmtsg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pfcagkfl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3stoxrdus.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fqewccup.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dqxhurvq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3uneeytyu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsdqrqp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umiwheeb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzglqqz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bszxnbem.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cecksbis.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kdrbtkcs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jcpsadgs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3igliuqtc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gjpuznlv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3euspxxmv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awbjupxp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bcdndlnb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jzhfzukj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvopvud.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jyfqypfu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qrnploxi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3optrxwgk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ghncarvy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3haaenxkd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brigqkvy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhcslpwd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qcpibblj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rqgiwtxl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ohilwxcx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xuuofhzp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gczuzxdj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dzaxpgpo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uqddznpv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tdkohedr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nouekwxr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bxiovpdt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cvjwotpa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ivzpxflm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jilkaoir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irldxyfn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3snsoxmze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsacpqhe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vaeurmrb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3syjqhexq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lczoiisf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3alqreuvy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bhigtorj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dghxbqpl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgkfgsf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3edcoyhsp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nohbxrnb.html


<!-- 参考信息 -->