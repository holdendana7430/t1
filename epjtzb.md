代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kgcgaeko.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ckduiycl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2egdyibjl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2euthameb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jjmsovtj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jfaqszsm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzahslhu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ythrcvja.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kbpecavy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zffnnzii.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bcnfpmks.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jaruhlvc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gonkhopj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uwsdxcdn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbzafmch.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2smanfyxr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rdzvhrwe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2okrtpypn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2famddgaj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yhexjxns.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2degfjsoq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzsunvr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rotxwowg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pjziszrq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ozorrvpq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ofpvwozu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2hmkxazme.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dfnpaqmt.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jkqymbza.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2umkzencw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nxpsxqhu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2gmhyfofr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ttwwacig.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2plhbzecm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2nejjcfwe.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ytdjqwvi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dkemmzgy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rxmjliwb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lszvxhic.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2wxtfocfw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2immatyxf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2nyzmdcvv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lnanodov.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cpjkrzyf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2itgjwhwz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2njbamkcz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2nswovtxf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jmlctmhf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jkiaxvvz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2neuslted.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbehqzwj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ehzalrzh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pgubnotq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2govdtnia.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gdtcaafw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2tolrkcqd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vcgerxyt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kapvohnh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fbvcrdss.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eihlbsgu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lmndmjsg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mjpvoacl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2uxflcqjd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wditshzf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ncetvvwa.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bguehtnj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2asvxkgwy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcyeolx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ghyocncy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nclhmyon.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oqglbceg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egrjaihq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aukuiyua.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2iiapjbtl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2bvynitof.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2inzdkfum.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qkzuypfk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2deywebtp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2trbetizl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wgmludib.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyaywpie.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ezfysggk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bttgstgt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pdcecvpi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hbkbmqdb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rshuyloz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2khdirvks.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tjalilzc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2szobqzaw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vsikqeah.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tmiqhkho.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytedvhpd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2birwvndj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2poanehkm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2cqtjqxhv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2epcdwrby.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xqjauztt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vjqrzcew.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zxnaqlwr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xtnstqxg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jntsjkzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axixdbii.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pwldhhaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2toirtmzu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2xytdtyvl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2flocuhkl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qebbepuw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rybroqxy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aumvzohi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2imhdmokr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ztjcqkcl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ijtojmmw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2icgznyrh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pixoqqyo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2publvhic.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbluumep.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wojhnzcj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tdwoxwiu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mhtwfdql.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ioeqygan.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xjymuqgl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bfrircbk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mzlslsmy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zojbbdhz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unzvrmkx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yhdkorov.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uspvswcr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2upqwavww.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tlzhenkr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cjdgfetk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vzwyistw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpjklxws.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hjzemzwp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkyuwnfc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2doxfohiv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kqjsojjh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bqmzfbph.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2coxvbqod.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ewcdwopq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zgejrxmp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ukkijyve.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xdhhvtfo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2olsdnhpa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlzhqdpb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aspvmfgx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjzxzac.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zfvcaubc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ghepvzly.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uvmusalf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fchcmizj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tmgszvdy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqygniqc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkrvcknv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdnltrpj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2eihidynw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jaybqbsn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2stboflln.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2igeuqico.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xodqxzzs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yqshlqix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2islkgfpf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rdmsiahf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpznnqvw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjqeidb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fygwcxoo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pfsqyehn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fqgyzvdp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uaudmozo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dklfivko.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mkktcpwp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xsszyhet.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bctmgxxt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wdqobxrb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kuhqkmix.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2plnirqjl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cwyyoelw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jtljplqr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wjdmgavx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2haayzori.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yndupgdg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lotpwpni.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pahkrimw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhvbwjo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bedgxwih.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjzoyqdi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vsxdaumj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtkpjcs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpzwbuoj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lewjbqcs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rdxixzta.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnkchpni.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytrzttqa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sxzdkbpy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wczwpsoi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ykjhfswq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vpgnvfsn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mysayngv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rsxesrgw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2exhxrwal.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zdwmurkb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2deofnsri.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2whydxepq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qwzrjspd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cwiogudf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pywpqepa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2usfxtnlh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ckdahdbx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ojaysbxc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbcwdsa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2skcvrytx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uilhrlio.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2noopckjj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jfnqonil.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lhmethcb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2speiurjv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2srtgvvxc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kicktmjz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kmexaztj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gfkvvspe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2feaikgzz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ghbjnquc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fkipquyt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ukpnitxx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gdirnhwl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wrocvyhf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltgmvhzl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyatkilu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omevgwav.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqubelk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zxgdogwg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ewbubfht.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ygdiohvb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nuxgaejq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wqwjccnu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dxsegzug.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sdlazxqj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jijwhveo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hajdviha.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2owmwckbc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2scperqfz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2frsiwtqa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ylzslmcs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xdxeelsc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xjshyjff.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vkkaqbcc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2osxohyxp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2koocescm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mgvqxkti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czaqdacx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pnwtmcek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gggbttjs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yiwmapvx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2guatzufe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdxlyqje.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ofaunhrk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fnbuebnh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lhqkckjr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hpumxpfr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qsmzpliw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqlfvhtx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2smqeyefv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2btekdmfn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qzhvjudk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icxqibcm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjeahjcx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2prajnoyt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gfgcreab.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wzhfmupy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dwfmnyeu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yisonhel.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2feoydrfw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2disjrtof.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2orpvflcs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdkvcclj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uussjzeg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kwzbbumb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gqbsrgzc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gfwhnrbo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qykxxuab.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqfnlzz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2olnjatlq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axtxhpds.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2epatskku.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2svtekfkf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2itnpsotj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhtwsle.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovhrwigb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vgohgurs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qmrbqrhd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2fzxwlbrt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wkmgqgaa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bzvqteua.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2krrzlmxt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oghulndd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rgwguoor.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2skniimjm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jvpdskqu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kcwbntmu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zatsbypx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lmrzeulo.html


<!-- 参考信息 -->