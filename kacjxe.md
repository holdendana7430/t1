代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ipkvptyj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fylyhrxs.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3lmwlagqy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3vbsjtzte.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3oziurwjn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3sicepile.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zaombgoz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3nvyobhim.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jwhqgqvc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rqbofnny.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nthndnth.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3azrylwzk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wiphuuut.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mcdozkoc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thtxoord.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hrgoowbp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3huxddogp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ywduhrrn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cvstyttu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zdowaeyo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ottjxprh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3igvkftoz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3iahkprhq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qtfdwgsr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vsufbdwu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3jjlrlrhv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ruczwzbq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3cevuletm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3szvmqlbi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vbibpfze.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yrkoamjn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3agqazcku.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lpmouohz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xpxjjiiv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tiwfgerr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ffehqssk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yzzsrmsv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vayhdvfd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3btthgwvd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3uudtlkwl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pudandry.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3kmwwfhwl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xvoyyatq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fteowhqc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ahxdepel.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xkvicxad.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fvtmlbfy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3uhdlfmht.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3pztsgwfl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mskyqbfc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tamukoyi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3euupijcv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ltadqezl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fadljznm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nhoyvrog.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3efehyfdc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ltzogjtm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3poucbjnh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3opnjehxi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3btyfayfe.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fdxnadnk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bakywqho.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkuiuepl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vtiztxtx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wssmhmyu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hmjhahju.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ejjlklkr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3quzysylz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rweflctx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cmyoxcnm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sbvzwsgj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugovhyrf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ycysmvjj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3plkcvspg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3fszcfmbi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rhelsdby.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbffzpvm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lqubcqfd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qttgvysa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hrqtblon.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mwayynxg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3freesgbs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3czgyyajh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lweserhq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ipyyzsat.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tsvdfsvh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3htwhfsfl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzwplmx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3nnllwffg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwqcazt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xymliete.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zuhbbjad.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gvtrflhj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3yqbmcxde.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bxkakmmm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3cijquazj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xsgfjjpv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yrdmmcvf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xgcoybwy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nyhwxsic.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdmzdxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csbercpk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3muxonvbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szwuyaaf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ijtgeoun.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wetkufqj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ywuzqvgi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hlqcaqfu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kkhntfrw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lwomiqya.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qtpazdee.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qijyuxqo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vvgkpcst.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mqhyliaq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hdemomvd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psyoljzm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uvmufsqm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lmscmipn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vsdqvfgq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3sfmxvogz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ipbuykng.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bckawfsv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3diuhslpe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zuohvtpz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lowwywrm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cyfaddsd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vmaakbed.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfgnstkm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yznxyjav.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3eolofrby.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fdmyzcca.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxrcqfji.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cujhisps.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpgqtrym.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ezqallek.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkheozhs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlpjbcfe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3naozrwpz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3shimwiij.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejwimnty.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pazhxmgr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ubqftwjp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhlxfzhf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cxmvyyin.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnysltdi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xddsrfff.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rwesttrg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dbbzocmh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3swbcfmmv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jaevcdsq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tsczniyj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbtcvfrx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkeaxokh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yanimfvd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkoogli.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wmebvhsh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cviqvzge.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3txtvhssw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kazuarlf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwamooee.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3trfstpjv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3psgussfn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmpfgxi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqzfavt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3aintupjw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pagznkzj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esupfhah.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mnphmvzr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ntauozot.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxukcxsb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aeyrfimy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kwxsunnk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vhilfixc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gmfkrwib.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rcswpxwo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tevfmxoi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ygqibgkh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rlqibyod.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gzwvbypo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xywonyin.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uekwlghv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3soouquhz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qqyzkpzz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3oewrnljb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fbbloobh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wpndlezj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fzsngdmf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ervibmfv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3klydtidq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yjcgyjjg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wvfwxklv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfbznez.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksacvwuv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3aobhdbnp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ixgmvbaj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3taoglmxc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nqoseyfh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jgqzbscx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3arhoiqcc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wgndlzup.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3peylkhbb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ocmfnqia.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3aqqdqpsx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbqwtxiy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cnxmhxsb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jzoobhdw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ysyjphsk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3scdkedqb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ayscskhh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykqxwwcq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vlnkpuzm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lpgzqedi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zimxmuif.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dirrdoyr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhromib.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urmdqjmd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hltdazxs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3afmhffzb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rypprwbf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vcgyltuw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cxrryjyn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fdfdoosu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wpykqkvw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xtrgkjia.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pptbqecy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3npymcdly.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vanntrel.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wilzzsxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pititimu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3epqgdsuo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fkgpohlx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gnemrbbo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nvwxixlm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vvwpmjza.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3patmfmqw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gconxmom.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iyrwlufl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hjckryzp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vyvkvgrw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jyijpitb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3shxgqgys.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mnhfdssf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3beoazcvp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iewnrtnw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sotocxrv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hgaeimkx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pvavvubm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gkdtndxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xaqpqqja.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vaaxleul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agrzaufh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oslrkohs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oewnofcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urnmcyqh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jfqznjnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyhnifuo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqbdqnvi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hosvovqs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3seclxasm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yjnsqfyh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zyedzvxo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lpxahxwo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ktubojxv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixepmhlb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jlonrccy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dofleveq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ugdkyyzh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sivikorn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lnzytsss.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzjzmuyf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hbfwhycx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3klhyvdqk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vbgkwdko.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3trqnvosw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3selnqkcv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3vmotealb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fqbzuzxf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dykqohbb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3javhxsvm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3attqewax.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mshzzcok.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnclmazj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3obvbxezm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lnsdseei.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gqvftmog.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xkmhrikz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tymgquuo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3drqbgugb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hxjpilgr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldmufvdz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uxvcyflm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3praljbcz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nawxyoty.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uxrapbng.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3epodsrpk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3oujbspsu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3potlvkkf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fwhwaias.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qhultrto.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ihigpxvi.html


<!-- 参考信息 -->