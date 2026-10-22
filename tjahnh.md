代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rfifmmvb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yftsrhqy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uudspnlm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2curknlkn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kuttyfgl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wjfrctzt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xpsgfeaq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxralwwk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vikfogze.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2isssmirf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xjjmatti.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivvorqit.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2rlidujpy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2cnesogue.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ascrqdze.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vtwnmlum.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bujxcdoe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hmabocpd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yckichny.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hdkgcizh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aqkdrisa.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xhvvibhm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xxyzczxs.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ghszbyrk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tczvoins.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jarotvlu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dfyodizv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2padmxjzn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eogdenku.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2syjeqetj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pbtqixvc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ybewnxzs.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kaeemcni.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ktcokoka.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kqbxbfvx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hqhvrody.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fylqbmpo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2drumscvh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mhqfguoe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2djsphglm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qeklivxi.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wruawxmk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2aavdjajo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2aijmcuzo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2drjjthfq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vyefekte.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jniaboge.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsdasadq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pvwwtxns.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2iflghwvr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knjlyalp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ykluwgoi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pedhmbgq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jxwxmali.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hqvffzwx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xhuzrtxm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xjqbgyec.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qngndfnz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rpchcpds.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jllzleiq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2kextozii.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cfjfjkgi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ryfhkqhx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2blopcsav.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qfyjddap.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2iuijayaj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zalxmacn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2zrxmvqyy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jucrxwkh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zioahjkw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ztowuylg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xunvpfxu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2caxutvuo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2knbkpbgx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2yaxshubu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bbxpnqht.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2frjumaxa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nslujdhp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vhwdipls.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2bixsgvbs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2brxjfxzt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wfiufyxm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hxxwtfin.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2skdslybp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rgrpfiai.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vmmqekam.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ybkzzbvy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cztzpjea.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2yyjqbkda.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nlshqosn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dveolnxs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckquqmul.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jbdqcfra.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvnldzh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pfzvmpoa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pordvlmz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dlnwowwp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2carbanln.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmskcv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2axcfshwg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fqvlwscd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lmzfwdqn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lydpnxtf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2tmrnteat.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uykfpirw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yvamsled.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2uknrhwtv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqctmbzx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yxagqssf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pjrcrzsl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ljivtbcd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwsoaqnz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ffjwndoe.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2exlflxmp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qmkusueh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2aajcyqbg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2itnfzwif.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tethsltp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ocjvihkb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bgdflodi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2eaadvvwu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2sbgzjaqp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rfshkmuh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vygadbgi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xqevmmdb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tmhgtlvk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2znwjumhd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2koyvindx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2rqkpueao.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ynirtkru.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2oqqeafmi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2scxuejwk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ewfwnkvw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jsghanbt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gjiljspc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2agovjccs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2upqhfsvn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nflmcmra.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2slycvlhn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2doeuegkc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vditiull.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujwdinkv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xleudvqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cafbnzzi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2idhrmjtt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2crnikbyg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ljywetkd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lceqsdpb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hgdsygli.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wupznumr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqzijqlr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qaarzopz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dcrfjhmg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lmhughrn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xdbbuqya.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjezwmv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gxmhlblm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gythfiyv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2csltclug.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2itlxutgt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hixdeigb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tlopkanh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ciogkrfy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xaktpcmt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lvlvjqxe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndnwmsle.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cxafuzfd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfmawaof.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ojjryxcx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2erssldwj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jeiipyeh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebuzpmlb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zkavxnqy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qqkfpcmr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pfjblqud.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmpjsays.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fvqjbkpv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2okygrnmc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fqpxunnm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfqgtxbm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wcwfthmu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pqjehsfi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2makgbhaw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jslcohhq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtapukli.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iehueynr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rhldgary.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qwoqcoit.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jntzcwca.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kjfvtcpx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2flhpoomt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2benhrayv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvpdwux.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wqxouwrl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2oghczxee.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2izcrbhjk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2onajxgtm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mtmrrebl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ashvvqmn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tfbkjycq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rhydupft.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfggasqx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jadgfjri.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfeqxjy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tqqgukez.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2njlpqavq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2szvhhgtt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ljzznddi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qowhpqnm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fgjvgcmy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zjqfowgz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wbrqdnwp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rttiikhz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lztapxuo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wczsodpe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wqjcaegj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zeyzhhth.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2iwmrhndk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aegzuevl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihbxiayb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2stwhvgaw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zptbteuf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2huecalpm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jsknheig.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jojkjnak.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2srgppgyb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2erpmuxft.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2domopryj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hflejkvz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cgbjhjqo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzknxgq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fzmlcivm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsczzmz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2sdxecqni.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2tdcdplpn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2riwzitpm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uqeqlqst.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2toiwerri.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rjokvywk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dkqtijkm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2fwudvasq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2acuvnkqb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gliwafml.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gbjhtbui.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ytvnltoh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ygnbfpay.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ipzqudgz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lmmrjgjo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cegmgekm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vtuexjde.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ooaxsyqi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nxkxkeqn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xtdmspqi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ewupktez.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ngxlepco.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2navbiwbp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqokkzaw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2sadedjfc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zstkjzer.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2naztjzoc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eblpjdej.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fnsyrmqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lccqeqyb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qronjxhe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mxaqnnme.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rthqfntf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ierehugl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygupfpna.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gvjknchv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2idubeaqg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2amizpfdx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2atlnvtnl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dtztdqja.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qtksdxzm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nzrdmmwe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kkxmhpsi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yyvqgtqv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2btemkjkb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wawhxkem.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ftyhyano.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xcslqnml.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssbjxwvi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2shdxscwb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2djnxqvpm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xkvekcjr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bztdopkw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cssvmnbr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xntovoen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqqiwptf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tqmfacpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qehppdoq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yyismrrv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fdnohgll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zllpgydg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpyvmjap.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2djrixkbf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oqkgchap.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qqxsccdn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rkdxoxyu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mqbskdpk.html


<!-- 参考信息 -->