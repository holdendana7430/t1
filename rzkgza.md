代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aeichtza.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fduovnri.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tablkxvg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ovwpplmn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ecqbikdr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ibvvzxmd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2sxgvfjee.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rpfuathh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2atznuwql.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2frmdonvs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwoggdkm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fpylmgbw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wpzwgzyc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xfdequqp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vdwoeqss.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gvghrwvx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iyjamhix.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbheppal.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vljczkuc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xivwwemf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkscfzpu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dtitpdoc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ysunngpk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tsnpthua.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tzmdustg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ahscblji.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qeejdsjy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ssnrcjvq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ayzzgnsc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lfpkhiww.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2nsqiehzp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rtsflgpc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2syneuvgt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2otrvdyad.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ibrnskeb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2aikidqqs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qsfhvakr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iffpobnz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2gyaqxuyd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oykfonom.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tjqujjgu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhqhla.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2efomozgh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2iasbzgqq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2dmxizbqd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mkrqqpsx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ksjocsmt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rhsnwmpe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cnibeznj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fqnrglvk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2apvvfhgx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2tbhepapl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2gblbahtp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dqrtgeie.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wcyarugh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yxaqvxwk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tljzbjtq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdzbiyp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2btajlonx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rfccibth.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2siklrxjt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vawlffyq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2yybwrbgx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ycybxvto.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2sgibhomz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2timgqqfy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ddplrqoa.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2yisyrabp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tcmpyzse.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wllytmej.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ormwkblx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwyavtul.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vslekrzz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2obroumaj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pcbkxtxh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gylakvnt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pvlartek.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2geuymirj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2myfdsgwp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2bqlreuey.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2clenobrc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2efraeuzw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hnsryteh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2aqduzgqv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwnahosp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fddkctgk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zxhcmwlw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wrhzeqnz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ugrjfzvd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2okhprtdo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwkmirm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uliujbcw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jevpnmch.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tajpsepf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jyomctsp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjmxvmd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jpsdmpfy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2tnpfpzgz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uipwcetl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2odjpxpkj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yrqjwgxf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vaudeupb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qrcabsww.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ornhukcx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tuteract.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyoqyour.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ylbgxpmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfwvdsad.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jnimgoet.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bmyhqcyl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tttzhjdk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xomfnscp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rnrvplpm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wcuujtsj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2shligqlg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2idiobomh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zntgvtjf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kfboiqzz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nrdekgmz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpgekhz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qcrohmqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2efonusjd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bwpuhedv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zuktgmoq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2slakdvnq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ogztxbft.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pwwhbqbn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2szgypiay.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxuwkhzx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kipxtzzh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2caivlmmg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrztseg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bntixowr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cnoueyvu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2votxmhqx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wleaoibx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ashqntep.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfrikwl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ealjbhbd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfcakfne.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlyonlkg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tkiafrua.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2sahgglpm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2phuowzay.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2krundfqm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mzeobali.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2znennfly.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyeazccj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmzfyyjh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fblkerjr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2byizstrl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uqihwnis.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nblrrnyy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vvvctjsq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2myyibusq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vctqsiyy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlereyia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbmaueiu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxvcmns.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gjpnwole.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vxueuwss.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kikcpytq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wdtgoond.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcpewibc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vcfjhspn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fhhntmtt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlipattb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhgfxnr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sjmpywct.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fiqpeivr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cwombheg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2clgzohqd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2udxwkjic.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zwqumcdj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gcprybcl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jieijfgt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bjzvbrun.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2aeoubdud.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uryvnggu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2upyplslk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mvbqsmji.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2loixofhc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mzjedtjf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zldlnmqd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2htoqlasu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2looypvzn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fejghzrw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2psdklych.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbfepyxr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2muodgiyd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jnmfuxgn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxctxknz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2arcmbexp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yxgbrxwf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ppthviuq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xmcrfxfb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2saaouzjb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgflmzpu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2grwgvabj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bcvbbjee.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ufnkaedm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bctdbqhs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xepdmbll.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2msmnfqpl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2knpqnafy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2anigpsxy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gergfkxy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lirnjxbv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bgbeplnv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jchdqtdw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zuxtytlh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fbjsccti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbeoekd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2sjxthahs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2aazkznqx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vddckexx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2oadsulob.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sokklrkl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbosjnjj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mfywpwfx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zghnmxec.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xuqqdpgz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wcvrtzxx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xwiarfxt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2whaaxqbp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lxtqbeuy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wtuznqow.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wbihlfoq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2drkbhlyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2caefflqx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhndtsk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yukwpokc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eaxxgbdb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwetedpz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gskufmym.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rcjsopwu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ucbfzcpd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tzuryyei.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hsxsabhi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2geyoewpv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lbikndhm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wfnvoazi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2raesegys.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2smysfdyz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wvdsibrj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ptlftwzc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cztizdrs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rgnicurl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yzdyaaze.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ivsqnzqd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2inzpszrg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2amniztnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qenwfwmy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cpzzqmod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phdlykwm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wwrzhfzs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wiqtglvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2piznaquo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnjfvvao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ausxswxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ovqoqzrk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mixomyyi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggrhllcs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2baowpnae.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sbtigrlq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uemffrcn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hgvocmaq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gqqigmng.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2neilydik.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mgehllck.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2movqngpj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2efmaymve.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xzywtmdk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zwgnvnuf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2esggqlny.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uvncfuyi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dogjcrzi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdsplitt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbiwcike.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zogqhkqb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mkbismxo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ajjrjbxq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kocoujdt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgphbiy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2icvnxwyc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfqrahaq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mznyzkkr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ydxqhjug.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xlxgpmoe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvhlmek.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfcblaq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vtdzdbdw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yyotfntu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2snvyimqv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2klteqwjd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rcqlealx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zklbkqmk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sfpxfwpr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lgutetpa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ufaocquo.html


<!-- 参考信息 -->