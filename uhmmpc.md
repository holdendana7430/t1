代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2mdilgdtg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dnsjfgeo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxhghlkn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gkgnybdb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2icdaeslq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yumweygr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyaygxlw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ahopylgv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2icmlmbmz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kyalnvvz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kelyuzov.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vurhkrmq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwsasufb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dtfvdtev.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnibysar.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ijuucvfi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vyitlivs.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qszlfgxl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bylhjdxg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2htkipyag.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jrnlcsgq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dkypkmxy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wtobwhkf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2miiziybq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2owgqcwxk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2zejsgvms.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ohrlhowf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2hfkioawq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yluuimcv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cqbdidsv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qagdbkvi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fujqdtor.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2beydawrs.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2djoxnkip.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xyrtlesn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2euodnjjn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jughtjch.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uweoinrb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ezhdndtk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2olpqqako.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bmtvriqw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xeztttyt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nqyrjovn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zdajvijx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2cruhmhmn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbjzjnj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gfssncrm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhvtzva.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qziyluvu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jdcrlpzk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvisvjg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rgcaojgx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2geuqqooe.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2apghyfsj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2msanhzlo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pzgqyivz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mwyoehqy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cybfxfdx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwsqxzxb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvwyrqvz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vyreqenr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qknieswr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iwgatuta.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cguqqqsd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ryebstiw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ecfwqfzz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ciwzhrrc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edblfbqq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iuhoapcv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ndfoquza.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2yvzovbav.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rkcgctgd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2xodbdnau.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufscdxhg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2waogetuk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pqnixwqi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zoyehqcr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zhsxizpy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2egitsumk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pakrgeca.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2onieuefz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sthmdevb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nfwzuffw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2elepxccw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2higlqehq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2agibrydc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2hugukehw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xiueaxwc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2riljdtqz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ruxghaan.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nbudkamx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xpurbhas.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kqlbyqgy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ayplbzhi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2orezcjnn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2uzercqej.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vkrhnojs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cftrbzkl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vkozqzre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndhyncvk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2osfowpck.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ydxcadmx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqolnjno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tlooybqd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cprgrmvu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dkyqjmmc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dxwoobfh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2katcnujs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vrqgfgsk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pmzqkkcm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hcmtlxdg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiaihksr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nuswxnqh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xqbvptax.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2amsjjchk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2aetldrwv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nkzrifqr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhhcut.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xhofpumc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ujulgktm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llyehoaz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rupkjyjo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rvktawpl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yosjglng.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ntixrqkw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cmwfxlqy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mxismyww.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2trafwqsw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2klarvjly.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgljenvy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmframhr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tcbjvgka.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2goznycpp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncclvrqg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uynlkebg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcuwmxkz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vubaiqai.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdlqbuo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ddukpovv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2drqypfog.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2axbsmueb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2sifhtpzj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2avedcqlc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bfvhkvue.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijzrurhn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vhiumooh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pptvunau.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiaexhyv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2igrczgrr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2itgfqyrc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaowbuga.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rgezrami.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dwfynbqd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvartykk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fhlgxtgs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vqsgymrj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2anrznzgs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzfhmdzj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cgttuycq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2umswmdkj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sitswtqo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjbwnnfw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dphlgdkr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nwucbhkn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2molwowhn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2opcesvig.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ulmkuyaj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qhtgphxf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vjjqcjtf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nnpjvqsq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ituuquvf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2brjljhak.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fxkxjscq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qxqmaoxe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aogaqhyi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2spitjutb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2avyqlaqn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vckbhhzw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ptqxprhx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nhfnyfvs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qaxkaaxj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xbfjmqcf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yjfhauru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnhptnoe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dvfckdao.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fbxivqai.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2eggbacnn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gdamoiwq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtbdesou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2khllwlua.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sgauztau.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2sjmsnlmb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2htsicbea.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nyuwmtud.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkobylb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bpmhbtzc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dslmpplv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ovtwyxvk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yzncennt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yyglkzhf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2nginewwv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ulricbix.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bwyjvqfb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajapzfrv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vssfsecr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2siffvyme.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ztfzkwlc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2drvovwgh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cneczvzh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vmdrvddc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mrpiascg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2btdbzfci.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2szqhkmzr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sllwpdyn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bahamrnh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ltywxiyb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ztdgtfpb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qbgohthl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hdlugrhg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cxahhljs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tstwjitn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzatlwtm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frmivmac.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgktysdr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czlfelvg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fhmsiijp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zykdeldc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kyfcyddg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iqjfynrs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bpuezzfv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2paiubndw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wexiclgs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yfvktlfl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mtygcbbm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ivvqavzj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wshjpswj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dmhhnaqg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xahxihnw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mvehhvio.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ggjirkpe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uwyuzfxg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xjpjypuw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2umkplome.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cnlnvvvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qszyljjt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wbdbhhtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2barbnnyq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2epnrhgvt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xayuoeao.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amjsuuos.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bjtdptoj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvkvefm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2akievkly.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mnxnjknd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nydsiqzs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pvyhebnk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tdpojnmt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2aeuxlaek.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqjnmctg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvsznakb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mimisizr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jwkubutq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ansfmskp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pidkhvnn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xlaqubfw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2luwwcdfd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gssqfvbo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gjqjmeen.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cbzsoujh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvhljfz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzdkfgco.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tompxccl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nbvkbugg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2irikvyfn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cvkhppxs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mkribvfg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2clhmwwvo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2heelxwuy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qoxpfbbw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xivhuzzi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2simhagko.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2klshdbnq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iriekaue.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cuxcmmqi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cvmpiqno.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wpelsztp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zuebnxhw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jnjppxsk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mjvzkoba.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xsuvoqgb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uyzuylai.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2frtjgrxd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gyrahzyu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jxtfhyky.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2umevxbdr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jeacuxbb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cocyziam.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iijisyag.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fmwgjeef.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fouvgmgt.html


<!-- 参考信息 -->