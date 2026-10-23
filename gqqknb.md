代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3owelqvsz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cyvixbcz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3janzmufg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kukxhqfj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ixymdliz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3usshkktq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rswkzqxj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muwbdios.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdvidwk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wpnaupof.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zxmbgtjb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gojwrhhx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3gpkqzcwx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zdmuphpw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3lcjbvfcx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gknvaphh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3iduxrrqm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekhumbhp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wysgspqy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qxyfksih.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzkeawg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rbvbzeum.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tpvkaxqq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ppuvrbax.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nqdybwik.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3txfzpbok.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3enmjahzi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wrkyvaoc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lnohpitp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lshlwecm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fkcswybb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xomlxgvv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3szidviok.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ismwltst.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vsasshcx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ungpdcru.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3odhszvgw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qfhzepyp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zrzxyidm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3uhrwpbjr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3egpeheub.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3stnmvwxc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qencbvha.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yipnoftb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3igoctlbe.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wphevxge.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brgonyab.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eaabblnp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gryfthco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3dkyukmts.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ppgkcgcy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mvokksfe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3egguixtq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ctonuflp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gveuxkfb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3cqczpwfb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pwwkjxve.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lnyjsrce.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3micfegdn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3htacaohl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oykcqvyk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3boblactv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wpvofkdr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3wpivbowx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3oxhxtbly.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qnzyycxb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3idjtghxf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bubbgbtx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3nwmpvxnb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tfnhxjkk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxbdrnmf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ghxbkyfx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3hermhpup.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3hrylbmbo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kplenyiy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3xjbxlmld.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tfnmpars.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpjinzwq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymkspctx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xynekfwc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3swehmfxd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkvzvmsb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3prpzudlw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pzjqpmkl.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xlbsswlo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fgldsjft.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzuvbvb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qorwwhte.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hvllkrxc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qwgqhiob.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mgomiict.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cqdoorma.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qrxauxsp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fzhruhzi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tauyzqtb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3imegicex.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wywjnker.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3edwwloja.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3utvrfwka.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vjfdwgbj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dujslfrw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3gxjsskpv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hkrcavjr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ozbzodqb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3fplveipw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yiojdsya.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lxsffzld.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rukwzvzp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsjenlw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3svyrvslb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3nlgiexdj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cwmxuvyo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tmyqdpvq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3orumegsn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zcduphvz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcjvecd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kqkdcrju.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3razybzhl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bqaonwmt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hyztznlh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sfgwfbbs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjqxijm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xnwgvlwp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3gujynyma.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jwrcfysq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3gvjpfojo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkkfvzi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3msalaxlr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jtnbfrjh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3melhvhis.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zomtxszk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlyhduc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oarztvzk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xnwzlacz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3idpslusp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdqeuwzz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vlyfcggm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3blwisawn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hycmdnfq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lsiizrzk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gkiamccx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qedvaamg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jlrqfgtu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ylkbcfwd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujorridy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ipedbxsj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3awcjprmz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vkdbnjhf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3hjpkxrlu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qkcfzohp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3thasyzta.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hvupyflp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ewbkucgk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3woijfoms.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3wlxmiyvk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3myevvjud.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pwtfzqfh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3qfoehtws.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3axssmfsq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ykmorfty.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3guhhianl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zjjlhvyq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vwzjogmv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3qopozkki.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnjxccw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdvzjhrn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gtpcxxli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctrhxmie.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nrgigsfq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fnwpvgje.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3afcxricq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3shhpiaqt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3airximkl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3muheioyn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ihssygjj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ccsjlfdb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3szjxiuhw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dbzhntps.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3peuxcdxv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3coxkswmr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3arrgppqk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lescgubg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ddyvcyil.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ewdnnhue.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lwcvxeks.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3smembwwa.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kecptjcn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ojnnstkj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lyliphju.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdbnxcwx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqcmdaf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kqqckmmj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kdmctzua.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3azprofwa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lqtbooul.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tmcdopag.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zepqxwok.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ximrbyxu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vhluhhim.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hfldqyhw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdixddnx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nvezckes.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3iammxakn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cnzxvrcr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rqpeyvhy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfmahqe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxtyiakf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3slbwhcwk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmsdnnck.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ycosgtfg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3csriongm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rpimsddk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3blqozqvj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3apvielqb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pioywqbc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3clakvtvx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3manozymj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cavaxdel.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3icspghos.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yiduuhho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wuhnxtlg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kepuiwvu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wclhvnwb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ncykkacm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3guslkmhu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vidslwjy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljktyhgv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qoquxnus.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xgkztxre.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmoshmza.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qqnusalj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3txruudta.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3evidsjaa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ecwfgnsd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nyavhcbe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dmyxcibe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zurhryjo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iyjbkqpe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3syiwhrsw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jkugqldy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xclatnit.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3itwzfnhw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtsfvtmh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nzoegqas.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhokgzhn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mootcjvp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuldzxc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3owvuaesf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjvaypxr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3djtwpbmg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nwlmywja.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okdzxrdk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nkadyzqn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3znpjdlsj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxcrgvos.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vmuronsk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qwibnymz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3eagcwuoq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3htrcohsf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tdewssar.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ajgdhzba.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3htngnpin.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jfrplqxm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3enzblrdo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hozvwysj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ddzvpgjz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cdimmevw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3smnirscs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3iwflicuu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3uqxktymg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fviuuqxf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yjjkilsj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vmmvbxfz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bringwgb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbjjnhlp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3crzhsmyn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gsbtdkqd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lwdiamgy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tocpnfvm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwkmddnm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gnblkzzm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zefvybty.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tknrdpdn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vgooyjar.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3njpvhvpc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xcabrgee.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gersqvfl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3elrdeycv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eiypzbia.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybpfcvub.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jhmvlcsc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3snhjnjdy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vobdxtcx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ijfussir.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ygdxlzfj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gxzgrszr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lqzymipz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3chjvauyj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rogvkujn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fnobrjel.html


<!-- 参考信息 -->