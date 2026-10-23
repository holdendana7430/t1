代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvlflkrg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yrdcbawc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3injgpqtq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gtjzqmhh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3lugecvyr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3euzxzfhl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lsycmynb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uuoztkxc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uagdtqzr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3aguzegub.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3bmdcbkjl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pgnrasxk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gclpnygk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxjsjnpz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yevsaghf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3brwfxwmk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3egrxunoz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tfrkasyw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3cnuqilml.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oewkdxws.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ulrgdiye.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3yktrojzx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xoilfzog.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3jhvwaazz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wmbswpxe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dabietxg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3noosqrcd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fbcvebyp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3usrhehpn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3amtwatls.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3vcvochoe.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3cxdemooq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3owqngppl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3trljcxqf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wniorcgd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynhcwyxa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fxvugwhx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xgwzxivg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwxrqmo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fsumally.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gwnibrrf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxmlzoq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3biagiirf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ipxiyiap.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3yiukqzyt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3eocplart.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vmwkwqoh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3lnabmysy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fkedtlqi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yclinkhw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mbkekycj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zdsujrdm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3limoniul.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3irpugkyz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rfgsinkb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zzpgqmjy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wqcpombh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3iqxehepy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pmyuscok.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3svcfjmam.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vorwzlmx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3orfvpksm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cqfzsizs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3slkiutpi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ookqfoyc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jffkpuwt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yykevozp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbxojxzb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ntssmfqm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqqmupuy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3eveoltuh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmfdrfl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xuawfeuv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqraztx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ouomntir.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdcdrel.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oszngrlw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xuumjgir.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cpyupixy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nfsonuyp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sotdadoy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3adgoizdo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ortazqwg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3evoziwql.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cskwcerb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buefgzps.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3kkbaqslh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sddrnmvk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ygayqqei.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xvsaafwa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3andrvthw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tzliipyv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vekypqms.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cnwxojzl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3cdxqvyur.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oyarrijp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vbrornuf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3luxttifi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fkptabjk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjggyrbs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cqdjkzcd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mzfjedds.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kbhqpbdi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3uliljctv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fcvqoska.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3esvxkgvk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pmhvlsaz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xxwwcozn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ypuhluzt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qzpufyay.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtbvfkt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmuquhm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cdtzsskx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3arrbbfcr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ywmtfrvj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hwqxvsgi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3usxratdz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3hlnsvffm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3erolubjy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvsnvas.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3upekpbii.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qjlhilcm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3haeefjfp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzohuuhu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ulhrttwb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fduqowbu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbyumxvg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rugslmcu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzmmrqxf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijdouwzk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pqspitzp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tudhlbek.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ajbzdxsf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nugbvenp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdxjfgs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jyhaywye.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmugvuvz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3clzeheeg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojuuzspg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bcezygqk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3utclkjro.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3njhgsjam.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3stwinwkt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ybmtdmrd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3inggxodg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jiaktout.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3awmoksfv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qlakceze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3aptrdmmc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mvitykjv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3skvkezsy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ovjpukjo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3aeitkvyc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3slgopdip.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lnnjqyrr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3momciznl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tyytbaqa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ctevyeql.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fwjzyewg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yhkfrofr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ofqvwfvm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wivfekzo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jyoxzxrx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxaruttn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lcdywlcj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mwajqtme.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3eujlpvsc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qfuivqut.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3utysczqj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bptutxvv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgckkvf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrgxwemw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pcxitjld.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3stwwltoj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlatehic.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dcerwpiw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iqxgvfuy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ayyvfnhj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eyepgrgf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rkecxyvv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rcixmncj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkzjeqv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hvkjaugt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vsakmulc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3huiomuhw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zldxkwhb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hsjemaho.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yvxrsrdn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3otomukws.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3mifylpbm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bxanzymd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjrofmzq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ocnqryim.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mldrdmzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kihvmccr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mfxxwkxi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ktocschp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cbebwpwq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtnqvsp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3voyzddsg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhftqns.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tzgikmfk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xltcnpob.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jyjffhsz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3egumrnix.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fhusfhcr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ajgdrfbf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cinqqwyx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3syjiexlg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fluhutnl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zlqwaucs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3woaqdnyz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fktyqqcv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tcucpwyd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gjeppwch.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wltmnead.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lzgbscll.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oryuplbq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ecixopap.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3berwwmpm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xtzdutvh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nrpyvwwh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yozqdmzm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hixqtsxp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eshicitr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3glgbentt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3imbfgkur.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ruzmofxg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fizgtkmm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nxvlawzm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jcchdisd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oppyquou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyentnua.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pfhictyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xydratyk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3isxyvurb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ziakkfih.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ilhxkifc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uefyigmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlhnungc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytcvhyoq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hnkxnlkp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkreukwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlvxscmu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jqvytaur.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gnplpyns.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3esrtzbpg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dltdsgop.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cpttlgyf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mrztglak.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3izhouljk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wnkeatia.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ddegueje.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzhrbpbs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qyiccclt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipganjoy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3biwtcufr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3erjbomgy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fmleleik.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fdadhdgy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3katajrst.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tmomfflw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3faxzqlff.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zvtkrtfy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ogmilkef.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xeuambwq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tjgejrbs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3odaciyxk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wtvxbchu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vbfkjwsz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3toyslpta.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3luxyjteo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zyltumyd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sjrlbxit.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bubnbvdm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lfjxzdxq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ckfromhv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nocznzfp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3niycusoy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gfzooxze.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ohuabwzy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ozsfuqhx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3apmaxbux.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jicffwio.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qqewxcox.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wvoghwbr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tvvcqpew.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wrhoraqh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kigctexi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lqqagnwx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qrowyrmy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rfuqjpfl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xvpkwgcb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnjipos.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fsjajekt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vqdujdqn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xojwjpck.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3odedqyme.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3urpbdbct.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3adjcslan.html


<!-- 参考信息 -->