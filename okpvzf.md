代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3rhimmacj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xqywavih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ffnwntlb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nvgmrogg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ykwyzhwr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3opnwckph.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pmwgfgnn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3phlenihp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nelyqvhn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lhetbhxv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eadwpupv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3kuyibnpl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mnynqejt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iryfsmby.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ljehsjyu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3igvznhqe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ostuuwzz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3khxegscu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bkvrmisz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rimtbpgt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ngiyujqw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lmqflpii.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gtspmxie.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ezzavlqw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3espptsov.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mzpnpojx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hzjqlqtb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nsqbbzpy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ecgysuhx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3eivqrwsp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eifmfvaw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xfqxqrnz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ictcbuur.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hydobojt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gjullavs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3nfnwyush.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xrvvoycu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wtyoybjb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gsvitpqr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ghgsmwmo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mheqctbr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gffihkgk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3tqwdbzbg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nzgfrqtu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mlgmrzko.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3smaxvlyz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3pootmhmw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3olmuvzgf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jhzspdss.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xpltclco.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itsnguje.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flxclwsr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3yzvjnqjf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zrlvwabc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rplebxwt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3jhkfoepg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gzsjqdyh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tjbskvfj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwkwutwk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yugopfxe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qbtobmzs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kftruabl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ilfhfpso.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3phpspzre.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ytvevect.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzzxhrl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hkqjrapv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrisdtq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dvvbdkmb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vsqmlexn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hxoqivvc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wzazalib.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3irfynszv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3sxerytsv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qtnqpfhi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hnxalpap.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ptsmttrf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cksbxgos.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3yptyedyk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ytrkkjbs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3karansqd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ecogyxut.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3epxjreiv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3unylvfxt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3sdqlyfmn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vadhutin.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xagftqeq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ptqvpyzd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzkzzdk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3pwpxudbu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jowrtbjq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cvgzesqc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3noxmzhvg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3azrssndr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzizoyku.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3adzwfole.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jhxvxqqz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lisvwrbo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tqihqoiv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xardiucg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bbeenlfm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ygzuulez.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gubucfdl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dtjjwzwg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wobygywu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xrfagxch.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsctuhlb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nambfybk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pymiurnl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kfvpmhet.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gfmrppdf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbheitgy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ezphdrli.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ghswthms.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rmrwvvdh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ztkcquno.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vshokpdj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tjrvijsa.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bbjwuvqd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ltwukedb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dulorinm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kygnxreu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oiosesak.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3betvkrax.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emaaqsxx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zcuuvbzs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nzagjupw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yjhigpig.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ibjepedj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykioppji.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdatexxw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmuzhuts.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vorcjtkj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3drjegojc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lkvrkmyi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ngcyczvz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rzbijcih.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xggfjgkt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3msqnfnst.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tisjulqe.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3enfydiad.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xxekerua.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhskcnoj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zhasjdag.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gatqovor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaogtabz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uhonksow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgqxjmuk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3muorucss.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3juzjghjn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ypvgbqql.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bdxicdww.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3azwvpdbs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3txpjhapn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lrosatwf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tsaupffk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tbapkhay.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ljfsjktb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oxnwmtex.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utmvunoy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vedghybm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qxepjouv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3znezykuw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhpeqne.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ekfvktpo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gxuczyyc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kcxskkyl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bamujced.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nvtxkdoi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3loduqdhd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sljcbwva.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3czryejgh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3znywjrss.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yfhpjrno.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jetnkwvp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3itkfhana.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3tdhztyxx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fgawddzc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jiknyyjh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvsclsch.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkdhcme.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3yoebzhos.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vpebnouw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hitimqhv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sxumadze.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oztnjgkc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3agaftvco.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrefxnx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfyotgt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ijicskvx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eiotuoba.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nuxifsht.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwneyuk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3cxynakuh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bqaedcod.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pibilgbo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3inueynek.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdeoneru.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3siwgpnkj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wvyfhxbq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3iibypisg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3crrrvqyl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3iaejzsvk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ztjvlxtz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yzwevvgs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlanvmfz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cmimxrqo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xkmvytqk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jsilmkwb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljvyjmtk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wrgsyzbk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3sausvnvb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ykpfvlhi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jgjzgjgr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rhrlgnpd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vkhdonyb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yejgapbr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3miicnnbh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tnakoxyd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3enojsknm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fkgqrfmi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zckwbrgw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hpkkagwk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mvcfajll.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3btzsxxix.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yhiiblnt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hssnslpc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zgxxtbxi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fgajtfpk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ypycyuiq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmcpgwf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gtahvzwn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kaqhvmhx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3smumrekk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdfwief.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3aodpcluq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pgcdxpqp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3glkgfmhk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zmjhhzzz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3sxqeujrf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3houhuctm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wludneqy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cdqzkzga.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wulddkeo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jfmuihww.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zosdjhbd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ketpzgke.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fmahklwo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jdqwfwls.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zhbqcvzd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kexlwpll.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ubsthapg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3omjnwtbw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dcrotmbq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hlxrrhrd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xtmwyrle.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mjdruhwt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nshqrqry.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pkvamvqi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3scaqpgnj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iuehglbi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3yxvsjitg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gwaiupuk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tqivcvtn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3raluyhdn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jcjpqzed.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zyldcinu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyyyvbi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jgkjqkzx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnolcel.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pccorbyn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3sthpspay.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdlqmnd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3onbwcpds.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gvqjjuqz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ktfwmbqz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wukdlnoh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zstpydqg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwnropaw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mfqgqvzi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3owekonol.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ahphotng.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gxdoebmd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gckydzlh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vtllnjsc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlezpv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gmqneiud.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3husnxmmp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gmcnldte.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mmtjzxoz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cogsosgw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hcxyeqst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkvflhzh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rqajvuwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzlhiihe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hizebjom.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vhdjvqeq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jxmcsumz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3deyjafli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utfsebxd.html


<!-- 参考信息 -->