代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3actixuda.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qeociiww.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xzfvhxlq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3njlcrkjv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvrfqii.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3uateygre.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nauvcchz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xwmnqfpt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xzkpyokx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jginwoap.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qavtdvwi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bjoycfao.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vhixuyyi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mdutfamn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3atzasoeb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3colifsbs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hqftfvxu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3afwehwxy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sprrrusb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3biytaiji.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tmnswezp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3fvzehxae.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lgebmmin.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3goncpvet.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ndadqfcq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wwprmhfu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wieiyocq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3trrddsfw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3txwcaece.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cxgzcwte.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3pkbkrhvt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbheutnc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gachmmuc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3brwevocw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3errnsdhp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bhcjbcdp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3icliopqw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3uxdpwqur.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otsmmxmj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3egnbhsjc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jrjqimfi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xgepbxhv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umlgsfto.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3xdtbcfqr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vbrvudrd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qatweotm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnypdlgz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qdajizot.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qxevbhjj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3omiucywq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tsmsaofy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3csdglbbe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3mtojqrdt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uofexovs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gyqlplli.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xomrmwxl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xswthjqf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mipdvwdf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3stxrtqbv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3uwjqxfxw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cpopcwzv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3gfmcsxxw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lvnrxefe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3webbpwuv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mmvpfbqb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nxhutuau.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mvpsztnn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nnfestzl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tvgtxfil.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3stzqtjaz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3drjikbit.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qflecgzk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ossawxtf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3arhruqsw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3blgsnqbk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pkacmlde.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zbydyexk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lrzwoibp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3daklgbjw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3mmnsdlfb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ellucizd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fycvnoor.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkppzxfp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmfggod.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcfweni.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hbeuzhxk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdvwulg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3uyokdgdv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qwohypqc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjgrtio.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3exudavna.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pspfxsen.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3auqnbnnz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bjpoqojn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kcauqgwc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3hkgimasz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qqdslkrm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kggwasho.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nlblcpzw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qwavdwwc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3biwvbyfo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wjpetdar.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rczctevs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xddibyqx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ppggbbke.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gjereeqw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tuuwulxb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kojiflxu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrfwenoz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gvwmfpxt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dgeshtje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nmlytlor.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sixlgxbf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ctqxhpkf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gozfjczv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cjuzkaet.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ouifuzxr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkgbcfc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jyweabvd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ephnnwsc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3guckebst.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zydmbreu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3svkjyeph.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mhpcgyyc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3obmqqgzy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wofhpjzf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3clgvoreh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3hjonfulu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vitshben.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xvasruih.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rajrntql.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bwiueavq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xbqerqpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhckaxjm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3eyiwowta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xztivkkh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xrqgfxhq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vnxgpdpr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhsunypg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ehkzrend.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3itfaaegf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zealrfvn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3paqrlqwr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dqgsmead.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hglensac.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3bpdkgrct.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sltbrhbw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmdhizxh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zgrlyudt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ayzszwpz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3petqabne.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3exrhdkax.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ghlpvjec.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xazpaqgl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mxmgbxio.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3avovcopf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmuvdax.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qifablzh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwfpmevh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exzmumhp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hixewkqg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ajaxptrp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wtftknxn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tmnescyy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cfsxwulu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwpdbrw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsindsbg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlygjsxi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mztemgct.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cdchjtuw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wxsggpdc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoxkyyue.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tmhkzrvm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qbmtshrl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zahutrmm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fcjdeiwr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3brwlhswl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3erynwmpe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3djnwkzvk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3figynffv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dttczoso.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3psnjtmad.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bevfqzlp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3phoedknb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fipmlhij.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgrusvo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jaougkrp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rluydkyx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pcjsomum.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3soghsktd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nglqvcdj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mhtkzgqw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dnqaicor.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rbukeyes.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhgltdq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ufkdnfty.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tdxffrbg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3exvqiboh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcuiyenz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uuniuhis.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vxkteshi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vgalcfkk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aurjiobu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ondgnwgd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3izowngww.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uybzumjj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yxxrjixh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3azhwmkyv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yqoysdkm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdstyhvk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qcgyudhk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3whupktmc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tliqxttw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhaytwpu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkzxnht.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jrqbrgnt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hbegqruh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ktvbqmkp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3iuxsxtkj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuwqpnra.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pjdmthfk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qljimjsc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvwzdyy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rirdghtg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldpnpozl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3eakwlxbo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cnxhhrrt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qhihkvlt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ezhevgru.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pufrtruj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rhxescqo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jugsbueu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3usptizot.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wmqyvjtr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wdonznvg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rpdimkjk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3oefgtafw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3oaqxptiz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3coqurpgl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fdkuwunu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wzlbpyjp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vzumfzhx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vklvxnzw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3czrwgvvx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kcgkmnrl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mvuqicog.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxdixkgr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hwobozfm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnlxpunq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lqmghlku.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qdpblkgf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tfckqrcy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bjnjvvjf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hpkavluq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tdrdcece.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zxmqicry.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nmrnqqta.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uukpgkne.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ykeptmqn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hqipyxnu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3flclfevu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3txapdbvc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3koabhdsv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mbapwwod.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3azbagbuq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uoewtuoj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhdbuxul.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ctqhxwmm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hrzbglyw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kkwnerpe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gwrrnswv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3aixznnxh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qhpczrwl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3znjritjg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xizckkrv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dztvndda.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bzairubg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nmhnzmld.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3upcsfsex.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qarkgwhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjpdblnc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kfmprwpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqiulfan.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xhhvynkj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uvpgmobb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ltlvifmy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eziunetx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzysnijg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yphhktcs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mnvifjid.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nqrpzqmx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3koxxoqct.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jsqcrvrk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ykthdrmx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ryjmepdf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdelken.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfigcaqr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yjmfnhgq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmiuqvay.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ywadnixe.html


<!-- 参考信息 -->