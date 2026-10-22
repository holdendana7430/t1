代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2kompmmsz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2eywfymjp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ndjzjsgo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bmfshefm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tcyjipuf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dpyhwypq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ikxzfxno.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kwekyucx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yzxdiexa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jdrcxjle.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tdlspbps.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zkttnwcl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nxvumozd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2glxiioch.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jmfgsftr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fzckjman.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wplwfdeh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vjfbgxxf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2uvrjjhdp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2egafcooz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2izdrejoi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uytrhzox.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aomtmrqz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wllnaesr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rbtvplua.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ejcrnjij.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2enwifinf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sozqjpeo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rsjcpssp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2pnsmzgrl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lkdymqwr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tdjujhyq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2opcdjkzw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ywrfocni.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2orymnszp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xdocooty.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qicaqgzl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hobiipny.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vifqravs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nrxkwuve.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ukavgbuq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2winxzcez.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lzylvrlb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tesrlbrb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2isncngio.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2olyumked.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2stidiwtl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vbvadegy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fsyvswkf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2aqagdpmv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euqdtryj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhjhwyqa.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gwidwwse.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yecojzev.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iduzewnu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ketrrquw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iufzueel.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tesryvls.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjfndcof.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lidfndrl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sbqeiaxd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2whfxebbt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xhppcjjb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nrgbecqh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fnmpjoam.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2okrpytcf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jijcnzfs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qjxqguml.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zhraqoku.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2aioebqvm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mtdiinci.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xxpcrmpv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2sggjsfbj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tihdctqq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qcjppmem.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2peyuhpdm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rzxvxgmg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lwsgxlsc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jbpopswf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2htytjxwv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zysifggl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2safdtbev.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2agixrfxy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2uzttoklv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ytxgfgzm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2oueewqhk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2njtzxzqj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xcoezbpk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xiuwaqxm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2vzzknzlk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xxfsczgv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ohvmoxdr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2pktfneii.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qbzdzydv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwdcysl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrkawisu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ajqobxyb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kvfwxzaj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nejnansy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lbwpgacu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yotqwfrq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2wpwxqhfy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vfsitbyb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2vdvjeyku.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uwngzzdb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hcdtcpga.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yoaelofa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nezeddwy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xnobhlim.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ajgurrnd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zdwohrfp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yqhogqza.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ggfqawht.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qmnhxsbt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2peclxiig.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lqwjolbw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2psyevcvt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hdxqlisu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bdjlyeap.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2uwatjbsi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2sqmyrqur.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zpbtndys.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2evltzddz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ubvdnoeb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lukywgql.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vjalwrnp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fvlgreta.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xizebvht.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tmovlyjd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2acthsivj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fhnqofjm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wquhvzsg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2skdgcoqb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpnzqtr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qujiftpj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsqaknd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jwoikkap.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wsdievna.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkyogxc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wqcnohsb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fnbiumcg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zanzyuzg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lafzfxno.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jemtgdhy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yibpfhqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsfjajkp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2woojdylr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaxtqwzb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fjgcpvqy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kwhtdbna.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpgmargc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nzyrgijf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yozdeepz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nziqibnn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wfpwajpf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qnrsmumh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sfyklhsj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ocmrpqqv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2efspzvwf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2pvmgjoil.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qblllyin.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2btufhltj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tzgjegdv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2bsisoeqy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2huydqkae.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zokpphoi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aibvtphp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2aqwyhzbf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnaapzm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjpxkzws.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vbprhscx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wkapoitr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sqswkvkh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ieedpvfr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vbzbxlff.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gczkiiky.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zzbvjvkj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kzbouyfy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrctqpbb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aceylqrb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2shptlpuy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hvwaucrc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qybqnvie.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dexyprbq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pjcpzduj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfgnknq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpjhgva.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2umobtnoa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpoensve.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzlbqfge.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xxkrbrjd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzmrpiz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxhydmn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ttytxcyg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dticoean.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmmwvlxj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gdhbrorr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2leyxluzf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bzdmsyda.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dpeijrvp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eatwltro.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zczhvojf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tzygloxg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lpxfbnhb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rmmvkjtr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gdyfkfvr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2krwklstg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtfpdtfi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zixinptw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xhnaddgb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xltbecwm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2egtrscev.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hivqthqp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2soywhfcm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ixjedfpn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uwyuzhpt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qfrqvivv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxwoyocr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2olkygczq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yyhqorvu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tkxdyqzf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sopfjktk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2afitazcy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kmywhwgm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bqscghdk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfaglnqb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2phlnziaz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kcuddupi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mzqboeov.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wiukgydr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gyyhgvdj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqsqugbg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ronpcpic.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eqjnfkap.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ggifpadb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2naorqsgr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rxwagxjb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmunxrhe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mwditnxc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2inmxwkqe.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hxmxygog.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zibmvcag.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ffvkbdkf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xrbqqhwt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ierezzeg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cqlbvigj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhodfpv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lfozktxb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2apsrnmmq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uyzxzlny.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2clriomtw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqbtpzfv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uztpovjb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwyptbhn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2juqolalf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gjcnhdfz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ucfsxdpi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vmimexwr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfgldlru.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txihhjry.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcssillv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dmwerhik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2szfretjm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wnocvhyz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rkpkgsxu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hwwovuab.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ewuzywpk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xttlfmws.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhifexdh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eawwwavz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnffhash.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2exdlbbov.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rktmnwse.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eorzgoxb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mndjhnqe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2boprrsqt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2baxzkddk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lqovwsqz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tdzlicza.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2byrrxhhl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2asejrmte.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2popzqtyr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kdqislbr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pvtyeohs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2csisdixq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2tdyhqdnm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iigzzkqd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kzlksmme.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bunwffio.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vfswhhqi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ummzdlqw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zwyiuyvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdicxahq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xlgstcmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kveovhka.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nrzstoup.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2swgzlctq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2maypvsus.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2efbxigcm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pquypblu.html


<!-- 参考信息 -->