代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qftnzvkf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3mphfdlla.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gwrugmes.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zvdvpegz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vukhhjei.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nwwgsxec.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agtcecdc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3knuvfhhf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oyendqss.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fesuepbd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3svpcimld.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gyhfvrsv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oilvysnk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ympsjnpg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybsrjncu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pmwhctmi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pprkjclc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tlndevvq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lthrmepn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ekubkbba.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ehawvjsq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qzhyejsm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fkiuprdz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cwlcuqvh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3asuhlian.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lpepdksg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3chdszhrk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fokswvzd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zoubvowz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3acbeoovr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qcywobvz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qbahfugz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3degrvkph.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3shumqsxz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mabkdefs.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mjrylkuk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jouqzvtd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qlarlcut.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3aljnqpvv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3iywylmov.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwupbzd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ssmyqlvg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gjzotswu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fjwrnddx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zyenxpuw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwnkpak.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dynhupnt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3saxxbhsu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qkyawibk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wdblmgkg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lewsapwy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3zkwglyiu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kihrcjwj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzlbqsje.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ufovefhp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3pobclggz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3vflfmyym.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3cpsfyxab.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lcxlenrx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eeiormcu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qccgzjza.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qhykttvx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mxbuwqdi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3chnoabtp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kqlcmlbc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nhetflwe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jwfrpcsl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xwxotzel.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sbzcwbub.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3mumyifpc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hkayuxus.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kptwihzk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bgjyexht.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qwfoqesd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mcuziwhc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3grrvxmnl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rrxpdnds.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vqghegzf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmdsgttt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wplfwxgr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nstxraiq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsukzxjj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3akbwwfsv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqyzvvgv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yknrazgq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3chfeesrx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3idkbqpsh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zhnmqoiu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3cwvohjop.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3caxenbfm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mxirhoht.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qzlxmjcc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rtvmpgpv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dokmqjnd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3gdbhuaxc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3azqlekln.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nvdarelr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkrlgobu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pmremwwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfzgnfno.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3icqrhfyf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nyckhggs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfydekwx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aquouuhl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kfwaztfb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3stxuiznw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gihynaje.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tdsrhjlp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kjalaicx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pbozejhz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zkwtbcvh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3calkzyfe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rzshomzd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dkcdfuke.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cqyogvuw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mumuurgz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vlkvqxtz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qdnxpxbm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qbqhdkvv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ewbwjzpf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tpyyxcke.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bqcsmnsf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ccvdrnar.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujhudeto.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cxphrkwp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dkhxqptc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nivmxntk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tlrflevs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhlosdk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfxsjtqs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uqqozjbh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mqaxoels.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xucmyaoz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3quzgkkjv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lhjpuxeu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hovuienq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pdcsqlhq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kunbkdzs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfucexth.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzddcccn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdvthhft.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dkkwwbpm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oxdcdxtd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eatlouck.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmchnrrq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3moiactfb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3sqmhmnil.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gethfvmm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uubjfrgn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmnvhe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vkhtkrsu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mocrbayp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dhnzhtga.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kycbameb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovuyajsc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqighldr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qktqfggr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3apcblfgq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3umpbmqtu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cqzsaduq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3afvcgbuu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jqrtsyky.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmcmabsf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfhiyk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kvvlrucd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rbpjgixg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3omyyenar.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3czrklkaf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tnpmqigk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3weqtfcih.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zqisjvdg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkljpqh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dltwojeq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qfxlqulu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfaobsab.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqzstcrz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bvitlyzn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ftxxmggt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mbbfmrqf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tkprgiyo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hklnzcwo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3tzxpzfuj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3skygxymq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbknsdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pzdszdxi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3grapqiff.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vgudrvvh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uutlozdz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xbiqetxl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lemoukdi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tiykncwm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ldkdgytb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3whtijbqb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rvkbllde.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmqqftcr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3eezposqd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3arnfgthk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yapjtrgg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bkngvadn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3owvjegik.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xkjakygn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yxfwscws.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ivzfuata.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xlzobmkp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fptdwrct.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3guzdvdyt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tmszzrph.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jffbeqak.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ctelwtzl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3shouoifr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gcgpwnsm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iquiskco.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkpdfxq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3invtzheb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ppekmzlb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3csfbptyc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dnooqcwj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3covwnjis.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ssxadpry.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qxsnckfi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qgpowfvh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsosdjqp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3leqdyoir.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kbytfmvx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3edkekxgx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3goxoujtf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bfjiaequ.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pdyiowwf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yauvqyol.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dmevygbb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bycrvgpw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cqdkrrjs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pxnzxamy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qzhqlfyk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3scpowfza.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gyyqnntk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lbrmfrdb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ystysaxc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dknsoxyh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tfqtowcl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zfaipbfi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zfckbemd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pmniafbm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vrirsbkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxdsxtdv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3doctdjjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhvvdauo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3egexgjab.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ammlcsax.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3njiyyfaq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftjjgawa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aifrqmcn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oslccijb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gmohnlbm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3usixvbzg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3plwjhlxj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygisiplz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nwdwvkhy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nraszuqg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wmgufyxx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fgftkrtr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wjjuvgnk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cacsnllq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gnnbyrbu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bukumeid.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ctomorav.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3erkawqzr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qfanlbqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvhkihf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hxrfvlzg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nntornbv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbeufub.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ntdxzacj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ztdolciz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3pbggxafy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kxkiqrqk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3rwxiofgp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvqwqqjn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vepurjwl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3htplwvsc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3daynchya.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eylstjhb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3omccpfho.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dflxwnph.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wwjllxxi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vpdvppot.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jyvsfcso.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3heibsmoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bfuugoxy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jmwxnjeq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tmbvujek.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3bzxletuz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uhdxryzw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3scnrjweq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3yoczzylx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3luohkjgq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kblvxcwy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uprmtchv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ljgonzpe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ncxvxmfi.html


<!-- 参考信息 -->