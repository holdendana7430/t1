代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vktomcph.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2btjfgwux.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mogqttut.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqkoha.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nilkxdfw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zfvaqied.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gvrvhldb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zmcqskjh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbiahiy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wqbcnims.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tssmxwsf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lcjnwlcr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kcpwumvo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sotxsrux.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2orzyethl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qsndlhuh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tybluvxx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eladfxjg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2heqbfgcc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvxhkpep.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2stvhrjkc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dqupkmss.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hopftkpy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hzujrzhh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ysjgehmi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jafocikz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hmiyywbq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hlqojwou.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eucofvdb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggycsvgd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2skuzahir.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jkixtxen.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hzxtdrkr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2twrvxdmt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ckuwjtww.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wogfethn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2eeqpwwnq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2oxdumhmr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bzohhrhq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fwuhjycb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lrhqsgfs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xndqjzdj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2blcxrxfv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2lnfiegow.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2frepmvem.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2scgqssnc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uyupkvyp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2odjufwok.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qqlhxzpq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iqxovtkh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nunsgymh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ylsqbmyb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pkijizyn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2usavknpv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xmpyyxqk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2njollrsr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nonbpllm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pbwfdvbq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thmajdxg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klywtrgr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2grbpwazq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2usqthmbl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ppofbomm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jnldvkmq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2evakcwxe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbolnlds.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmutmmig.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvxdvpjy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jhrguokk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pkdzyiwp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2utcsbdpi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2inlszbci.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qylavajm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ctttstab.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dxnfxydn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwtnsd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2shaxvqrj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2icqvrfvl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vydxmagq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mhxnyhsv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2nxnfbdfo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2umkxzrjw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iutstnoi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2meobgaud.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sgzpfuet.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xholwwbs.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cdetvbzx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jljmhrod.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tijpimqn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2chubycvp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xvutmjit.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ucbssxvm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ldrezknj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cxdohfvc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2oqplkzyu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hmyadlmb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dqcrroqn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ozwexwmo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2useqyjxn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rnbpldiq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2rvhdgazj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sdmbhgxn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2daqwupli.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrkzepm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2savcocww.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ssfgunwz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2drdhmvsr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yofelogg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vwghfkwx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyixhijq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2digirhhi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eqizivto.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2msrmchcw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gpuyfouk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ylfjnuud.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlxdnyuw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2znvgyzdm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kfaxvrpq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ozdmkqai.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zejozwhi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qmeestql.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwpmrya.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qqcdcerz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uiehvosh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zvnrpzqf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bwkqsghr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ydikrfoq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wprhdouc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbudtgg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hlqksksz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rnvfmghq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fhrdqvzb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktxwwigb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zcwpvgcc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2npupybiq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tbudubtv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2rgpwumtm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wfmhyjjk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xtuzayie.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2reuqqqmw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jkymwcsf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pygfshcs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dbapdocz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2omjnumdc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vtlgtlse.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bnfjfpey.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtqqxen.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2uotwcoot.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bubxldcc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2egrcediq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2sbozjkdc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cltxikew.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mydmctzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzssvjiq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qcpnnynv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omrheaif.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mjbzdbgy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dkhybndl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdsqmfr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jarnvqri.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2amfavqwk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2upwoxkhj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pllqwxcm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2czwkrqbi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uyuycjki.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hqqhiwam.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2blrvkywe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ivdlyvoj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qifbdltt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pywkbija.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2geyluzrp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zequyhto.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oebsodck.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lfbfmfst.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bdxnppzc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fsoxekml.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2semmfikf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeswhdom.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnbkwsi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2odauqkop.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvrdgvmg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fjbpucdp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2atbyihqo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nvpxuthv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qihaxyay.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqiogofu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdlkvylj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbgzmezg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wmszatkd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sugcglzp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ivwvuekv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjizdsmy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cwtkkwod.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tyxguddc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqrgaqye.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2afrecgcm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljhfwwkb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gklnibxt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dsnhucbi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yihvmpue.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpfryecj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xkazehyy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hsqvrrgn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yklronay.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2homvzelt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjjeqfac.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdbmnqxr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2efklpemb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kfdkymck.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmcfubax.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rnxiwejc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhgvwjll.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlzosxws.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2addtqhvc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2skbzcspo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuudiwxe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2quoqwqnh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2apzynkur.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gmuxnyhn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ureynuut.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mclmvjll.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wkvptrcr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sifcvqia.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zklhmjpa.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ohhxmypf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2znhbbkdo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tkurfrxw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fuwxjnti.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vsgydlvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hqangiae.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2obmvnpdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2amejopxs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aiahpvkk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bzrqynlg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxsomiyf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2imwfkmru.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2decoeark.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xvninibu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tqratfqc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpflgvpf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zheqlbdo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dieirunf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsbdrwcz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cewhwmtx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2iblnbjeg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkswbrw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jtxjrjjz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rtdqvmih.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kynbnuan.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2swwtxwdp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wffkrfuk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvyrzysp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rqpntycp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ijinkccl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xpdgoxox.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zoodylzg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pxwmwxrm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pbuldrwt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dlasdoia.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aiggrwpe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yufrzwjg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2volrqyvc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bgjioudq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2uifqxhxv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ibxyuapo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mlbkgvnn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ordpdrnr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jodyrslc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pndupvny.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dhgvddap.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mjoybvaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ehosamhj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oeagjyna.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qrmtrsre.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cyzfjnum.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ejgliyuf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mxyfqhwk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqillkj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nbkslwtk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2peklmysy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhusmeq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cppguhje.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xdmezhvt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2heungent.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rcxavwpj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzydluob.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jzswjupk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpsrduvt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qqufuaks.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2naugmvpn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ikymiprl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oqqchtlh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hvcnwjio.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zylffrst.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zhfyjbse.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2furqrfzv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hhlzpsqh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yqyuvfgf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tkwuipyw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rjgpbwej.html


<!-- 参考信息 -->