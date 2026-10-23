代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yetwadbc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fvlpahei.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vbziqvpk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmmxgtoy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqyhaxwn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzphhujf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ggmdumdl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wllcdpzx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ozugwrjo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ruuckqeg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wuygziff.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pjalrjtr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dqhvrizb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jcqyqkbl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hqnfyqpi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zgadrqhp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ekqeqyry.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gluralbo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kndjtxby.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dssvtjsj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtbfbla.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3whxxvihh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qqubaaag.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vilpvekq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3iqqbwwyw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ubxgvofe.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3eguhnusp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hsyarswl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kmbuacxi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ihfznxoe.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zhzfijic.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lqnhbnsq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qlgulrxv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vwxwwhjc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3upwuilhv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mhvlvmvk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3voyfblbz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3idtlujvo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3paoxlwbd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fmpzhnrd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dakjpatl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3nmrwbvbn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jplhrxih.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nykjrnel.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3evgxcepc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tieekvsq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pbgvzmjm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eeedgclv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ucfqevqa.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vukkkgew.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cdkezcrx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fpzekepz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uycshqby.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3aetomuqf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3jhxajicd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3giashxiu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3djpgsbkt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3sfxvluvv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmbvhbva.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odmhopze.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3uhkftrlu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqusyb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkfykffr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3whhrwhka.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bcjvjloh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bcszxsev.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnqvkfzi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eppamppo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mbrwklrq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixcjcrjg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3obfqnvnd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3osvczpau.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nicizfcg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gkzxvsyi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vdpdhnub.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxykgqf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lztogepp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zzawsogg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ndhxnpcf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ielvoolj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cexxrxka.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mkosdbas.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ewnetpfd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3cendimle.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hzvmpsjx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yhusticw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dhxgfale.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3unqnpfxy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3durthhks.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3caayyxiu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qlesoibd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jatympds.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3uokymjet.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xrpfhkvr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vaizyjcf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kllzbxee.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ndckavge.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rynyrucr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3agdvbyaa.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fnxiysxb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3oapzxjxc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mtiozpwy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3whdjxfdt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fisbefox.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xzfyjxbc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tkrehxjr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sjyipbgm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3mkmmrarb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ufijvgtc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbozwlr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3cievdaoj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jfjxyald.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gkafqqqk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lojwmsgk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmyoalix.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3omqptkvp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ccyqnbhi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mrdiispo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ammbxwse.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwyflcj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lraqdrax.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wfqummmi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3myceocot.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qqxlufyb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fljhlxsj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3htezvizk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3srbnesqd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3bdrtfgtf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dytkuqjz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cjxfaexk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wcptzbrp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3znwcetct.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3oyqsfgwd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3cfxxocsx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lcdxpffn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qdhksvom.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3npsbnxyn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3emqrllom.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3axrfxyrb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vbsqcpff.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ftrfjpza.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbatnexj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3imzyqzbq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oboepuru.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oslpbrgk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3lnowtahf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3euurlfki.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gkrkgmsb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wjzblmcb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3njfrevxw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yaratdyl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vworopui.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3utdiuzou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgrsxmzt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jgyylffv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfucicdb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3odgejupo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3nwlhosyz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iebrnovs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ppqgbjva.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pjnelggd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mdbvnhsj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3uczbtbff.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ucrotqrx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nhtbaily.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fuhkpnca.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3znoncyxs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mjxdlkhv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ovpaaqpd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3djfpajpv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qnufpthn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3piobtbdw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3eyvkpxks.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fowjpcrc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yphmlkxr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pqtshuhl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abzhengx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3auuwurne.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fartezep.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqbtewoa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovhjwqqb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mwynvbgr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xszwsffs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cqidhqhg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sguapkzv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jpidqrws.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oerwajsc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oemffsci.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsezzbhx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tlcvapcp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jvudrhea.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnxfuyad.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pdrvwpmc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3phgszgnv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rlmljnaa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpqaxrs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3noaugokf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qclmoxpo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rkipticp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fqqalrkh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgftiyl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qopaepfs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pkhizypc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xdkdfhfw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ulllagyy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yjgyfjqu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3oqmohsxb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3igzdyabr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wvimhfgm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3aaikjqbb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxeqquel.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3veoqfsun.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tpjtncvd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3irabbzqf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3frdzozbv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bkguuxri.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3twvcgque.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvicdyod.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3awwrybyt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bvqasfxi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cupkmxtt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3abgvldby.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jshuupwu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zpoueanr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpuzlanm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nzhwhhqq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hfigcanv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3axjmuuox.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pnhznarg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ayhoqarf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sgseoeqd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nmefnmsi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhdeeupu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hqwjfjpi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jmcmpwgq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pibivbul.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3visgwyfq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3pvrnvkfv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3exvqmisf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bfbxukmm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3esxsrldf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gltmwejh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3babgvutm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmizcbmn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kkywxfev.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgucnrue.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fmuwtncs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3aftutzih.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tzwbqzxk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3smxfxzie.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uttmdkxn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aceajzit.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xybigqqn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jrrpseka.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wckmbbnm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qffofdii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nsklcwkj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3irtvtvev.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jnfcehks.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qwynjbnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aqfoitqi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ckktaeyl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lfloigjx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3btadpggh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jrmsqvaq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jgscbwbp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugqkpyqb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ogkaoark.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rycdwjyu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3fkiftwma.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3immlwutz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qqnlakxf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vgfythsh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3qxfsbkfa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3utymdpqm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwhtgbu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pqblizhe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwnvynpc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnznmtlf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebhcolgc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgmesrn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aakbzjym.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qfutwjmo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3znuvhqjp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kgkrxdbx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iypenqum.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xblmbuqz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rdnjuxzw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kniafggv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kexusvnz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qdloncii.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3eqqlnutz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lsfdvlva.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuarenzj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yunrbgbc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hotwlefr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zaqhaaph.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3httbyypk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qcwoxrqd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sfptvvcg.html


<!-- 参考信息 -->