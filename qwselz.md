代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xxpkzexi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uwsrjilo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qvwfggfj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2pfrswzcx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xnwfoyiz.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2szqextpl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2lakigpvb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mbkfjthn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zpavvykw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2sfxomvme.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkasvesk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ytrtxebh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2drwrzkag.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ocjqddvn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lernikcm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ayjlbpfl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bwofvsch.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2frmavqgp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mixwyvxs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyjkklzw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fqxxlanf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2quctsqjb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2behrrviu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfrxhnxv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2quvdpndl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bmzfpzel.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bbynvljp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2omcemtso.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2udsuceyn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2igxarffx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2sgokolcm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2pokkleye.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nqdojlxq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkctqolp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2peogxtmk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kxznkfgg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aawkkvnc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2elykfeuf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dpdzypke.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gvknczkj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gglldlgi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qbgjvcmi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ofkhfdkt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mbmtlcfn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2romtnpwp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2phuudcvn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gztkhnfy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2socgjlrn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvizjkk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jcafkeaw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wzbjnboo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zewlvsgl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2vfinuxlo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2snyryjyo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gzfoexyk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ojgfbstg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gcyyewll.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vjasvcvm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwinhwv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2noyikiiz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2akajpdbt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjyalty.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2meahjprl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hwvuzevx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ptibcnqb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2igobdxbj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bdnkruus.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kypwqiya.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tcigtclh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2enisysfz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aqxkblxi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2udcawyqd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bnlkqpzq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ctvgsjcn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dfjfncnt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rthunuzr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pwttgglf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2awssakhe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lkhqgnbb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wtmpcdxw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgopjfz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qfwplest.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pwvpcovg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hzvayaur.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zlhcspoh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2najwnqqc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqyttvea.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zoqizxqo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cgljzdwe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2inpdjokm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2buqldxdi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qgxferph.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jelcbvhi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjylylnj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mnqyqyio.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzodvdop.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tpnmxhsr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2chlbmagm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2poncgrqr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jutwrodc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dazrgdcc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnsgrtk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ekxyyobp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rhqxgxmx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jaxowqpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoaubwve.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mrsolrbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olaejtww.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ducltqtt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qalpynst.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqtwrdld.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qzxuqjeb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wmhtnpym.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hfjcrcxg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wvbbdkyt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cjzeznhv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mrmvjvwf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gdkfwdyb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fchqxlzv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nmbhbrng.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ncjdynyu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yfihbope.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nelcflvv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2cxgotkav.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jnxgebow.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zyrmpgnl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fqxwglox.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xwrzplaa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ywjdugue.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fljviqrg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gomaaqzs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vgtlmoak.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2swjphgza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lkkerlaw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fguttzzh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nztvxitj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vgyyidoz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsjqoabt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwrqjqdj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxazfrhb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yehtqbvd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nynbpfor.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vbejzfip.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pyabuybm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fhqqpazk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2iomxofcf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2afjvnfcm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhhddfpw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbvxjmi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2clpnmxyc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nciddure.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ipvckvwo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jmqubapp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gzvtougl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nmtstibj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cbawoysy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wrfbsshd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iucldjax.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcjdfrnl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xjnhuikz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lkobzpvn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fugunrfw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ywpfwpat.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cuvxcgsx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmnmqbh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yetdyqsa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlglwneu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bjsfdtqe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xhxqtydj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qahzazvp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ljtyxduo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nsjlxcnh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tilpvsxy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qbgnifei.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hpwrqmlw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bqhhrjfs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2doajaqmk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qxaahmau.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ppkqromj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hugzpqpp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2csozkjqv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ercmifdu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2edoizcqk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uizdkunq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rtulcwcy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zpuaytyl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ytisoxip.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjivtbgi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sxpeacpf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vflaquch.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cuvsirqw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yunsxybj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pxdpxykj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ouniihkd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tzgcbaya.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgigjayv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fvbbtzko.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fwrynmee.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bkwdovzr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vqymzhwk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nagmkylj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2grirzyet.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bgmplsrq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uabnwivt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zloisnhr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2srcswvqi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bxvciczz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nroazlwc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hlaleoub.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2eiuvzgvx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2axluersm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uxuijbuq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vunkqzts.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjaadqec.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pnhtkizp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tcdtcdzt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jtscgufp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qviudqhe.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zrrtbleg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gdgxkckh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eqnuftwb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cuevwdwa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gkyygriq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2uzyramiq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ekjzelfn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ntguajhk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2metjtiap.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fcauujzp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcavyvol.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aednpswn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xajsbjuq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtuezdh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxjmeaf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ngszswdz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fgptngqz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gxwixkvr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bdpundgx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tjxfxuma.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ugjtvayl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cgwybeda.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mvshkhak.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmggxsee.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rlhnqxdc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2frlyystl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ulicaiev.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2frfmzmds.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pozpezpj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2veqhcyai.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rcjdpwdh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vfeqpmfl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fmcorlss.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jircgiln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ridlbgkj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cwlnxurc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umgdmuxv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rziryjnq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wjgbkexd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hyduuzxy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gpjirjrf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2afcyofuh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbguyksb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pmydfibi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qlrzbjzq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufcdgkzs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qiaplwui.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ohbiabao.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lwpzhzuz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tgkvcful.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaujxduo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yfsxbyro.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ekinemcn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gkhutgxy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uedrniov.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxdhoull.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ffherqsd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mddprokw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ssmdsjcu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lawiusmi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqxgijgl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jhssskvr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqnuupqf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2niozzkji.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2chenkksj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrayqh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wdjivnbu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2enhitvcc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2aguykhas.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ruitxkxq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cxdikrve.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gybptgee.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2stulfrgu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kbmsadsf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yxabcvhg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mgrlgilg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fodryvbw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tlufzbop.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2spzxgizz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qkjybfbw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ibauzxgt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gfufdcos.html


<!-- 参考信息 -->