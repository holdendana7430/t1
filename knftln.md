代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3sfiymulp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cgjllnea.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hdtkbkox.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hicpulhb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ljrjrwtk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jyipueqa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3asnhyibc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3wxzkbsxc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vwnfvmoj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3moehpzsw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ssfsucca.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lrvlefbq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kkvzbgrs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gljkazdq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nflpukgk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qatwxosk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3aoosbrgl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3scoiqfnz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lehliezs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3isciiwea.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rblgqzeb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3otfpilsb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3twfkduya.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hnfdggoe.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fcityopz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ullqxuzy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3etoreffv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ufmdzxgm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3famwcemq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hhdcuklk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3qfjgyrka.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3wafylqlr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vqulcqjp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bskymkef.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wmcmicaj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3makpzzwc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3iaergdqe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3emskxffw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mzjwcsvp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycbwbmdf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3owgsxmgh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xikjvpfu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uuheofwx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3maivdrhr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zezpxprn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wulbceyv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zgpmcqem.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wmsoihlt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lnbquykh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rhendzky.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsamhwaf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3elxllonk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ukxcpian.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gtclotoc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ptsehoyu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xxjqtanz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fowfdvco.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3zlfnvqcv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3yanolvry.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3lmxuyizp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3erazucew.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ckgctbio.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ojhpulnr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xrtjihca.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ujqwcbmm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3klxrvmwd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3epwmzmzi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qnbsnpxn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3byhcxfeu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rubmbyod.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3bvsnxpjp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3upuovxlk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bqezhthx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ncucufrf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cbltnmrz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jbxxdhor.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3odvnvxti.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3vzsbjgsx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cfnjeefp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qtlbzmol.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3iwixvodz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sbzmtuai.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwoszua.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pvifhiqp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hifjiasz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sixswsqo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uzvgdxaa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3tmazbasj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sdzbaxya.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnyurait.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dzaksbtx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ibcsodew.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rtrdaoxq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3agqzkoel.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3deckunmy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3izzcmhvv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3cdcfdyeh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oggjapon.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ggyatpdd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3odgsnqxm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fizdhezu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hgjynvog.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ascxnmah.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3keyxjxjm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kxdskgkh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eauyrwwm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3uhzszsss.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3dhqehuxs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjbmagnd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3oxquwpkg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uidzejkg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ruqxcdtm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tvakcbuq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dtyqxmee.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wxgxwjpd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iskarwtk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3yanppizx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vexwpffp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3axbzezsv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lphditwb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fnqkplow.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzzrung.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ynszqpvg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uzbbcvbl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pcwvzhdn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pxdjjhkn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pucxexka.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ftwsqbbl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zhqgllud.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rujbuvlf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ejnscyfn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hrtlmxkc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cgveaggb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgdpioff.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yrzsoqyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dajysavl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3uxarybru.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xfwwgiin.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xtypkvwm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rhvlxxpx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yaiejdia.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xkitwqgz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbauig.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hzmbuaco.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yfydzxkl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lymhgcsx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xiuekamv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lakvfuah.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xanhrjgr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fzabegyr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3naewzmrj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3oeodtplx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3uoiyoclj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3astllzyo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ktfiuysk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cbggrobf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tluofimx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wunkcbhx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3byyujvgv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vvehbhma.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sjuyvtez.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jqvcqnac.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3magyquyg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sgqcmtkn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pkdqxcbf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhiniaov.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vmmsbunc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dufpaceo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmvctmo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmwkqlkv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmcuome.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zvcyqzdb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bwgtlbua.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xsxatokl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3evafneam.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvrafghw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aecdjtcj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhremzxy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dnsslhvt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wcanbmjf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgynxpuz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ulrjsmuy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fkfwqynw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqeixbgd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdtclcu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lubspuru.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytoneoku.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xryhxtln.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kgiypzyu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dheifnzq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrzkgcuj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ferbvrzs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xidzyuew.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3buccrkuk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oweiljca.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pwqinncz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3unyuwjgf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkpymwim.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eduuqpeq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mxhhgquo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hbanzhvr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhoyhjv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ajtqvmza.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lpnbbeqp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfcuqzd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nkkiiwqz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xthgedwa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uqccaxip.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jcrhklba.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xtjixczh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rojgsprj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lawiffhp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eneerwqw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gpdoxboj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dwrmkaah.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jjxqbkit.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqvrczci.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jgyzfhap.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3pflqdnjh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltntlmjm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uznditlj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wvmgiekf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3aytjlqyo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lhvvpfrh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gnpfirpq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kabbnxod.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tqjaopqt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3yrwfvwho.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bgsuksah.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cniqjfux.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lmfugniz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpacdy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zlctbtue.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jsojzuwa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3femmlnaj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dzuwfxnu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fhqnslsp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kbuodums.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ouzwoykw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzppdkwk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3unrjjhsh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrdnouqa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ekydzqkr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3iwhzuhjb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3aldlufzw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ubkipcxn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvxtvgp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xaqrzavh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3exkdvthb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rxlipcwu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gmqwulnk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3caikxkvc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yndyogxl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lxaqsnzb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3juengdsu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdrnjmw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vjreunrd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zwjzrjkn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shzclqln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxahzma.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cayuzwws.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3woqzwkdx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jrgrmzhg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3evxwsttm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3skdlmaws.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lheeewex.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tcoimfyu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ocmbmddz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qhambpiq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hnurhxhe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3usvzowiv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rufboekw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3eymgwjan.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjlqwnu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3liwdguqd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sldeujmh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tvcgsxfj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3orfrrzbv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jjebecgp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kejarigx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjxrcxpw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3szzfbnsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgxguptk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bpzrcopx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yfvsragj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzhrpulx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygiwhiji.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqrsvdyr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3awnvbkpp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvgcjjj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kbtcruhy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbizmmbs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vpgmutui.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3awkiphko.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otjsvyzx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3evcqkuwp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zeroattl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zdbmjepk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wouahail.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yxxflarw.html


<!-- 参考信息 -->