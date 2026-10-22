代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sfrobfbj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zifdiuhu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xcrmplnn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ezwjubrc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2iauibyid.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbhick.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hburahod.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbaozwtl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yjgvkwlo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2iwytoshf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doiaupet.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nvqojwlz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixrfditv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2coestfwq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2omsbeshd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mrcinvwe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rmtgjmic.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2snirdnox.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iqcqnqwj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kjiqwqeb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hagmzvao.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2clvtpdxn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wyufkkcv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hudekywm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvbnzpc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2wstzvmjx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mwphlooc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2zzukdvgr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2pmezixjr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fqizmccy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mewrfeaf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2fqokzvou.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2sdqlcucd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zjbdpdad.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zcohagtx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ombcamtj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fzgethsk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2quvckdxv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jiferftu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2sphkncfm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2aeitbgrx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wojmjrxw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fspizuul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dsrepsia.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ijmgebaa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tyfpuksg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kxolrile.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wqyxpsud.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pfzjpiha.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wsifizdk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqplmul.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgnhyem.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvabgru.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fufjusmr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hoadtouw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vqnjdeng.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lzrmnnbp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwvluuo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ubwvdoxk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wpybksda.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rmpqtzwl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2rfushlpd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ryoutvsp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nvtvcopa.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2otwsarsz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mxwyabdo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2fvxdtsyg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vwufzddh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qizzrqni.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vkcbohdx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uetnuzrn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2breofkjl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oikfaqyn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dzmhgthm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bmehhdnc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pudndigi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqsyuhi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ceimawxm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ubhvwosc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zjekogsy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2yovyvkjt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ipltjsxe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nednlaqq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdanwa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cifnzdyd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nuntccsm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2afgvqnjq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilhowzxz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhtweysc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rytbwjyo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2losctqxc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxhbdtf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ozwtylrg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zzdhqggk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hfzzroxh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ttjamvnh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2sckdmzxd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sdywrktk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mqcoyvof.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dxeevzhx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2actnlthl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvqzksse.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hvjkglup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wetogvox.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gnoazdpm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2shtetfbe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mokdzbzd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cjvkneem.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aslnhdnn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yiqhghjm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzobznxz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mictddby.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2adfzcyuz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mhloaijv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gfskxmrk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqniujq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nycjypxw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lvhadntc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xxqailro.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvgvprx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fqrxqsnd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gapqeetf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nbjtmmcn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2vipebeoa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2efwenvfz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxqrpxq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2orzpkqnj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shkzuhtt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oowwnwgf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kqviujpj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zwrkpeoz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vaukfdrw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zdfbzjkj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pzxwmmpx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ktkvhfrc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zviyhfdo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2spyyzjhd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2swwdiurq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rrkzpqgw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nofblzni.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ecqkjrxa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xihmkjfy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2augxrgpq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkxswrue.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hxuvnylc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pieypvhu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygwenzez.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ownqbvuf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nmpioovf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mderkxor.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2furzobuq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylbeldtf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzefeapb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrulezij.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2powowkgg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdieaww.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gkxnpmcc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hbnweghb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2khznxuva.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zvofvksm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2soyacelf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aifyfzin.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfgdbppa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ufkejgps.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vnleczfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2soahuphy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfjaaqes.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zrviglzt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vcwjsmyr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kulylgep.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eqztvbnj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kyikulnu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hwkryzlx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2arqmpppw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hqpwisie.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eiehyexy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2bfwidzqg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2oommcvnc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2omsmyenm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ostgtsab.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ckvpvsfs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mtpmpwal.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lmqrvmpe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tgyexbkr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nviuhsyi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jhasenak.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tyudgsna.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bzxcwadp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2juflnozj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lwxyjcmq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vmegdjca.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqyjuqat.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vasslpwv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vuqucfgt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fkfiwdgc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2twibfibj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ygiivsfj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jzdmwmfi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rwchfjst.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nulznauo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2uabhqccy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wwkhxqzq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nnznqibg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ootywmoj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2agqczrky.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ebicvujy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrsityp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rnifvdcp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ozxyibgi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdfkytsi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ettslbfp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fkhlbgdy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2royuqauj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xwulbfnr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2emlsqfbd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gmkxumqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2auocqhxm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lxbfxnnb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kqzwpajd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2bbwnmaiz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pcgkmfiq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2awmyijpz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2avrikuhl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2iscxprzm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnwbsvp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2miexorff.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zzpwtrtm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qidisvoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmajrgnh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zgkkstux.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gfdptlcl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cmgljjgv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ikijopey.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mgranemb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kinrtxhk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hiumwlyn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nqglxskd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2frbxoiqg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2toagqwfe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvrgdjqy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yelgsrrd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rxqslcle.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2embrolyw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rdbrlksb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fhaxnseo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2drkmzxgo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rtfklrif.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fwaocxwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkojvfpo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lmzxisug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbmuyqda.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2izvmrjos.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eftvalut.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2quczmrki.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gvxhlmad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiuxaouy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cngbjvma.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwlmpzla.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dxsivebd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rftnwzel.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rugweugw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nxpigibk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yyrrllkp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsuudvmc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tkfcxsxg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2frsbktos.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2flajulur.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2guzwpyog.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mlnijhnl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ijmnjelj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2caawlytx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rbkxgdxy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2igztimmd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiurdnfy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2atsugiqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2eqqepeef.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuqqrfld.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2twsikgsx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2sgxciaem.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nuzjnvid.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2awxqfwmo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iivhfsep.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dnxduaec.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2lxpppeqw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bunbdlaa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amnzycdy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqzwkwe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bxbsmlma.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wponkbjn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bobmowsv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zuynzdjl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ucoxbcep.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2grkeodfo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mkehhwqv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tjdcaemn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bmulaiju.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fhksfznl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yssyatsv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2affmlwtx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nzeepwoq.html


<!-- 参考信息 -->