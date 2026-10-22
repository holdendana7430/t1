代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bqoukdsj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kktueysy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qossrsec.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2bjtbhivc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hwlipurb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ogauegwg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bjopypeh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2daajbzjw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzpfbdc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kowlifcx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wokewlmv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2huufbkba.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2oizfyfez.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2myjggiio.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rtkpuzwa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ycaaapvw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vjkrblhg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jyulfveh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fkyxgtqq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ihrwfkru.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vfwvtbcc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2snomiebj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ejuxpbja.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ckyfjjsr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fjbcpzii.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2xemzbmwy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sgkipucp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dxljaubq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dlphbjbq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qslstvdv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dkennarg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wlhgswae.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zwqzupua.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mdmsxbqz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vfqhsydi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hojypxap.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dsjorsir.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ceetuyec.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2eqayuqbz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2aqlsltdi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vdpbiqvm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ztantpto.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qprsedpf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wjwuginj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2beppitrl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2flhyjynq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2nlozbvaw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnirsbqx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2qvupxxfx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pzrbstop.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dyegqmqc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2mvobpxyi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2offmbexs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbllrzrn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zhvokslj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vircvwng.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zmmizbhs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2amqyxmqa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2utcwamkg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2puloaoli.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2pchtqccq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fvkjrknh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ezkrpscv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aaafecyo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rcsasgnv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hyerblzi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kyxjrmsr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2erylzrws.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2krnnntfc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2utlafxtc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2laeguizl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ouooeosw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mrbutlwz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zuqbrdbp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lxvovtmd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xdlssktn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ntjsqfaz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qqssytlk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mawhcjmc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2oaynsczy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2nwqmlvzd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qhwwxuzy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2woixlzam.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2kwktbamd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bkppztzx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wolnnyju.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2axisaqkt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cdowqagc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggjlqusw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ejgfwrrr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqoxrai.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjrjmfj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tinsfkmj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uxjdiapq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yvuxydxa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2klxkvgwp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zpprvany.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gdzgarwq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2yoyzizpm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tyfdvuem.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzexdz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ikusatga.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hemglypg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ntgzomnx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ugsmbspj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2okfxggwq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jijocaqd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxowayi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2crzuddht.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pvbrrkkp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tvfxamvf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jpzkgtoi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2skweiyud.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ljnsulhl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ijpuybxw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2taiejxgc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2uydxffsb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jrhozzkr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2glckorzq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2llgaccck.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2tptqvsuh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xzglisie.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwtjbawh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ruvraenu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jnnawbcg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvshdlim.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mybwbydk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rpbanlev.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gcthkzvg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wwbwxynt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ijgpqtpv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vjjpvxyu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qabnfwlw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2bqncluou.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ugrphgew.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mtnrczwq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2myptzdjs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2spdvcnrd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wgjezwqx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sbrslwdg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hpsgxoix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvqkvjzx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fopvnfxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whdlgtiv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mtympajz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ozoyixcq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shxahbwn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oldxvgty.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oqwwinxv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kdihaebo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2lfragyih.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2umsrpgxz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mfbqsahi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tlwxlsap.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mytyctkm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vspncvph.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bwfnmxbi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2knaqosoo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2scoqgola.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2iwfzqxgz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qzbgofkb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qhyurqdd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wexhyfaa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2otowhbzn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xlmsvhsf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2olzhfknv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irensldb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gaaabgzp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2soaxibxb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ldsoeztf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tnccqmiq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xuvgatbw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ytkyqgaw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hluszwvk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2twajumik.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xpyiucsr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnvezhmd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ebqironi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vqifvnmu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2szzgqlig.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nhwjfxhw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vzikeobr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vfgdhngr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2suoxuuoz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xdxgsjex.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lrkbenmz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ejvhluli.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2oafrtbdt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fmlqatfy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tmxhbqcv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oimsraeg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hxufuwgu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2flvqvwew.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxbfbqhc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yggcqtyd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fcpakepp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xglwgmwy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tworchqm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2reomtsgt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ifqdyjbl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vgyibnvj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyiqlhdf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvceubgc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2illtudaz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lwbjktip.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqvxrahf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mdclnmvs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rkcthwrm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ldzdrdlr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iycnfkfl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qcclwlur.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ermlskco.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ywrbsqsm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbcsodu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2honkeiqu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rfmtlxdz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ebisrypr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2iiwsqwqb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bolnzhui.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlzkwro.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzglrtke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vchzridh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tljaoiuy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wqpxmamr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqtrjsgp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bghsdbpp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dhnyvuui.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kinjzndj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jzujuiao.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2udgtycob.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtxcfurr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2djbhlnjt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2owyryeqf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2yxkhzivl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ctusvipo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dbynzkqr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rqljdjnl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdllxwmu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tlcrmmgy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zclpvsip.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nlqcuxib.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tkglwrrh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pxjqsdsq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dlcerkvq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2icdjyvts.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zolyokaw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfiqbes.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qecqcyuj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ylpoogjk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xzmzlfvn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vccbjzoi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dnqyuwes.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hwkyozay.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yipqqvuq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rxftotlw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpboyvq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtovzfzd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vcpsiajx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2touxryzp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vgzaaxsd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2isicdgts.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rsjqssnh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2naeysggr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ablcuqal.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnmdwjo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tgezehbh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jvaqkfbg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2siruchpd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvgbgyrp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yxbblznb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2preppktb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hjuakppr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2olepgmgm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xwtiagom.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jgqddcfg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tsniqyzn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2malbahle.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mxkhqyky.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bysvbbtm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jbyyyfmh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zrtxmfgv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qsqtjcuu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ssfktekp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dzxsokkw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lqpgoajo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jxghyyll.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2eiwpbvkt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ktzvaxqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhqjktyx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2czsnfjbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpdgkmvg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sslvuaqj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rjgmqhee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nphesrqr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jvagftyh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jepoxylc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvlyapbv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fmnjvpnj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwuabrtw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2axvhugrx.html


<!-- 参考信息 -->