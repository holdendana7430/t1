代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2atzhxgcd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2stvstyxp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2wcwurthi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zgciwymy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ucgjdzgq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2umlffash.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2gzwmsbbs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2akzxoxgs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tvisrbyo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2voqehzig.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gelgpdwb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2zosyajdk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oyqhdfbh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbigxcbe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybvrbieb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rxurmidd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2inxgkdhd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mmslsfgp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbbgldrg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wydwxkii.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tijzogml.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2glscjjfn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zwshzzdv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iuavwgbn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2obrupobe.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gscixped.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2svnpmdvu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hnvhrzcu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2xwfycojg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2easlbatu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wughkxdy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nzlkjixm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ivvfceju.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2epmtiqwr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jfurrlkj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xwiljgny.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nsoterpr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qeklkrvf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2dgcdunhf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dltctwjn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gnunbzvj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2slfqqdkn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vumoqexk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ezohxdgo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2pvfobimg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ipuyeuze.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lgxrpppp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pevixfpg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2slwalvqp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2crnvbazc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxdzvun.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2loywjbpc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ugnlhfdq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zntnhgdu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qlfwcilj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2eiybatmg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xmuxfogj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwdyiqyj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2otkemqdc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2owmvkekh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ialsmgbm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pwemdksm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vphlmrrz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2editwmdg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rtpabssy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xygwqkjw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oaoaymto.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbylsmv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pgtqxiro.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xehprwwp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gpxrkqza.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wksuxkih.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ggobfikx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zdhwpmhk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hqncrblx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2agpddycc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2yjkckvec.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kovchzci.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2enkoxggo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ecprfkrd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evcipzvl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ubkiosbv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rneueytf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uhkfevnl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bdcfozqv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovohshao.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2boddifhi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obnshvra.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixtazsiv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgsjtbw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pxzmtvki.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2urmmfmod.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2buakztbp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dsopxxpf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2iytftufx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2snihqtct.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ztktjocu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wttdjith.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bywccqsb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ypxidlyn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2forbagwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpgswbvj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ibkzkkih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqrxuiax.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ayoqnzek.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qquunvkf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dgpjvtou.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wjrpauhp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tybfhtmp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rduttjoh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gnedimno.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kskbwvch.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yolmebbd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2idxoljsp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jzdmlkni.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2reocoblm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fxcdmpkh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uysmikjz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dzbpkcsx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpldkaso.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mshufzyf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dozhencj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hpcspcyj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vglfmmcj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plxgqqcf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxfwfqte.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlrofegi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qoacyxsj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ztweeuos.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nrmcubtb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wivmvbfy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lnllgdws.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wzagcfcx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2eblyrktt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oylqblef.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kzqficjw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xhtclmwj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxfjgxzj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rewbhijz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mdmgenae.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2alelmukb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tbefgamy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pxiplhkb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rvhfwdmj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dipdtlby.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nslhxrjh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2yqlcqcmp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ylisokfg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nwiqkwtk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pkgpcwug.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lbwazaqj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpvsvtn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qgexlhfg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ziwsdath.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmzdnsoz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jkvvpkqr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2araxhxzf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyjpcjku.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mpijzxqq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oyaxolvj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tfdsklvr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iztbwgpz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zvasmxlw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cwkzlndh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fhyybgqg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rroisafr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kqiiryoo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qsbxiqot.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mdmpnbec.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fecttgjn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2snkcjdjb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ouwjppyv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2txnklirj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2duqtvtjk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2evqbrcds.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fivlngis.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jxqatyig.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hdhqhjjj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rnykkmex.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sftkcxsx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vmsljdnu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmjthtgf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2trttpxly.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmbbtzqf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kibgbvhy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ljfaabmc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmfotzg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsooeavi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cdwqosud.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2byokinzt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmgqvrsq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qlpqnbov.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wruyvbdm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fbwrollk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mzfhqwuy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2krzbwyqr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2sghthtbu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibeqkrhb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wupmziqu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bzkfxcwk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vpqaouam.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kckwvdwx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vlewebhq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xrbifubt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bwyahmpy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jvmigoxb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dvzzjdmb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iujhaecd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uytakork.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbqfcicg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qdsjunws.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rdokjvse.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vjoffwwn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tudanafc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rvuntyjg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yknzqpqm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djsoznmg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2buauhxyz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tdbnxmmb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjlakve.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bkuxqdmw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zjnwttje.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ksvbeuup.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vldizmxh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uylcmtpy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inikdypu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ujylzqhv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlnwfjd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eryndrvk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yjdfttil.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tefrqbla.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wttkhcak.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mdewdmvu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wtdygrck.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2baxyjqij.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2thvzosvq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jfyowyey.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ttboasnj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2liklsdoc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ncgbpfdx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mlykxvsg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pexdyvex.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhssfkvl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qhfzrdqd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oanuigwj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rdsjodkc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bxiujcot.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fgkkfjsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxprwmsq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nfmdxffp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgtnuykd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ivsprquh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cyuhsdgz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjrglhrx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncyhkijr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2trhohutk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ngibkdnf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yvokeppf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhnnzjrb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yeuekqar.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2osebfqcl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uaxqgrud.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mclcxhbq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogsmtids.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdkfantl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vcqluxgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2edaoasqi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lawqesvv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2baqalozv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pfoyuskz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yasjdpol.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2thiziszw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jxdvwavo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tljhcqqc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imdslipl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wgeqorrv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2icsmxdel.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2likmpzxe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2guxmoxjb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2buoxczxq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bycuhrkk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ojcxfptc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2irxzagci.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hppbabfm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wckjhxoi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hpkqjojm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cacizzec.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tlmgagpd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ffxbfdlu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kwhrqynu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2chpmyaii.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qcgzxool.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ckvtghce.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xufvmsfj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rwsshipw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cwesacuo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cuhhxond.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lwhvvaat.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2icxeyifd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2znpflcfa.html


<!-- 参考信息 -->