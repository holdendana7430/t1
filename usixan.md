代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3udqcefer.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zdtgxcjp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mhqrgtzx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3gflxzdxp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tegcqqxh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sgqnwrdn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nuowdswx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3pwlasgqz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuhvima.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pbirueew.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3katxtiev.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3cdvkxrsk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bgpflavv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wdyzelqx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qlkcbwoi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3fjsqoogb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3igxeedrl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mqjexosy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hrntzbnm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xbvazusr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3shxwuvpf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tgedziuv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gaitnrlm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iycfjyls.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wcmpxest.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3wvjgholu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pmrgldin.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kbmsnlat.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3awzxwfxv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bnqpnwqy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vslegzbb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nspeiomz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yutqxhwe.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3abuzjiko.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3txnlinbb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kwhyimvo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ngegrxhk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ssvraqym.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jrgbibhm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlgfmzwj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cnwtkfnu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dxwidddt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3pquouxvd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oeydxijv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ucwuqwnv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3oazysxnv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kmssqzbi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3daghvvqn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rckcuwsm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3czdyhknk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vxmjdopu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3glywzevk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fcxfxvns.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpwolsfx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjuzojaj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kyuiytbz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zoxcsnbt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gcysvmrj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3usnimdmq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3llvretdd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ratkcnjt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ydtsmdin.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oovzyqzs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jxlaspro.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3spqeirip.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vhgsywhj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ztmzhzqg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mqbnapqs.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3rjleitwh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vxyyufjv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ukmqucao.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tgkcmkas.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3khhntzgl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xhvpllby.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3csxcmran.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mbhduhso.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oaazsufm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3phpqgbqo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ihsifvoi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ztpequwn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wpuxjgsy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3odwdgxaq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ltsbdppt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3efwqkfil.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ezpghgam.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qfwhlhcw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3umxpdhit.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3clghnfah.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3sgmroxoc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sldpofox.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkuhxeyg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3owoufrin.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3asutieyp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vztcivts.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rfnunqwz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3eicmnzek.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyberhjl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kpkrbriz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3amtetxys.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3gqofuqmk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zesxagry.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qusvgttq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvyjfjx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3uvmiknyp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3afdkxhyz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tvdlcdgz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3lvixidkd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftyyvmha.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3alfsetsc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wkuqatsa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xqpeiodi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fidjkpno.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ixrlqfso.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rjdrirme.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vjscrfkr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3chpbdyba.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3efhuaefe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qshnlfvj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qwnvwtrr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nemdyrob.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wfwgjvdq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lljzkjvo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wzhgrplp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zhjaajym.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qbpsnxuq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3mnfdxsng.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3elpksgqn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dnrtavbu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3oquilsju.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qsmkkuxr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mhhwveis.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xayvrlfp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ntfljogw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vwodmvly.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3oujsqxzz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3wgmagkmp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xlvwneot.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dmjbqkfu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mwvbismg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tikdqbqv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqlgygj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcrrmrcy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wjrbqjoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwztlvnl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gizesybl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kfkunibr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gahursbk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sjazkvvg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zutpnbpd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nxcdlxsh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3pybnmvpj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gznymdbq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pyvgnhkd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lqiqnepf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bpwdunmm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwfnrnsp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xhzparsf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3clnswsiu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gjofimxh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3eaejtnod.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jxlckokw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sirsmcol.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pzvsiiey.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qiwxbhkd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wbcyvgdk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcjbdprf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvojuuhx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3waibqeus.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kzktnzay.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yqcethql.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lbpyuinf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3elzsnkad.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsrrrha.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylegrusw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3emsgqpni.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kbbngdqh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3krugrvwo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3uzpsjelw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3enbpmuyo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3txodzram.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xmnwwukw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nikbmpku.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bphcootv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdidjzsl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mbimixzx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehokhlin.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aiavgnpn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ekrfsvbt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3snfoxdmq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lipfotfr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bsstftli.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umnuszuy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gofwaywy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kshtbqme.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zeovsuro.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3oninzjcf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3puxqpfda.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mfblrhap.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqwyetna.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkwknzcu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zkjsdwme.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3edmrlcor.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fllfpiln.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3npihfjdg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vyjwlmbc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kwppljjv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fmseoups.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xqiqybea.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uagdciie.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hkshpkyl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3obkfknzz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fupxniyc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zslqfkbi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qrdngzjk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qwklkhqv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hqccsfay.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mbsyjmop.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3seuzlckb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zwxbkmvv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgtmjjvq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmpveuq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oeemxyuf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zofgubje.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmmdqgj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vhmjymih.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3albcblfn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yrhmrnrw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivhtywgh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3elraelcw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tgiiokyl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kxfdnlem.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mvtvzlul.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3suxnjkqy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqoxydlh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ilgipmai.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3vitejxpz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3utsbkklk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pspxssey.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkaqqtbd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qxjdbqga.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3sckeillk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zixjelfp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3emuiukcb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dsfpznfe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rmavyghc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqfqvvlg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vycknpuv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pwlwofcv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oitirmgm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugvllbxu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jpkwrdmi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3npsltvbv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3cvjcqnqq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3usgeosul.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lztndbws.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jbxowtxn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iyjbjmtl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ldedykxe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ivgfqcia.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jerhiglm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3znoruhim.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hnbqyggg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3actytulz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sxqbshqr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xyjeopxt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddftibjw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3logfvawg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhumwzhi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tcgjaske.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wogmrybi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wxjgdzme.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fgkhrmcm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zbbvxvfb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qagqkced.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tiwafayc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vjslzpxc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aeduyrjq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3avlfancj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pylsehur.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lukbcche.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bnlhoklv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mkukvxcp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hngafqkv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xrnxgpil.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iqliftjv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jlrigskj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ksqqjnkg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rgdbaxzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqapsces.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3artacbtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqmyjmet.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jbfpgcmq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3utsdocyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvswdnfn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wguabygb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiapdhkm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utytjynk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ryzuowkc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mflwuzxs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tjzkwlyy.html


<!-- 参考信息 -->