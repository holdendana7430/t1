代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkrhxhnz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3idjwhwki.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pqtogfew.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rsufkfrc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qdeddgwq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vemlvqtc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bcyfywsz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3irqfnvhe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jeojkftd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tsxnruoz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qlkhtgxj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3waatztnk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3znrbdqae.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3mnpioaga.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tlmpgrgc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fmycsmmv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vuwxcgji.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yysowkyo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xvfzlxnf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zagzfwpk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lblrucln.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hsedgvsj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sphtubgd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3beojfiuj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3eptnejze.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dchwiuoy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mtlcnyjw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3fxgiddoh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ykfsijul.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrqeoa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3cixjmkzf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3bojwfdbc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jggjulex.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yczilxjz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dzxmpupd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lumcuyrj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dqwoihpc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brihfvba.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mrjwvzjy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3auprzhoe.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pnhpgqsq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ftyqobob.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tnyarorj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nfmfgbba.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qshdhekh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3duevdvdj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3shhgifvl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3zybyojhf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gtfiaddo.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eiftgxgy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ymcjiice.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wrmxgjmq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tugaojfn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vzjasgyx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3haelowjs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qjjidjkw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vtmrxkjs.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gjqcolvj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wlpmennf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tcoxkfvj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fbggahqw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3nosnwkwh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxndgbsa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yhehordj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3amfembym.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3jsjwmgax.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3divjnmky.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3edcxpcah.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qyzxfhio.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vlqtavld.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hsbwfoun.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aqzqkesd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrwzlrjl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lgezloid.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpuxbcww.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xbyppuqe.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rkelhiia.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlqwfbn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pohwsrem.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wltwlktm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uollyyxz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3tgetupzy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vhfdewxn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mbgjuoyr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3xauxnjvw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3snyknkbz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uucliiel.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3emmiizwu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zjpcyyoh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uvxifgjk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3oxzsbldi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fvrzitya.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oaatwbtz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cbffapoq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ubvpsamx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ghbwwhfe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gsyzejdh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ephfwmrr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3isesczqs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ptvjmjud.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3fqkbwobs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3doohwgos.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3djrpwmjo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3zavdassj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3amtbwzba.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xctoykfw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssqwyrfq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dueqpkxp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hxxaqkdw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zkzbdzep.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3emunpres.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lpbfnstc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wbrkelrh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgvtcwt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fultychc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3oazfoecy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3cettssds.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3poasgqcc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijspcjhx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3yqgkolwi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3djfrjwwf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3grnvxfrp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ifnzhhbh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3rnoytett.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ecbuminr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3imljlhtg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3egdjheax.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3unhjxcci.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vlqhhylp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3uxnwojwt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3aeudnmqy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zivzkpjt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yeliubjp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nmwimwrb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3khbjqlxn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pidqxvxz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3yyzawxcj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qxrmgpkg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wrdtpgxn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3umuqjwau.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3txrsmaex.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fvsywcgn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmpwxybn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tmlcrgxw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3femzgmny.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpfleyn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xdqlawef.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lzbugqht.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wszpexgj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mfvslbuf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lvajypwd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3egjwzwvj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yvxixoap.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3upsovizg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ngrigepw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sjuxnivw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gouiwhdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylpigqgo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ytcrtwvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjtvfgus.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3apdvvkja.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bnaykypr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbwjwycy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3whoxzndt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uyoxsdbt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rxxoddzg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwpizsh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3idvbgogy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mepqfnll.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dhhhsrsg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3aqdrkysp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cnerxtat.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vcgiquqc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cqkuhmuq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lakkgcvu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hkgisuit.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3bbgglcku.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vkespthc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vcxqvfsm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tubiimsg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giafplrm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhvdbnhm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhugttn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3itbndhlp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ubahntqi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3knfljdad.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gpfdfxmk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fhxlfjmu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ahovmkxv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwdbdox.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zchyhwls.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbcsxtv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifiaenfd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gxqhlyqu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3btazasgj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uchaaaho.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3esryshmk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ydakpyyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bjbnyzza.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tlbsfeyq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmvgiws.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3johgnjbh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vpokjpdg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rtqeqwfk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxvsfhlx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3acnyoolm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pptdufea.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qciestqj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3prlzggih.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkrnxlye.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rjyrjhum.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cclekcgp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3brakexmj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbfrgpwp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nopbjlqw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3iocesvrl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eswbztte.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdjowrkn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lzoxhtjj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pkofsexr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xrnxjpyw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kopmzcrz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uqeygasl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3yhwosasa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3fvdlcewc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ttlvnnsy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hiaznryo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kbmzxeuz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fhfrinhw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aghoqwrt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3cdbvhipt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iqyzjckz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3otanyyps.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3klxoesrj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3amurbxcm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctcjygrk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnujeqmw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wmjghiwa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wsuqgffj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3brpnzesb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cksapliu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wrhnadbz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mphltwrn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ezmumxos.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cxqrgkzs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3avjgwbzd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rbykqcpt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3schzaymg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqrhdzec.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uicayanj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3slkyguao.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jbdipyzp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdsjeiml.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qpvkxrck.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3afqvrbzt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kjvpjlqg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kntyiadu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rxgbrtgu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tigfuael.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3glsyuyta.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3addotuyb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lqvmdkrg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eekgqwly.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ynknacbx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhsmwokv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3apbeftyi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3eanewpgg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mmvourhx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bsawfwub.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kdigyyjr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kydpakqj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ijuutxzc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3piksxejf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kiwpugiw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3weqgezfz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vmhsmsdi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vsclvsbj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mchhxhkd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qvuawwil.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cnehwtbi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ttrdoaqc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zgldeomy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smegmmcy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3etnjsvbo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ildyrvwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arphggfh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ueiuuxpu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gqtrphcq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rtvmaotk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3soglfhrl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xvkokpaa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yagqdzpd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pupxcdvn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3daqlznsr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzvxszqu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qcpwucuw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mequdwxf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xxglfaul.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wbtfirnt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wuljdmuw.html


<!-- 参考信息 -->