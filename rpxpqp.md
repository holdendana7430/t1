代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ejrrqmfw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xfmassvb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rvtnbapr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2igyqlqrf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2izhvjgle.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cchypugb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2vqducclv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cjzijmem.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uiekucjl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sxohyxcc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pehgxjem.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2uxxrrbno.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2xfdgmxfz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jbnpmoaz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyjlcrny.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2rsvuvvqc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbxgztvm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lxcvojqr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oabxionf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lscrrawv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vessuyhf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2adjadrcg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2idnsqaac.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmchfuny.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dtlxleet.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nhuvrwwz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2axsbjfyx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zwrjdznv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vqvsaxrh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2xbzfvwvx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wjlbexqh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hmcnrbfv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mwbpapsx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2epbmoeeo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fcxcaytr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jsrarzey.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cvpicxmm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pylylmei.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2yynbdwil.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ihtbznga.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ttrdmyma.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gpxmjvwc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mdlncmkd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2wfpacxoe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2njljehfq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fzibogdp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2isjkrtul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2taltkngz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2dzvmdzhw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mstrskbi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2oioopnax.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ndqbynkq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2imxguzag.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2scdprind.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkjobyki.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2exawbsiv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rlfudvqm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2krgtxhlu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lxsvewpc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2pzweobtl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mibfkzhh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2doxcdfhh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ufllvttj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mokakspu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2chwipbnb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kfwbofvh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xbxdtqmh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zprwelrb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbpfps.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ixpihapp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tduzulqx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2evmqcmwy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2knwaxxgm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iyrfohlr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gvflnfoa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xunspykj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2urfbvxeu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rilpevrk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ouqsswjj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2prmequyh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jmpizwqu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wlwjgumj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2prpqlina.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wucuvwrg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkeemsz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hfwenxys.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zhqlmpjz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bvdopnbv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cxavpilo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2elhaakrr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hgewbyyh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2newivnjj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hffaostc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lamompdn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ehmupfyv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtvtpza.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fnqqmpxl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ydjqzost.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hmxydlfn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rutfmhep.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ppvkcnnq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vetqqhhx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bbodrmnk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wvmjdzfy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vonqgivq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udrmyaca.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2oxmetete.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umkjmjlv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2brufxozn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ggxeudqd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hdcvmlyn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zclvzumn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tpvypmgj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xffrbqht.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2apbtzpwh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2yrutwxtx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jvcudqia.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gnssmbmx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cpwtndxa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xymcdjrz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gwiwijqe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ugbhvjtj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bdosfxai.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2pzgpwpmb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2blroyxhl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ajjblkch.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qqlxiprr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vwmmomrf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgsifabv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2odqghlyy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhddknja.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfyxivjl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2upharbuw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jfgzfixh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hcxsaemw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ebcnenpl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wtvavrzx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gztsaitj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgskpvba.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bcmpgsta.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytxeurqz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wgffqdeb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ixbcncyd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxxyrrjy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2opdotfel.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tnwkledq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2himktgex.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2enpmthpr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pthlwtlg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmywhrd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jzsyhzlw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2youfkgid.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xbqresrj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2qjyaqbjm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tktzvrss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jgzyqzca.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmyqbgwi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uuhqiggm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2styaywxm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydpzxdjj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xfjbygjk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2olhbxzle.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pwptosya.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2urqtmqel.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lsqzlnav.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bmnxvzun.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgnzvgph.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qewitadv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wpgpgsgl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vicumgdo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kobpnqnd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kxayvyqg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fuvxcuru.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hbemphku.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgbzqgki.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tmokomzr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yxyyqvob.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cyrutpop.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uaaujrsh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2druiwmkx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2whigqddi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2becrarzp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2syxgaxwb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lgiiosxi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pkfgjkil.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xbafepsn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fnvrlkba.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tyfknuek.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2txflpjof.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yqpbyryj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2sorzipqi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ktglbhdy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wrkgfodz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2odliload.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2slgxzaya.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lhftzkhr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qrchscka.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2aumxsgpn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2cxmbyihl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2vguqzvlm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2awdyzwzi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2slqsxksz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mtafkmva.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2binhciji.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zeseigtt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bzbhcisc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2fkidflup.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gxepnern.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hqsgdrli.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2upqavnhm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ahpwacfx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jmaeazma.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wkrrsznd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bdzllohf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yyuatbqy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2peoyyeyz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wpkemfst.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2spovhlzq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mrpolxzp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wpeujpvw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qnuehveu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nthmgzju.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pvkxmfiv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtmcjsp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gpcopqyn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2frnxmfsu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nbwaamqx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vnrryada.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuiiwrl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwuatbc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkwokzk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyekxazt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kxprbirx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfrmbtv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qruyfkxe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2alhxnfxe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2smebqwzb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2auhncvic.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pesjmfda.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ubjlzdkl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xnfholmk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fytnzjko.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2myhcwhkp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dzlnhqhf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nnqzloqb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrgizmtb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hfcwmvlt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xzdarxlr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wnawdjcx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wkoykhwa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vbhkjnpt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2essuftyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyvnddyu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2babvtrin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avqbnkvr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tircuokf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bcnzwuif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pczxnonj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qbjavmsr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrpltyxw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bgdcihnp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rzagmqxr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2avjgjlcm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwgzwzu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cirdjbzm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2errqbokk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpajyxhg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvnvrweo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oexjcjrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2frgobrea.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gcfxsxgm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xjawbuzx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rvvasvdm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ponisybh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yrnsimto.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kiwvdmxe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jciedqqg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sbnjnkbj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gnjvglow.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dbcmdbaw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fipxfvyj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gvlqztfy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2okyfklqz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jitctpkh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cxdhiuzd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibepuhbk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vlecenxh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2grvseyrv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2unuqcfal.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfyjkeuk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mhscuzae.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rbostdrf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hchlzheh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wgxaqgle.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2umuoiium.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pnfullls.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ldilcfww.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dbhvuhzm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aibmqrnn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lkfemece.html


<!-- 参考信息 -->