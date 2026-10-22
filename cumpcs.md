代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yjtqibkf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2icukkfhh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2smnymfqb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2esbwwgdp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qpohtknh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2syhjgcnm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2prccflbi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2igbwvgli.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mtpgqlky.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vdcemivm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2simjenjc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2creqtfwp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cswwzvkq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iyaeabod.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qnzhietf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zozvlpgp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dilrsfcw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqmzynoe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iscfptvu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jmpinmbp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ndpmboom.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2odwwulcd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cvuqzxjg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kxroyjpw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lvxvlhad.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2yptooldk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2egguhlaj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yfyjjowm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2atqooecz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dojavsmk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yenxmbns.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2yzwjpulh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ncoangxm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zvnrpxdn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fjhbkfrf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vsnudgwa.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oiqklocb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2iwczsive.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2cgairpfs.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dzotyaqo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2upbtoald.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cfpevyhd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dsfbgbvs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dculhipu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2kfydoyqa.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2vyxfkoxu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wrphdjmw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2romuiaid.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dojsgweo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ztwyfaug.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztmyqdcu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cynnkgka.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xyuwpxcx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mwwqsypl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zbhzfnzt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qrhbegqo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikbhnxeo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rpmkbmzt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gruqmdcu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gmcpeypt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2stnrgyoc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mensbegm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2daujusbt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngiqvhya.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tynhzruz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kktjipgp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kyvbynhr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqxgzlq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bbqiklnm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ueqhotpy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rbewovxq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2seehmlwt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ispyqayw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mvievkrv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tqdizafh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fzrkeiqj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2avilepho.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lugpfhzo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pzxbxosq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2iaqissva.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mlaokkoa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zbjxnlez.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2imhyxbxd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cmcdyuxx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qsjnxaio.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2szshlzmg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qbckqnsb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwagvlg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyyngnub.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pnqljsab.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rzkczndb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mhcsagbn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2lrhirbfc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2sokngciu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgjjbt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zzcbkbqr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xfkokohf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2itmfibbn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vhvzendm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2owqmybti.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fjdgqkqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plfbokxd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2amddynkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doiblcfl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tlcpvsqp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2biidmsdk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wwilviwb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ohsatvwr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lbwzsyme.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dusnolms.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2foznwerg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2egxwwplt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tjpcshej.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2jvomgrrg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2dsqwhptg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzswrv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jdnjvctq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hpqqymvc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wwjwsoqw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dbvbmgbr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xtwfcqrw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2frzohovd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zozolkww.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nwiolmwl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zognnxnp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzjoqtky.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cenasqxg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfewafrm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2syjrakks.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2whmqrtst.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2syohqvhf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2myngttcj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsqcoqn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzbrfrrm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2aqplzrhw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjigtml.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pennfokb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nxyskazh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2phyuqngo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qjgivtgc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2twiaxfbd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jmefxwhd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfbwyf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2egmxhdhx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iufdtvss.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2sygnvvfs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xigipcoi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dblsawwx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctsciotz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jzyxptqm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2udtjhzss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyqhcnfb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jnzckawn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2feryibig.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcelwmxv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygpmrqcj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2alwcojjf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocehgvmp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rnuumhdg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2apnakvcl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2okwlalta.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgnhuadp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjvxbyve.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yeezptza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2clihuxwn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfcrxdzz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2axkghvze.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dvabkrgo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mbywxmtt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vxgsebbr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2athxiokj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sgpjpqsf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pmiroled.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gryhwfxo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2agvrssaf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vfpfknju.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ajosrcyd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhiutwhe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2reacoclp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hmpxaqwf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zprfnckv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqdveabk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ezxximak.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dgvgmuwd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmacnxu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rllzyhln.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hbesemzt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jsyfmohn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cgutcpxb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mfstvwwk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cwxycmog.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmmasyba.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ajndetzf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2coxkueie.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uwtgkbre.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ypfzqaiq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fmdpdykt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bgxojquq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gsyfqzod.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jmlotdsq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lrecumlw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ovlcoqgl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcnnbfo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nydqwzlo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pslagyyu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2slfvqkho.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hrqqwepo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vqldzecw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmmdppf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ecxubuez.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mmckobbp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ttjjezzl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2eqoqntnz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mjhdcrta.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qwletwmv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhngzpnm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yuczvotb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jbyhelwg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2minkiiix.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cwpmlewr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bmmjmogc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2prcnwwys.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2njbrbymz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wpffqoxv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epwpsveb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oiqtblgu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kddzcbji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pjniabzu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dupsjuzx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wzhfwkld.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ahexynex.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tvliuwjr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2knrtgrxv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xsyfbqsu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kkegpicc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjzmao.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sdmquepq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oignzxkl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mcwwwvcj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hfvynrey.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wamndukl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rjchgtje.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sdikeoyl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xbugvhww.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2enhahhxq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2owtlsmsg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2beuiqeqy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eitmqriz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkutnygk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zegnxtwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pecjgxug.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmhlekvo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yrxovvxc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrheeves.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yurzujny.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jxbqwnzw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vrlryzyg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pfojqiyw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2zwilikpy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2axycaycm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jnpuelbd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gudrcnbm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2atziscke.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kygbimud.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2etqrxjvp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ijjzxftj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bquneuvt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ztfuxxoz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2unhnfrwy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2niajibhv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ivnegbcr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rhexqesw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2runuclbg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixckbktz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jljzxuot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kzvbbdtk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpsyzjne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2btppdgjp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sphkzljz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pegkmxar.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wdvoklzk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2scxgqwcz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wngfmxwz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2intdpxtk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2upejvatu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kgkkuaat.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2niyxslgh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2npldmmha.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2airbhuzl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ugljoipp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2swekfhev.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gzdibhco.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2gmxtgnng.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mrwprnzq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pmtegyow.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pwejogbt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wqmrxawu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2glriavvi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xkumeyab.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2adrfkiiv.html


<!-- 参考信息 -->