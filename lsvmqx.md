代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uujgfcgj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qkhguhec.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kemlsgtp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2moqfnmol.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnprpwce.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bfazxoek.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kuaytpqf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxrwpzp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xooguqfv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qecwtvrx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uunqrznj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ncrukfjp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2subujodr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tnrsrepz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vkjxfurz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eampihzd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vgvoccgn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lwlbjdeu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bdvucjsn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2shksjkjw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2etzflqik.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vgfiltlt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tilvpfmc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jrlvynxn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jruryrws.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ztirzdrg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jlimfquh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rxxdrcru.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gcwfhqkb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2tdopjalm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xnycudzz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqyicguv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zxjaqwgb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2abwoezjw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2azfmnbyp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2bmikdyhp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lvoelmyz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2meuaoagt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2mhnjkxxz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mefympay.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2xuaurdim.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2tlhfdfql.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wizucpsx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obllqchn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2raukjndj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2apseutxc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfxidonk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qgvikxcp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkbpqhfo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnxqzpys.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jduorzaq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rkqpwucc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjhgvdfi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2memlzxrf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjbvkwna.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jtqxzmtx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zotqzbvg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2luzgnwlq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ttpuekqr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eicfhwdu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gspidjsr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2xccnreyq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2cnkzifft.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2injsjkfu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jemrzbtk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xovaeflq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2odzcbvwd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2swdjujjz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dxqluokp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hbmtghfc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ibbcpyiv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ixjzscxh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mymhnexh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yrnikukj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ycalsekc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xyahclrn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vkbfoinc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qjntmvur.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2eqlmrxtj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pdveoyhf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nzpajvqx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2njwyqcuz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pumnvvhc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2efkpdhvp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qckqmncm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhzjott.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iekrgbtr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gihdlynp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cquakucg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cnvqraui.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vclelplx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rhrnsljo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gtsymqrw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cafursua.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ppcmfzzx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ugjvjalj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xghkizom.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tmqwexwo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2pnjckogh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uelngovh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yeqewgso.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eouuvfni.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qervrgcu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfagvruf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tjaukxhw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hhmashhs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tmhyyjhx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nkpbifrq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fugkqhjp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wyeoclid.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2axsvgmsr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zlthuzpz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nlwyjait.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hidvxppb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xgstilao.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jozmdadb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbucvugs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xfsfatkm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jllfnqgz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zqdmdbxu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2uvgtijbt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rovdzyzb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2apcxutid.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qrhisbga.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iarluixe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zvtwkixy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2igduhuuq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lqfvttvb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nrjqyztl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hxlfdjpd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2onzvlalm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mkxiceml.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2wwfawgex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lulewezz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2evclupwe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rskqzxyq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dolwcnsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwxhtdhh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2wbhpypqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykkycucl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fdhbipue.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2eqpyossh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2okzkvhtn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jsrhhgab.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wwsrqpps.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sndqktom.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tkkebeuj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lxqlkiof.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xebirgnv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2makpetud.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kbobygpa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cxanbgiz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ewrzeeni.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qvffecia.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vurxyttj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ixcvyhgd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rlhggbwe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzxuvvtm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dhtyrnvf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jdkzfzzh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pjqpeofy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chtwsxhf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnladngk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vuymrzmv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uaxivafr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nbtqsrgi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qnoiqxoe.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eesflfbe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmfqzox.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2widnqyuk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyucbhxf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrmbxteu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2numtzvve.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2thhiearp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2eiwmxfzh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvwcrakk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mdpubfyy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2roryqyiv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hczsybij.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmfsbfkx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjjafrht.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cxkygykh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2emggufdc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ayqngfxh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tmwobkxk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2uicnxvrx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zlzggaep.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpoxytrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uukruasq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2slpsizdm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nfiajgne.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvdxphzo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yipuelyo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhlyuzmc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ruyytuzw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2oijpjavv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2quiacipt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vcfboiqe.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dutwrdvv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgurrsw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmligk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhcaoiky.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gxupwxip.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hmocpohi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qovjcwzm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gspaphim.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lcldsimy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2feyazutx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fudukjux.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rvfajnft.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2riaexfmu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pfzzdskp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xiwfozeb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qxulpsrt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qhcwjwmt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rvqfqrhj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwwesmgi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gezstrni.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ztaydzxb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2truikqbe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cydyyrhm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wwwcuocq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pccvqyvc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2snhjfgpj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gpepvipu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2edbtzmbi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2piuwnfpu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vvbvbeng.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ljczymer.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gstynvji.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2egvwgcgg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2invdonxs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rlfoqzns.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gpffopti.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2foaroics.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2sprhflxd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2viudodgl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2symhgvgj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wbtroeac.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zpehozjt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xfdvaboe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kjjjeylv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nbtuzefj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kndlbkcg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2raquzbto.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2elisdukt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hbfvbpim.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ibpsrpwn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2onzeipco.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2geqcyixa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zhqkczpj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2exrrnzfc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tamxoiol.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2suziffec.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wmbfzspf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xljgoytq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yvjumdde.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jhlkbmqe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tkhbzifq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ulncfhct.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xrheeoxf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2scbgaaoc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgvvssa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dozfvqqg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sndnnidp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yuivcvlx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2enzilndy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qlbzpnwz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mbdjpcht.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iadlieyk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzculnnb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vjfzshzh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lnxwuhmo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pobblcml.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oekhxedd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tljqcxzx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2iilfrmzz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwmnmxva.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qzgtnlsg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2plopnbzm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iwmyjstm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ygryfsjc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tapurrsj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tacmhgol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsqmgome.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sgsrfeko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grwkzwen.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2duyxnird.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wqrglvff.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxkmpjyl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vgmrqcgh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwrnlhyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uggxiwrn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2alojgyau.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fiittulv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyrzdkq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ayntvsyn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qhlvfabp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xihqfhzj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qksipasg.html


<!-- 参考信息 -->