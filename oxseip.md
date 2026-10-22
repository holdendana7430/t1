代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mtndadoy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rieecprj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itysdifr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2adizqscn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oqudkwry.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujkoprck.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmhowpec.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqatqlob.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zwcnuhmg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2irzrjnys.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsbeaazx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxlewygs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hstgtaip.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2buswsnag.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cgnxtjuw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yvprkkdl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hmgbalnn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2xhfjnivq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qpqyrjxi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2acmzyqck.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2duyjoise.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qkbbenwt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dszqiipk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2irrjyytr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2selldill.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xvvewynm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jtywrreu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qzwrkqts.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bxwbnefn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pvchnyhb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2smqcipnl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vggpjiyh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vexjnlsw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zrymqgqv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2crhsfdmt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rkvucipz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2enlhqomo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wltlvpql.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2eytynyzj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2sglwpmxv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2vobhevpv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2edgwcabt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfjjkpo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nvwhjdnx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xoasifdd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nbirwnai.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lviyulqn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2abaraads.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2irkqsnzy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aznlccon.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vsoejira.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2cjgwsmld.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uuiqglse.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2esgmjhoj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jdgghkwk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jbrpgsun.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wdvwuluw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sotswfre.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vobjphvy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqvdfvd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jykmznxh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bcwkvrmq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fglvqzzb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqfktbb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rbvxkwnp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2umphxwga.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xuifsekd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2szzyylul.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjawnerk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rgsxznkb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sztqufef.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2fkmpedft.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irfpnixv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zpprmsgm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwnpkmbc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2radcdstw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2flfjakxf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyowrixr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zagswqan.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jctjluws.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cpihyefe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhcwucx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ptqeffcw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sigsiljb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2oxtmaupj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mkczurli.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2npnifuwq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mcwbfelo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2frvgowic.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jafzqexr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2tsxcergr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2emvobfeb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2aawdublm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mraojivs.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dydhbahi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikanswir.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jiirbuix.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2oifwfoqm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzthpgrc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fsvyieuj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pefayoie.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xkblnbia.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wajiyxko.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ejdfdnsh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zueccooj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gnnrgsuc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ktczhqsq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbvpdkwp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmczsy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ailqcrtg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2roqdrhbf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vhqjjknz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2iflwqpoi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rajpihos.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bfpltxxa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2cezlhewh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyyrprxh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjeium.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hklmdhbf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vpvfqlvm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wfcvwouv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2njayloos.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cxetlhst.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mbnwxplb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2skypfscw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jgwzuxfn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjcncawy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygbrqpcp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kforsojw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2pjggmriz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rocazilc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ikqdnsem.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cgqtyjfi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kyamuulw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrnbvmaz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lprspgtu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpfimdxh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dryziiuo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lnppufnm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fkrnbnpa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzwbkjny.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ciryhvjx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2msuwwwyt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wgqjkses.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jufbqmna.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2asjdojey.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2agnutvjb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ccnuguyn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqaapiqk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dnsngfmr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvstmrlv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ldrhdziz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dccbenau.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtsswcev.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmrzzbcb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ieikplve.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dmqfmyav.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2viievqww.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoszdocp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2muespdnj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ndfhqbig.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2brpupcqw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xnyjgmsd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tyunfnqx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfuakpf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yvtihejv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qfofntnp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qtmdhnia.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zqznbqug.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tjzfrncj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiynuort.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lnsmiscg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwxzebce.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yshhciuv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lljdxgxr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvntfck.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiednkbo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yynzvxtc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2buflfjim.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ekbooagi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ujpqnlyc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ledquzyz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2joswhext.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2iqznyddu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ttucsarh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mhtesgfx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tjwflqkt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bliuqhxl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkdqmxk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kwuhjfdt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dheazrrp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ateuvcpw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zmoupbwx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uzedrqbd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qpmdytgr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nlrrkltz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rcoqgpsb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ekhyltpe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ptdyjtca.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xaciwvti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hggafaoe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxtawbaz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2omqksxik.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xtnhhzrn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2iqchyrbf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2efuwsfho.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2erzfwywo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2irkfrqgz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sklrkwlb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zunnhduo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qgjjlbah.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ormlzklk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fmsqygbm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dfmxijlo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2copygnsd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sfhtbhfv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gcztpwjh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwfsuuj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ennicpng.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qglfrvft.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zhbojqlr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frtbgarx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fjooodsw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2axheewio.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tfanxzwg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2unifqcky.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nrkrwarq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gnftrsog.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2udnatiac.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vrduhizn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oppnicai.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vchdoawu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ackkppdc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sxvdgawx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rusfhhli.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dqtubzxf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vtllxbvu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tuntqcsh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qbtttgmq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ugxdzpmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvsaajgi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2melzrvxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfhjfpii.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ekaquukm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dbxrvqzd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvwgxtln.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqiepn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdokwtlz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2grcjxrhi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ikygkszs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cexacqyr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dhpqczhq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ciqlrzxz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yxjimzer.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kawdfqso.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwrcrqwm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2emunyfro.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wgyhymix.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2altoslsb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nsivqjur.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2bfvozidc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2faesvyyp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ektxppre.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuubcmnp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aehyvvdg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyousreh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2etikixth.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pnlvrpuf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lmliribo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2duiuljxc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fyjrafye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgelmju.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pqpjdhzg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esnpakut.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uqshjzof.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2icjczuls.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hytqrtfp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dherngjh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2venbeeyy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rrajyzcy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2capjavye.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rihmpcih.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qwmqyuoi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dzctvlpa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dbbvkdjx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ijahwbjd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mlzkjcvg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hcyjuwvd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yagemcpt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2wrlfayql.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sbhvinfq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hgrhhtvl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kvmwgtlu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ysntghxr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nztmgxgg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kgliyhux.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qshwuqeu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2migqkrgf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrarxrv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2weamlwbo.html


<!-- 参考信息 -->