代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnrvcqrr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oiiyxbxl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pbfizuap.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3sgdommlf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qenrjyng.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rdmcamrn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rvrpuztr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ngnjyvqt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zefyvmqi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kelnorka.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fyuvlhrl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3seajrxkm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qhbjxwan.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qvjtwzsm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hoxufuyk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ttzroxpf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zaiswzgf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3buqbwxpz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xcxyewcx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3butwcudp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mzdjwtaf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ovmljjrl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3diyxqsfe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3zzgprulh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pcrabbep.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zoduxqyu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jbneealp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kvcvreux.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aftaravc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oqtgmzre.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jkdabsjq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wtlxsxln.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vikdiyej.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3fkapuvfj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dyvcoled.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hwlgufnx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xnfsflgm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3gsmcqocv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vqwzfpbe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mqnimxml.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qjhuasjz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ezvqedeo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3klskyndp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aevnzpic.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mxzqdskg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hvowfasx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xxuvtsef.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gmpfpuwo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3thuiksme.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rbwevrwd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3kiwainbc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3xqambwco.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kerazxws.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijacigys.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3olfgyfss.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3timmvgmt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhhxbums.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hrwjecla.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mebpnfbf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rnkicrqr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jfblchcn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jnvnubtu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vaziysxs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydtocqbg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tceazotm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3guzrbrkh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xyschqul.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3obnmksin.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ifxpetzv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xztffocr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vrepouoi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xphvjcjq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bmzynbtw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3uhxenafw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xdkufhtk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ryzbgdcr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3zfidzvzy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3snybvabv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iuvotmts.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gnafypwq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xhjpdpof.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ocnxgsjw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3epotoazk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jobeyfam.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xbycczri.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bagbezuq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3nqjfyhfw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fhrlelbu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3uufrfwdu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mucmeazy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3hkptpgtq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3outjlpie.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3okctjydv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vrfukuyp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3douujvha.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3cymhuanu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jivzpucj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yosyhofr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ktomyvjy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pfujstwa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ggqhnnjd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wemwsedc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3auxnugzo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xzkkiktt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hqsdasph.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfctrutq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dkukwuia.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3doymvpda.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3codoynkp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pebqdlyd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3iwgdasra.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjltxw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dagtoyhv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dedevlpk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gzxilmrw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sugyoozp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kkxcargu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3khrbxrkt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3txunrxvm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tuincasl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jivodzve.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3kuhaaubj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rcvlveba.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ftnfawcq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3oikbvhsc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xkjszgyg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3stfsdawc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wwattqwi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mhpazrgf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fiszcqrv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hhimvmyh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vomiobxn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3bgljmums.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwuzawr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hobuiqhd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wotisvrb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gkjcampn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddgzscmk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3funqlhzj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjgbrqnf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3uttgcsvi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vzhppuxr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gqnjstep.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3prcvubin.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bsfnopkd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lnuqclla.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fcddnhmc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bwfmybli.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vrnypeip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpevhwjc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3txzupmnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsuywiai.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qnplxepy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zwedqysk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dgyxrspd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zodwsvoh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rfvsjlwa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nagjeigb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nnrgxkbe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wvtiyklk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hwiyfrhj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cexpdarj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vsxhigrp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pliijwuc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tsrraaai.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sedfowfp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ddbzvnno.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3lfonuapk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zhufuzyd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ditkmtji.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zdqkrbry.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pkrzvvds.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cikcjtxo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oppayfsd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nbruumvd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nqngloem.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3goviccot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3andieyiu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dtrmrzoc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pltxepgw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fwzhderr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pwlgxtwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vspdywpz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxctpggq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3doylmcpf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxfkmdh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hgiyqfin.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nffjyuka.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qhsxkdky.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3usqutjhr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pygamwzu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftbeezcz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jemejjda.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eaengldt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iezdscdp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vbbagfca.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3aldqclwq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vonnmbcq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hrttfyjk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3unqrwfal.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpfpmpin.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3utcrxbdg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ibtlwshg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3sajzsfzk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vfhgyqfy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bjkmkylf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ztqrgqrh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zkodrcpo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gmiwarns.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vroeiwkz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fbcwuusa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3googwutb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3egslztmk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vuifpvkv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rilhgxrq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3szgbpfut.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wbmudzri.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ljspazlc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kubstbtu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cadeoovl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yygminig.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sowfzmds.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ksyavqan.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tyxveqfb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bwmkggtu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xbrlvjgq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncvjgqso.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nqoizndw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3huvoimoe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sxxacvvl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xdemvear.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ewtdepeo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ljigiwkr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ltwxqgpn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ryybukku.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqibkpkt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xddtckef.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3awagqsmg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3brfdxmrw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kxlqgqlc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bydveopl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzocoppn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ulunenqz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3stgdwtpe.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gnoixayv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3modetedq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qvqawito.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxuoumeu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xlqveuhn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bkmcnmzc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uzbiyhpk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkseovni.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hfpgrxdl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3psogvrui.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xougrqbb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qtoqhmsr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iyujdrep.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cmekfbic.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3angmmyjz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xblklmyf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pzhkqpjc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3iheawanw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqyatxob.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lqffzxse.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bsorhvbv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hmhfzkoo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3chuivkpx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jhsfzbzu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hduimwae.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3coubqnnp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nbeabdbr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3felqtmyl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwzowvh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruxqrpwt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lsdvksgz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3plsqqzvl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qdcdstoo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xfxznnff.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cvtpyels.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mrodxfen.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3siertlmk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3byaquwid.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swltgtdq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fsfmvqqk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uhfgqitv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yggxccin.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxzebjaw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pxcdnozz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nbqckuva.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mlnkouem.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pdlvzzai.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nfznwlhg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ofssirfm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wmbvwysb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pdullgtd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3trlbaiqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nipepgdx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qhdslrxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clvnhmnp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3otzkqdyn.html


<!-- 参考信息 -->