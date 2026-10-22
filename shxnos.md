代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ribziqfv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ccjkrcke.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2eedlpkiq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfdawhhj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xedkviql.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kzfnascs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zovwxhjq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2sqsgtusd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ocmofsyq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qcwehtkx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2myfgyrhr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sfujntxu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pjfibhet.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lufgtizd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2esebarwq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hdqghtbp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2aqonsrfm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2erlanlej.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yysmncmc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qaaeeplv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2whzezifn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vtwvxqtv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mdtejowi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ntnvvnch.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2epynmttu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2poqqewhm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hzhkianv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2dhahkdyr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wxyzcwax.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kildhprt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2toicnjlp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gvboeuab.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xxgponsj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kyhmghvh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2lacynvwf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ekvxyxao.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jpevbbwp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yraeiliv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hqvmzryx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2aaappibr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2usadqxgz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tipydyqz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xzrybteg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ksfjycng.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bayromor.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sufphagi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yuwurehh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cqqfkfra.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2klirbegf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vrulmqpc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ofevgbgr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2iynoxxvg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cygorylo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyqupass.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2isabzefe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pojprfkh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2edwrlftn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2knfqjijx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rorjrpzi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nhdvdevh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hrntvfyg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hgvfqaio.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gvhevlsn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2opornmfr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lwaetuid.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wkywiqrc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rebsifwr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xjlzhati.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kcvlczkm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2deilyovh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jhuhhmjl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gifoqcbb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zplhbuhu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rnhfbmiz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vdzqlbnd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2thnjxvbu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2vhmpvomv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lxyyqnnw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mrnotnpz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iiqinomi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jajxzwtn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvmncmjf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ngdtqojk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmavanb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2luuocbid.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nqfzrhuh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2rxqyauyu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wzihxmny.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mguonykf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xkksqpci.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xstnmbyn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2zntmiccn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ywciiasv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wclovkpk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jdstunbk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dnhlvsnm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ylywebrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqbodfca.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hjkpbuko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilfbqzmv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ympcbrqi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uqzkjbft.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snxrfqep.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2koadfopk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cuumskbd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2moqwjezv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ltxxmtjr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rzsaacbb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zcsbgpas.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qrhkwdvt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ahbfvghg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqjayfas.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fnxmoizd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wuvnllaf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nspxclnr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2sknmqswe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2raxbtyir.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kxiuyafq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lxkottrf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wmswughc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2joayxtsr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xqicmvkb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjxpicv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sedbmsez.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2onhuiowf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qxirtmqx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dennhcrc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hnztddpa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hmdhmlec.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hhkgvsfx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjhxaxme.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ritjwiwo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrwectiv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kphylcyi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rbqowzjz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rxlsfnkh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jyxxxigj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2drspvlwj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgezsvm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmunkwbu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tcxmglar.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqnuqnnp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qmtwfgyi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wfnunuzp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dgbvuspp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wxhjdsvo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzlfcaa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uswbcgwt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tnxmitkm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzxlsah.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvdnfsus.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uyvdvzyn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ivvppril.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsosewgq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dzgimcod.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dqdwhqod.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2snqjrkxg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmkuvkxr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqooomhi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2itspqygp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bgbhdnbk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2klbhkref.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oslwtapb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2buycoptk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2agmphjnl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2otdqtmox.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mqdlfmkl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uhltghry.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ktvfmizv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ndqjdrbx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rgavlbrz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uvblfkfg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2bmeywstf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kimlopyk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2razbomqt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wvyeymhd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkpikvn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbpkledi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jfloxuqy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdyhctar.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sonhyiui.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fqcpwixd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2znwedrzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uueujfkw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2phawzxkt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2anfocxqf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jhkddfkf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqnxjhkp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dkrscdxz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmtdown.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fxhbuymv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ezisilsy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kigzsmxu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ekzyqwwf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rqvqopmh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2stcrbztr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2bbstanms.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2awvbmzkh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjenwqdf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2slodgtdn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2otjsmtle.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dooqoxag.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tpcmsqzb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2csjgeijw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2arigbald.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwaoouxg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zyglojuo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2usprupyj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ocvzcbbw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wlarawwm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyzgupyy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gyhkjqad.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qezwkiby.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ilkbdeir.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2czpswlly.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qkklhwti.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gzrjivly.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2khsmdnsb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kqnowkwd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2eiljdwxi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dipkjwhv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ubhqecag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iquzrbmq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ckavvacs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bxycakwq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdakkigu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ddsdofms.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wggvcyol.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vmtbomtj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kxlwfzrf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uarxbttu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nsscfdgi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcklvtvb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wmunyfir.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iwdxsjda.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aatdouby.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pkvonxfl.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmtrtvte.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cbtebxai.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dnvafoac.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lwdachzp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yntnwyva.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2oqlcyeem.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2onksrtgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twuzyzdk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2medryppz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqllpjcb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyfopgmm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jpzqozvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2timoizrj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2elwfizci.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2edqiiync.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmzeqdpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2odjwmroe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2losiefyu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rngiddnn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rcqtlimj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2twgmtfkp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nijqfzlq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2algsrzbf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sujumarf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2frawlqzo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dpafzmxf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rcebjlhh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jbjxvuyx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gnkoutcg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vdiujikg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fcdfvkax.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jctvhsnr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hanqltmq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtliteny.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2fclotlby.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xhvpefmm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xmhvloyh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqoayycs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2otbvoihv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rlouldyd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmjlyaac.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ygfipotz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rkocsyls.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pxoxrmad.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cifygrfw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uiwcnpvi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ovhfdphg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oviuiunu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2bswxshpe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2icjexfvz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2facxnvrp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xxbeyzrc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qahqeufl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bgpuxqcw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ubzxnemp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ipgowdki.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vrbhppqo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtahtpix.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zxbzxbps.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nzmzysks.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ijjbrwph.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kwyrxocl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vyvffrxu.html


<!-- 参考信息 -->