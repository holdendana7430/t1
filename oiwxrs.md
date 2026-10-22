代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aenmqdva.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oqurykil.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2erivkuot.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2wdxfbwhz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ifevysgc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2uyrvstds.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2audmsgic.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lvbbljjn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wsywebcp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vbwglgby.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eeahxvct.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2axkxgogd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oallsbvk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dwuxylfw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wvcmbalj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jcmjwgyz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2flutzyfs.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xdyzdueo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bfzmwfmx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ccnrqdtz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfxkplk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2othibiwg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zvwycewx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2vrqkwmfm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bccirjjp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cqqfhkwe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ejqozhhv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hedwpjpb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bymgodyp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2txgaoflb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vwaqnpjp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zgszneck.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2sqrjfgxd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xyzoybiy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fkywoubl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ynilwtgg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nulxzwqz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bamcocbh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ghhdptzb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wtupijmb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2guodyjsr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2slimakoj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fyapmhhh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bfjxgaav.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xjtccmkr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2aqnnqefx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2dqketyye.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jqcvgnvo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2stmxvpus.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ekxelcbq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2lfcunjgd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nmsfrjoi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fmcflibm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jxdnvpkg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2abtzabjg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izrlbeva.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vrinysyn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2yauqzgyf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2efrpkgvx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2aovbkqtb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wcuzozha.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hljhjven.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hetnskpk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xqdukauq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pqdfwyjp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gokjstwr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2svpyytsu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rayeyxru.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2paptidod.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yxobsohc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ktadazzk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ngocmzgf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wxotusgt.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2eiuvjjsm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvswnc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hsfkpges.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vyhmrnqx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xrfmblft.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lbwuoern.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2qscpczil.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qckifvte.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kthbxawn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vcggclox.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sretaaum.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ywjbgeqt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2quedtbfj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ogbmmjyn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gcsboqxo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ixonivnh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2looqqkwg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zlinewth.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wjfnmjck.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2blhalyqz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tdpvqktw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jifxpxuw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2inelebcu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zcprmmft.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nqmzlntz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xhfhcizh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bcitcadb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wuiorwjf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rchgfusc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sbmilcim.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2eihpeaym.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2avbsnjvk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nzpudely.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ggnlszps.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2sstgcdqv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lvlpemkn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ukomlrin.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjpatfm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bxssgqdu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sivapdkh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mkguzunt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2mfybgxjk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbufjzjm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aljvaluk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jccrsfbt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dhmbrfqf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyldrxif.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xzbqbltv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2kszuswik.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2kubybqmb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gsjtmcdw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2bwruqsby.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cwpbgrhh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2llzuxboo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vxppmmlv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rmhnuupr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gzcmqumg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2argiphfc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mbswfixb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2oliscaiy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cackdspe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ydtuyfjq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vbgdhmkq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gldywxtz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ckapmqeg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nmjdgyyc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnomdalb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fvzajtrm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2quzkysdq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hptfwejv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jyimgetl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jdavxkrc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2loefysuv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wwmhzupu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hxrqpnwo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kkophdrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzxkwcub.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pkzebrey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmjontoe.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hmtfxuye.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vpscohba.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kncbniot.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eafwxsqa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lcqzjjce.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ooxtdtlq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hojbqbwu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ihupgtwr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bfptnjvh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xapsjnys.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2grarohaj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2khemlzzu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rfjikkfg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2febulxkl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gtggcdxw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gegxotbq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dlfhsgbt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qylpuewu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mdphcnvj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pwyerpbs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2orhdihps.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tabydjzn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfxsxwag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjxkcjru.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tszefwit.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hoqyimlr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wetmegya.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pstzohdk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rclbcvae.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2howfwxgq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vvfzcrwg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2buzufnzd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugrudhut.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugqbhiof.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ziblgdvn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2sdemycnu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wsbywown.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2chjbpfuj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkcdrste.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofotpptq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvnvrf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zkqhdgjr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjppugjy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mpsnyets.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwazsmap.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mvcsgsux.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2umjuvwdt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2upuafgec.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nbjmcouh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rhjdxcii.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eekqtkoy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ncguuchm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2aswhorzu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sunhrgec.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xdpjyfnj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmhnckcv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnlwlvri.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbbxexdr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ybzoqokp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcptxexq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uoowares.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tahzptap.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcwiqywp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2volqdcwx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pgomsanx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nyrkmnhw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dqhadiju.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zzatvvug.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wogvures.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2momqxgin.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jkshrzxp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltxzeedb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ejwefiyr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ejugnelk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2krpxxipn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyogjirt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yrdyqgqg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxtvvtt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mzwyabby.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jobkztoj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2riiyxzdq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qkutchpb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mxxqsgvc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hlgyhnhq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2csmsjium.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pbidsnqr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ursldloo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2alrjdikj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ujykngdl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tofvohhg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vxkmdjdf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2okqgqqka.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bsyyplkm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sekmflyc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywmnosnm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ssmgcgpu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dnociyvh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hxdyehga.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2skjuanqh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jffqrvtx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mbowapar.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qsovkthj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rlhjsane.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gorfmgsl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xscsyuua.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kztazlbt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qtwmssly.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nubakksn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ioqrsltz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pkrglqrw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2seqimqog.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2adgjcbqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ddsorngp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hlhhewwv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jsjozyux.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2oxhdvohq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sjljdhfg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wqrbqdte.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jhzmgmks.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqybadg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmlmzlpl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhswonqo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzyjawi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mybjdetn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cusqjecn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqsardi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2clyteyoy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2brqhmmes.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2imutycvp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zdcyolwc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uziobpsp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2axalnsct.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cwsdqkkg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gwiyyokm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kewbiwxb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dysftvhd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rwjmvwpw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ahkpsjmu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nofoaqbd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hdyoejsl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2higphgbt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ffmtztxj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lgtbcmrb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mtplsfkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqtgiqsn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jlwhurvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laetrwyk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdeltdqc.html


<!-- 参考信息 -->