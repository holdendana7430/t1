代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nalylcdo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gdkravsl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qtroasvm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3smnkpjxn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3jgewnttg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bbaoibkf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ixqdkcil.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rvxsxfil.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ziokbxcv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3buxnqbau.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3egcrtvmy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sycljuzl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gqpnpwsm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sywohpvs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ponnsqxx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rsrslcdo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ogzbnglk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vcbcqlen.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ripfjfhg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vraqbwcg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3djwxkeae.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3tsihdast.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ypgvbndl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bjuvwenc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kpjpfzmj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ghmxhmnj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dcbqsxsv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tnzctbbn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3frapkcra.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bgammuic.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mgupjree.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rehrcnej.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tjflrpwh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gvpiboxo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ecvuwkyk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vgposyqw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cdcknzgk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mjgzjhku.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3iwbkneel.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3exlzhwxr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jgyaymug.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3svsagcfn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zsnrxslz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvnftndw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3cdkcxrla.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lfshjpkq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmprgtbe.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ygexiewq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fejqoizi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqiyzuze.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbddanje.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3apzocvnp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iutijdgm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3igtmynez.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rrzkplrx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3saagpcwr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3busjemmc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ezztscin.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjwmnmk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3becibamu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aehgctjr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3tvhteyig.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fbfmgffb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vbezurfm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3tcqlmmbp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3grqyydou.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3raozyiiu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3zuisgwqz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mmvenyhi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yqfjjdhd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3itvkhvep.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xaaexzfx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sxskpyrh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tbaebhid.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ipbquuiq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3txdgnfrn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3djhhmirp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tvvmlooa.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rlcnvnnh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ppwtxayq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ilodtpvm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tkqehncm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3eciagktg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bcebmhco.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukockjww.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eznthtdx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nptioypq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fusskwtv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3chbvxzol.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yrjpkbdv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3obxhvshi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cciljzkr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kwccjjor.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3npurktbc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3obsvrpah.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ccjlngjb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cjmrvejf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bhxclbim.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lfelkxkw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpyklcqi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rogiyrps.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sdtzfpjd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tkgvxvhi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3eyacpdpd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bidktcms.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yqoyiuqc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jljpfnbz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3atxlsxwa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rgkypgrl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3emykrrvh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3afmerwyb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ybtjpovf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mgdcxush.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mirkejlf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ojqcqnie.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3erqezxop.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fkqhtkta.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ukiwlasl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmcrvbft.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ayptzore.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3wubsbixa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ukzjllbk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ennmaqcy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyrfuzwa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3flhfbevq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qptflnah.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qmmwbpyd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wlalidfa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mkntoedd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vxtmzcby.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3crdvholo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3znqgtuxj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sbtusbvl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jgxxxgkc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3cqulzrxs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zfejhjlh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3apwklmdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojwjenfm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3opxgxhgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfgilhvq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3opawvofr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3geaiiqff.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uchttkln.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ipwlyomz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xdsmkhdw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yfpzsbzf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ppcjitcy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3slvsznhj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zqcozdcs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3snllmqij.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3golrvuhc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3uwpqhwfd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aismsvkq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bfzqrbqb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ifkadhbj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wscdjxim.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vjwfwywm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xxqrutaq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zxxgrtsi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jazagkzr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwsyfakt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwcwlqaf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuiygdrt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dlhbguej.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3esgghdxy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yduscuof.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3izqhpqdo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3omzadwnn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eikocfwb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuuyjloh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyhagthw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wynsphok.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3plgwzxby.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mhneatyn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xaejtinz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3flifvqnq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hpcnabpy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uzgcjpsl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zpypgjda.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zidsxnpi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixocsecg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dybxetrj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vcwiqcdh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yecqyclp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3spgpywsa.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3sqgfpncu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uvhmoucq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3txmpwsnv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pkojrffd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnlbnwh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3afuxcoys.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mksvzwku.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kzsafzfk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tlttntxr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qollwpkp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pqgdapzw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3maxqvuzq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysagjdae.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ietcyjpp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gbgpfyqi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3inntyoro.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxbuwles.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ylqsfgsn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wqjefhjv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tebcewso.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hudkqmlz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sjebvant.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3anqvdpiz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dhzlkwmy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mjclrned.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gszrwsqz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fktuezkw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gepvmggn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tyhjnwgh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3slwbrdmt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3izunhjjy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdlngshb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wmuvavsj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxxdqfnp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ghevbxqt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuajdlwz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3amaawaxv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ecpzyefd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyobrny.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sodoargr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cbecwoio.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3aduldvkj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uupexbkz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bcaupkfu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgevvmdm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zqwoyndc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bdffubfo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yogvruuk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvfvncgz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqpdekpj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hpvubbus.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jrtwkecg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xgwxpdmt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ioftplaw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjrcrkmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jvlrwpju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3fdzovhxe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hdjgkbvf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zaqcikxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3llqalqlb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3orxtqane.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zpzgwfqs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mdmduvug.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yyvugmhf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nwnwxzxl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iudsrawk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pexexgnj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdeftzif.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pbuhnajx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqfuheg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ytmkcjzb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3grtvheia.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vnhfidxn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3blvhaxci.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kldgdfcy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wpzekcvs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhjuwom.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qnvhnjns.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pifvfgdh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qpbsmicu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dtlxonsu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lxxvjppn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3eqadhtvv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xshndkrd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gysejxwc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xlmsylrx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gttenpgi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbecnsul.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yezzwlnx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cpfdhelr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cjllmrjv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zyrxjiag.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrtsnwhu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hzhdasyg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fbwlclok.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3muheotvl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ampcrujx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3atjushqr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yrbjenlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uydvyjoc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3atygmkpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iusshqso.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmsrqcnd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nmoywmae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovrigdxw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edkfdejy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zutgyzyj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkizxrza.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xtfkbtzq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3znysyssz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jtxdayza.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnyhbgvk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qsknogby.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llvwxjwb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfgthgz.html


<!-- 参考信息 -->