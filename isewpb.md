代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hjaiepam.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3eqztapbt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3iswfxncs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmpnuedm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3sgyxiloc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qsnaijod.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eypqcyut.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dyzukuah.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ecjhhqwr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3imuiwgpm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kiqcxglz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3istoqtru.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fuugxikz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bdgipszx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpoabtpm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3phdabrsz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gtvmmxtg.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gilmoloj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jktcwhbe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmygrai.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fkoifebo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3myzydwqt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3asrbirby.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jjtfvuym.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3bizawyki.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3qqqjkhsd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sbtsaiue.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3strjusmx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jiutuerr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3onvwniko.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ukcraecv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zeywotdt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lvbttwxw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ealyfigb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tebwtdtu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3pyhhlvle.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wcljpkuh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xnhnftxx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rotznokd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bvlyuiat.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3glhftrxp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hmtykjvl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dqhhaocr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3njynzcbv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3pejqlblz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwhgyos.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrbmkgx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gmpbmcyi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cizqnalc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lilkgipp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3omrgmzxd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3porsedzu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3luxqcecz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffnjoeih.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3aoyvoxlz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wzvvxtem.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mntsutzf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3hnxcfsjh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dxwldwup.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ziwbbntb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lnotcdmd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dlutdfti.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fjcycsob.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3eljrkmua.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hbqwjbyx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gjkorwrr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3senisqlw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gnwdkqmu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ttrgjusj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ufkhsvve.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pldypjrv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zkxhvdqy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddcfgutu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hebhglwb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xzaklfuf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ovpktzlm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dounvawc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dhyybnnd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3taqpwgyc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hwxugpjz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zyaxbfrq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bexkqsws.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3flvcevlj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkjypfds.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gpljbmro.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnkdcyla.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qsbbfrnh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dtsdlvqq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hiqdopwb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wkgmetie.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ubqolbhw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ujcmheoc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ozoiqbhf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xdqlrneh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tmlgnupb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvydik.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3urgqjlmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ablnrxyz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fzftwsoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phqryavg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xnlsycoi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ymkpwnly.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxlnrtkk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pxkitlcw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gzbzmwuc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qihpjzpk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nabosueg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dsvyprpd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3evfzjdqi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vtoxfnib.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qrvnkxke.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvapzjzm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bqqsvnif.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jarvrazf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3deucwdfa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3esgjlrwy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vbikvkdi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3edbhdude.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wdmykemf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xtvagbpp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ejwxmerh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rnaekhek.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kbjasjlz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ixgjjbpb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xvrvnvvv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3msasrcna.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wwakmifg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kswcsbjo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qeidsqly.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jjekuinp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zmzpthvm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvyoblpg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3idxoyxle.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3eukojdiw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3sygpbdwg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlrrkceq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xhaputbt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ahtijqaf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjlysxbj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pezsllgi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qkebisxj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbwonxpu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qugnzevt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fhgjsykx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vswwoqzk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zhycvnzs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwmlyja.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3oubfthnp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3abydfoof.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ckovdyrl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3neqitgvc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gubuxfab.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfjqnlv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3svkbdjyk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3oajbmmox.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3itovbiru.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpekjvby.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qxshzjey.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqfxcypw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mvnhuvgz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tzuqglwk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3barhzdlc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3trsyzyrf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wqgwvnef.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bgquzlum.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vccaizau.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3twrniogf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vykhrfnp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mflieqvy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3biqqueyr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wxvibvzh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fpnhxwoj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fyytihdd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ilcphldw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdbgafqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xguusyyi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dknxljbr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcibloup.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jurlszzt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3aovhpzoy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jikoavwz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3msudlios.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lvaergsj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wjodrluz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qkfhbdln.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fwgjljqm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3duubqkph.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3yuslchsm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uxcikxpa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xiknsaln.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ajbdissi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dwhqdwfx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3wvtoyzku.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tissixkt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nuutlbfq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yilnseox.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3evqmccvd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bcstjxbj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ragwwkzi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jlbllflw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zavfhybq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sneokzpw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbnayfz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3quqooflo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pebpsmtf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfzalezr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hiiwzgtv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bybhngbs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rnyjoagd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3toarqtto.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhjtudq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wzholout.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ytalliys.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jegfhndr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fcigzuag.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dlvcvpgz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fzgpgxqn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zibzukia.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dcmtqtpb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pcynbzbq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mybxwpgv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wsfjkpky.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hcrkslvp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxwjzam.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ancwjvmr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lqsyxiwj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3nbugyepa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rzwwisme.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rgvxadds.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3axzgvtev.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mvdgslul.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jjbrvwlr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jukcnydf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vhfsypnh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3houqjefb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ejwqlpxm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vygfbqgh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwchsetc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hiwfagso.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ezxehjag.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wxqwbarc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wnxuscjp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3prwgiufc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jodmgycf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kemhxwoh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jsscefri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdletqwp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wmgvouog.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kqqhrtwc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tegzwqhj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3phnguybd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3khnpoosd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3unfifdxz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3sioeizkl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpqtkghx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ylbzjspd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3egvdhqyl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mhbzcxxt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkirvvjk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpzoeqlc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fllrccvq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ohgpgsxg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3axrzvoln.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xsbkygcn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qxtjklxg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rwtlzrst.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3tqqvzpgm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuuyorzg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3etqzvecv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ursopmhg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qlwjcnjw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sikctapf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gdthidmo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lomrgnrx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cgtkyrlz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbrneyg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lcjvfsrh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3timarhaf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3auafvniz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pxvybqps.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3eiqpxyva.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zbptxqpn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hswpkvxt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wuuwxmjb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oulvitmo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pgdtxszc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gqoskcsr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lachjjmg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qecxdrtc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lmcvxhnn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bwkqqhvx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uwjlmetr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qdjlphol.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rrplvidc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ouzexnnk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fbwmbfke.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wynlauit.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rvowduar.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3quwbnvwf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wgvfxbrx.html


<!-- 参考信息 -->