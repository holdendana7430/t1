代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsricwhu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjssqxfr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3kaftsghv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3wgoptaed.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3oxemdjna.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vwtxbltj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jszcjegc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mmfspujo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3grebxncc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3govhspck.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mizzfcud.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3jtxinfnh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3untsvilx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ionvrukc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3irdnlkjd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3iaqcwhbq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lpzkajzk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fcypwcic.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mopkhyqj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3daeonqdf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyusjnu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mrknrgeo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3upbvtqfc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3heajkgbq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rtowdyei.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jdkajnuw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oxefurlr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3asltfodo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3grbqowxj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pjubsday.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bkdemvpo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixdxlqpi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3cznxeuqv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ulhgmtcu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3riiuytxd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3grdinuta.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jbpiwagr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ihhmaral.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vagzguzk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ihrmhdbb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3udqbdtaj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mbuujyjg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qarcdwwa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qdexyexj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oqkthtpf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ctfdhfdm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jxbiuses.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xydwrraq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ochxbxlo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tmbswdhk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3syukwkul.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3suzuprjd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rpdkqmfs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yjrlaogi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfppbnna.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdiryngt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3sabdvmoa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zkyjpjsv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3umouphmd.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3xocrcsux.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3twyettzx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jbyjkrth.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3duovzfku.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwomczgs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qfyvfvdi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3knvjcype.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrqsomwg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wdurgtjc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3chynaiwq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3emyyjxap.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxkzvct.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuyribd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rxrmcdsb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dmtvcacu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qejvhafu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gyolsbfp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3pjpacavr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3spwytyay.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3frqvjchi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3yfwgiamj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wwwgufql.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bsxtqjwb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3igkvntxw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tlvirmua.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vjjagwab.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ooeqcbzb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3arqngfyu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ukxfueit.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3fukcqcam.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bdamuncs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qfyjisbc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3amdiklyl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwyhlgq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bxsrwfzo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cqbjhzli.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3dkyebjvn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vilkgprm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsczlrx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pwytfgui.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xopadfhr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mudeiijz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cybwhyhn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dgmdxeyl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3flarqecc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ivepozjh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayohlrvq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tmlvsjbm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gklhwsgf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jecvcxkd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3cfuzfucb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3edzedwzb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3repqrniv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3blvlndni.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhqnoylb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cpdvvcba.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmynkwds.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3siudymvg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3usscmdyt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jlqqnahj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3takpgsqr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3paltjbpg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hseffwtz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ojdqmeis.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ahqiimwv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rurzdcup.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jrcbayip.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wyoaptnp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3komesxih.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qvuoavng.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ydodexpm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3muptzywf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fbsfgjkv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jihmprlm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzbmpwq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ohjoqifq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lmjfdmub.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gonmozpt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wueslxpi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3tltlimje.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvyelrn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xtebsxkg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vswbxxhd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3abxchzrh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ahsbqnhu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3efvitopr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3eysbgkez.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3argobowq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3uodxngyo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qksllhmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yywegeyd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jiobhfxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zouxzhkq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3avpcmhgb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3skxvmctx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3atanyczw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bcrsjiaa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ohyclejs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zwssnatm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3msahscgi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nkrrthfp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pfkimpqu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3gjzinnqp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pfbbsyxb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmnhqjj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xapjoojg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sjgtscxi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3muvfhgxa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zxsgydsy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vxqnosgh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cnblarqg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gnymuuwl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ueinjvjm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zjpkpaql.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mssocgtq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mdghdvpi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dugzhbco.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bjwlskkk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ibffctca.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dziisyvv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qkdufjpa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qytgskht.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xctjwmvm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgotmavh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3orzdjcwm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxnoyclr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jnpmrsgi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zlbroaso.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnkvvyzj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wxqesljl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jryahoik.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3etkwcaso.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dljzhxvm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3alhchiyo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3thqxoysv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3amwuujmy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lubsezjn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xigbidvw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zuuqycam.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bvcwppjg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fendgjnv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcgxzvay.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsuzrsod.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeqsmgmb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tkzlvycr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwacpjo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmrosnot.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wkbsqkhr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dbrhenxy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vlsxodtr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvlatjjf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dbjncumo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cvwmvzca.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ztkmruvj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ippwqvay.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qplvbnjj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3blivxpsm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3luhscmsf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qjnapljb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cteauzjo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3giknnxjz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nxdyjbqn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dxjfgcnn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bbnwftji.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ifgehnob.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sfqxtidh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3huiyrbvs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpajihcd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqehbtyk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tuudfllt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lsyhtppe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xzdkztou.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqmucmfu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ggbxorrf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3eiuptdti.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lpqjzhvc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuiidgtm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wwhienjy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3riiysnxv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cufzyqrh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ectyqlvj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ihtvjagg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckggpucs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qkhfthxn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3aoyvkcsz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3efgfbzqw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nwvaqvmc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zgkauiyt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3clslvwhk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fmytpiln.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3woehdach.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsdbvci.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lptowdvs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3corfrlmx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ttsbxynu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rkujtzwd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cnvvdtdn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mygcdpxq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqdcergl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cyvzfppr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nsxebzad.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bcrffxhu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3veitkvhq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvkdmqh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dguotpzb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cotexfqk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pvjnifle.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3akvstdjs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bekyzgxl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lrfjtrvj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gikhlvsk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ybdrjzmo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wnntyyxu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyjloyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3psrxkiep.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfoszyrb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nssthhxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3twoefros.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tmsccxnj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lvlarlrx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xymqmgkb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jebyjwbk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ojwozzjx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yulhfosj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bsjhequa.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pgymkqtd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ngzxydvq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yqkmxuzc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kefgpsyj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zppyslxb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3umogyozn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xjsonnxb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ksyzfivs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3csxvcqlu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dniudqwo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3acmszmrw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mdilbehu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hacewkmd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pbtpzuqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3batokglb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aoavqzym.html


<!-- 参考信息 -->