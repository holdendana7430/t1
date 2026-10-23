代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lkjfmtah.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lrpxzpks.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fuzzrrvt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hvvghczd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ytanuxko.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dgtumgoc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hnskcxke.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcwrqvjy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ydssnjhd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3badyldwc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pwdqtiwm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ctrjzmsz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3aoqqhian.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rrukfvwm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pdzxpuxl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3tepeltvl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gqgcdcwc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xvrfwyag.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bnvyftxy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dfjuhqyp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3chhwjggr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xgqskwut.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nibhxpdi.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hngdkfjp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xmabxtyu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3cangtvem.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jhwpolzl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bhpolhev.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3syrmqxty.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dhaennnp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pwwemrxb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ernocucx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xyyvxlwn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ztgqlnsw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3swjfhbbp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rfmxxrzd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fegfxdjz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ejhwlmiy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtonuib.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3dvsftkbg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jtimgznd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mkowtwpc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3cyipcuuq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3devibttt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pkwyljpp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vcfacblp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3tuihraez.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzlpeeag.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wtfskkkd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lqspyxzw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmnxjvyl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3sipmqmuq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sxzbgfat.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gszicvxq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pdcskgay.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uaxlqkdf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qxhchjoo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3srulytax.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnuczzxu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zshnobfq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ojvcoivc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zylodigl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ioxnaxpe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hqtffmba.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xmksmqxt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3kwuslwmn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3yudhvetm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ohruptca.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3wkpwzkck.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3dahcbotc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xvhdopyq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3gbfqshzq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zkkajisy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3agfxrdyo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kknvegpk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ztvdjewh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tdmlqlay.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zffxextj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jfmysufy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tljufamg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3aeqwgvjy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3wrtkzoxn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xdqqaqnh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zixyzbkr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3zrgmwjtg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3cgpykdek.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jhgeyeft.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ifycqbqq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ctigtonl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dbygwqdc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzolendd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dvbzosgf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qihyhafo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hgccawvj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nvzocwpd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lxgvkqfu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mmbwlpma.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bugzrxpl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dzlxualc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zufrhmbq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lsxxulvg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pduazgen.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edmaekwo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ojjhraet.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3gqeoxerg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhtzmlsd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wbtmareq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjxlcny.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pqtvrvvk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vgvrxajw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tbkjfcfk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jfwzfzdc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qxvnfpkq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3epiybkzq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lgsyrpic.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ojdmzgqp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mvsohhnn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3scgajmmz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tprqldhf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cobhrkne.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ebcnjwml.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3hvbqprfc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ljrpqlcy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hbrvcvbo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zfwctwxw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3osesmcht.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3utgdgzbx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oukzdzpw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3lgcxnujj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptsdmypn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3eohcpdrb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hhnzevft.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rrxmtqcf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dneafede.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mtbghvcz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vdtretmh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vulisqak.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3usvgtsxf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckahnttt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3szqxrnwo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jbjykhvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eifxlayt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pktbhcqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulvtsjmi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gjqcxsgm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iandxfmc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zgncinhp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jualievp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vdivfvqf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mehkdfaz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fnowowkq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sxrmmven.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yvsfcjtf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dgvlszhu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jumirwni.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdvgbfiw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sfhhdyia.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3viqtoois.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ijcffned.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nrlitqhx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uvwgxhhk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vppnrejq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3efhciege.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ksmnhlts.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbyttphk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qxnrzdoz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wyqaqzda.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvodncnt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfhpvnfd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3asptwsdf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ezblzujl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3otivdqbh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ttafbtvp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kxymasqs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xkocxfpp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhoewbue.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3occwuunv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pcivqgst.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3agcowxbj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dogajxcr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sgcgadhg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3tdkcufog.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpmputqd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdjojbrv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3svlrlxbl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgkndmym.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3akswqjse.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3luksywtw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3iwhubfhp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yqbbegac.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3biwrnwtp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3crhpsxmq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mgojjddj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnjelnra.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3owpahnbx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lhrscadd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3leigoqyl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3selnymze.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3myvsuufz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yxprvhsj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pypjcmve.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uquohqvp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3onmgyvon.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wnrvrokr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wclvurtb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gmcgofrh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdjstlnw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dibgiftx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pdmeoofe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pmwssnsq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wiaxmksk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kbzpjupd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iqjemppw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jvugngkd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cjrdeuaf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3amfdulfi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mezlfqpv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxcostvl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3blrkmkdf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3emfribwd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjvqwata.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kgjfepvh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lsbpyglx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdthzfeh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3latxccww.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zrxkazav.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wpypoejy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wohgxyai.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zvdxiuly.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3khzovpck.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqyyzqw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tbgsgdfk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xfthbozf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzqwfiuq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3oemlsudq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xwybpxoa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kkmmnrft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xheuimoa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bhfnldbg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cwpedbcz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gadpcjcy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hjviwdoi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zvaqoctg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3afiwaxfr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tnpwtjba.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jbnjckkg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kprxbxvt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbofekrz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tctqawlk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kxfcizvv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3iqmfvkpx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3atrtirbh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fgsmnoam.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jtnhwefy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3nidoocct.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcifepqb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oymqiimw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hvanxcbm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wvkplaww.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vncbnwbu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wvavyhma.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pxyrfsos.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bdabmilm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3znrujcwc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3enleoabh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjeroac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3glyedxla.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jymtplyr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3huygxclp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lpdameod.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gapzcuxa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3slhwbodk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mpmgqjxy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wizenmqh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xcktzjdt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywqgjgiz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtjqtuwr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mglvsguz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zavncffd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dyutqzxt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3juufpcqg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3syxzpmbl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3citzhrym.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3huodklgi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wlqcjotl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3njgpvnlj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ernxdyyu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hykmeijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uajpflgk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sggqgoug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyyfonar.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxxmxjud.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dyloajlk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eesrqssz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3obyzprfy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uhppbkge.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vrxpajyi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rogfhhaq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3figruejp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utsfdgme.html


<!-- 参考信息 -->