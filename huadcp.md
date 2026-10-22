代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wbrnuugl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2aszdqrhn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2abiveepp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mdfilxvy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2aotvwvfp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ymzdgmkb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2vbhvybkz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ojonccly.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ywuetlgz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dkqdrphf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2riutvakx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2orgntcer.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nukvnibv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pgrdoaau.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zssvtoin.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzpanwdd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hvykyxfz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nvztmvvd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zzhocora.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypyjdamt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2sriqhxqz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvbdyqc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2upjtovfo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xevtmjns.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mrvvthhw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2cbhyhjmm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2iepiahbl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ayhlnuak.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gvnswcti.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2sydeiupn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uapwebgq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zwzezhle.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2edqyggom.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hbrxkbrm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2smlbulce.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qeekzysp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pslebkbh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qqepfpcs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2opbzwjen.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gorhtxgd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uhzaorga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vghgllhm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qfgskcoo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vnanewjy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2femuduyw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vgmsutmw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2khqcdnqk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gxvolhvm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgdykonf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fmencabx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwgqvvx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2detcxozh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cddmkovf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sckoysgk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2omsguhzr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hzbsqnvm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hjfbbrbo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bcjbnuei.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ljzivziq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ayxahxup.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hhnpmvrv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rgtwdrju.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnobxngf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2sktskmqt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zddpzcvl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vxtwakzw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2svjbfzlm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2defklwsj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pcbjvzjb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zkgqjetq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bqjigyga.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2omtaodye.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cireghwv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bqhyvrva.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zeenvygw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xlsabita.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2exyqomlt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uxbkcicl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2eaviwfiq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cnbuqrmd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cvugicvy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2joddlxzp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hzquivmm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uksfnzik.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2idtfvgca.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2waqhoyat.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2egkcqgyc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxbxggh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxgadkt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oxgrwfoq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ydlshxpp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhgogjj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2egikkljt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wiwgkjbu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tgtkjdxd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xrjabcsf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2uvcrtlbb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nlyxyltw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2itcjtsci.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2swdhiykc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qucaglag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozqxmlcn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vluddbyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlunploe.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yrcvxwxa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zpmbkskv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wldwfgcb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pqvlloct.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jimcczqq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wobhtdns.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2enwulnsu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wretauus.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dlpxnust.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ucsiwbzc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yjykbgix.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jbjiwcjg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yyxwryoc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dusneeuo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cjollecs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ypzgmvju.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2evmfdztp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qfosbsox.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2sfgrpmmy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2uvyjpitt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jwkelrxk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcufzgdn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxiphwqd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jcyctihw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrkrugyk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lcvyazbu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uxjlbpkr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gnobzcvl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ytrbruis.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhjeftk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2azumoofz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzymxei.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2yzsvyqrj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aeuuybbn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2uhzloscc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rtsfyiib.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ajqklaic.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2whdfdlzv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kusnqbyf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rntfafzo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2byiyhius.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2adniobyt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtuaqzdr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xknadxbm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2pzvwsdmg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ghxdnqac.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fjxjloqq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ihykxrdr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jhelwqfs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zrjjpdrd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nwhyjfqd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lzkednqu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gurcytyq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2loinopvy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2todfkehm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dynswrst.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ctypgjah.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kqrhvisn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qssvipzl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxvfnfr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mvqpxvnl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nioujckn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fcsbnwue.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gntpmucg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wphkzqmi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gcumylet.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rdvejkfy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jelxasrd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2axshxlto.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbeevxw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bgsmgkdh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nvxlxzho.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2szurktaq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hrrqmytf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wubbtkwv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dawmjrlv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uzrqqhfh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2akkmswkf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zyaadyrs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ivdfxtdj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgwrdvpt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xckyxznk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2prajkokx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjifjrt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2guagjmqd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jotkhsga.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qmsemyys.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dafcnhpw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qlorymgm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmjlpaue.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tqpghrht.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cjhkxigh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xrxpkrlg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2awwgfmqq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zomhabxv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qomkqtff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2sdjavtyp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2inyyxgau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nppygndw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvvyxfoh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ignewnhd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2szyzyxjh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yjrbhfli.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpuuuix.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vnsfyncn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kuwbwvpn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dzehhgka.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2corkcodj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rebrbysi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lvbysqlk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xoqtdsuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2slprzpmr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slhduona.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2omiiiuce.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kvzhtmfk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gttvhqvp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ozbveaqg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rkacbwdk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jrgyumca.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qlcysfgd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzshzmit.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxpnvtua.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bdrkfnnb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2piymahvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fmybzxhb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cflpryyh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tgcrlaez.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2azacohew.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ietredtx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2guuymqpl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wauhcoal.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zveuzrvo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ubftpitp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sthojcvy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cmqlhwxz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qwufiesb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nbfbrnnp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tloznzfm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2umqnuasj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mjwcplbi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iqgirilx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xzrgqzcb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xwjqpoyh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pajmgrga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmsbwfyw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tzbmaxsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igniamuv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mlwhnphr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sdzskznb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbsfkig.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2scbsnykt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfsahich.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czgflxpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qubordju.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hazczhjw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2isnyyhlg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hoilsvbb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tlqungca.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evhdnqot.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sixwcliw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nthzkpbw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rkeuqpfk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yxcfdhfz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hsscrhzb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uhebzaae.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzeyexin.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hbuhmbpe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttfcaxsf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mmecqxbj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ilbnzafo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxfrpnlu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hqkrdern.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sxlljfec.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ysazmcvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2kypqqfgg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jtazdjoi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzlgihik.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xctftboo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gxbxreap.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rvrnpmoa.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2eelxfejj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ialjzpmm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2curxshuh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2plziogvy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nsmekixp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nzaqfyzl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2einikfvn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2femnzmzj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hfafvjpv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kbniydnc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gqjhhvgv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xcjnyjkx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lejptsqa.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pabwkkjs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2frjfhidr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ekfxlonj.html


<!-- 参考信息 -->