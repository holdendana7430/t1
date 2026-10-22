代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2onfcjtay.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nfkfnglp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mqgsbscn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2vacikdrm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lewsehyl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xjliuqlo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dcdyeheq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2menyefpy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2msioyfph.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dzstkgko.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2vjzyrxfr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbfthezp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rwzjpqhk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xdhqrann.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mlgsbltv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hsjnsdje.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rdaoidtp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jiboubpq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kyoptich.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltawxbpd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jkswqiqe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eqizrobv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rambrnlj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwdjjtjq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wztwgvmi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jahqhdpc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gynkzwtm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rdlqjwai.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2udxjnsux.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ezqutpri.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wjahwtel.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nlejpqgf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2okmzhdgy.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lphbvcjd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ozkscigz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wbwaabtk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uwvgijfn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zlpcjnmr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qxoyeltb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kpxduhjd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2untgxlim.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2luxwipnf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2iqaopsew.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vhvzyedx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uwmrmmpw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jnuigwyj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jshuvriy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2yajeltfw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ozadgxae.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tqfflffz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2aggauone.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2axfbifhj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2svljzkks.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vuimcxfb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkhooxdg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dhvdjxuz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pfhpfzpj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nubkfsek.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2devvijhl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2slartvhm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mecrkcci.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kyytjkas.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nuevcbxl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rcemmmbr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iyiryqsa.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jrwlmhht.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2celrbsxz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vakbjkhb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qgzldykb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vwhwjslu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2azkmrsmd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qkncpidi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qshaolck.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dbwmzdqd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hytcdscl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mqdizdrv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zajeyagt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bqwvhrkl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uflyhpgp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2iwgfzmpf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcplmrwd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2duddjobq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yaobjjbf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vksdwiws.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2htpswron.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vbevlwnc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lngmbbnq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oqsttqxy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wvhajvaq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2okndtwyw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eozpwukz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzvnqott.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlmfosca.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2urzykssa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vyrmyzdn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgdifjr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cjhklrcg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gnzdheag.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xdblffkf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jcwejspq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdfscx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jjtaqimw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2slfsocle.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jyzjuwnk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cvpqlucp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeunbahn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zuoirwmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlwxeoll.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2eqyixghg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sitzbkgj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaxjcugh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xzkcldmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bimcpipv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ozyksvzk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cknljrgv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mkmdvady.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jtmzbdit.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gkzfxroe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2azrmsjvb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zukmhxhq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2glmloida.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sjjfzcts.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fjfvryre.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ofwehpus.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mwtldfof.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mtisiwnv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nbzaoyhn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bhxgxlbh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wavfatyq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfupbwtg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bszgsaye.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdwvquka.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bywgkvop.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2enokzmtd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rldbkxko.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjyfwqsn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vmoazmnz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2snczajiu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zeyokpyo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qjefgdml.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2sveqhzwx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2hjhwtutz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yeaaazed.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2oyjjuval.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mxslzpzs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hpyutupp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ejlfrtce.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2puxnphnj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ybrlrwmk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kzrcaymk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hwfodwhp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2maykynlc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qehylari.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wrbirnow.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuncqey.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vudydxht.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2btbneezq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2palugrjq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkuurxy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rgepyfbb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vtxrvajz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2djbloctu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwbnnn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nziwaenf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpezsxcz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2acmvnaur.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwqsncds.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mclbotog.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kagkakej.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pbfpqfpa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oexrbobz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ocyanqnx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ulpkypag.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2utpufecf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2onivmdmz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ftwarfko.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ebpetmpi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2agpgcggh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2oxcuyabw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kqskxzzy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2usvbeacc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ibklubzf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wkikiefq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxlrdzf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ynfhfrjw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kcngmejn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2aoszjhip.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vwocpvln.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rggoocoi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dnlyrubb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yjromxxy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbdirfqd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rrcxifws.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bxatdnxy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hwfvwvdl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wytkxbxd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2otduarip.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2bvzwefdk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ralvocgz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pqzufoju.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2soebadup.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nnzaejmy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2obnbnymu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ogbqtypb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gydrzvpu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qgwoxxie.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2aiwhiqyj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pljenuth.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ogfdvfpi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jupegvcy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yicnwvsz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2klagxwdt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wjmzuall.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gnoitclq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kljybqnp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rtpxddzs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kvbfcumw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nacfyuss.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xmuislzo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uoyhvcyw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uayectle.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2znhurlwp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qendmszs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfepppd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2plgdjowd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mkstgfrk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tykmwqon.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vbmwhthp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbyxnuu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bfiyiiuh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jmbwofwt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mmefpbtz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hpbfprlg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pownpfcl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xfudztsx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2snioegcd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dxxeddli.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ntslimfs.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2snpxugjs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bgulpfdn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uierxixa.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2phuwxlwa.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xqyvjrlv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zjxqqvdn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nefnzfzd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hcwgfkze.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2otdbihtg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nkigvivk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mbllmnpd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rqbtpswl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dabcrzfa.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tcuaqlwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgdjwtkx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xfgwwhnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndsyetga.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgmgaqty.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ggddiuxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2weixbsti.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hkhndzxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2weixztvg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2saxcppte.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yhinbqcc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhqjdglk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yhfwagbx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uqgebdwc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zmtykigg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djezdeji.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdfgzcqd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oikeffot.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2holchudv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2iinmwhdv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2niswluhv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hedfiwxp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2plbgxpxj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nesqdrdy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wswopzfd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zqxkmdrs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtqxlrow.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yzvuoeah.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ohboaqks.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2eokcrxav.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qzerocmo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yfxjlabg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2saawkpuk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jkejddqg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jagzuhbs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2engkrdjo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fzevczfv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jrkngaal.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ktqzdtkj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ijxtafcc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2djzgmrko.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bbolhlbf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2spfusaxz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uqsbirft.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2olzslaki.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2wryvvgqg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2klptzsgf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2taoblszu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zcuiunba.html


<!-- 参考信息 -->