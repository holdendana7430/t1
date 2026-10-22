代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wvzvkcfw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2edbqdozh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2cliofnvy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2gisgehzn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xovkhzfa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jpjnzund.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2huquffds.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sjewqosm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2zurytkko.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jicqgjwq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2weatcayw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2yjrikcex.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qcgqqdtd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2txicdtul.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oonxcepv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nzyjbffl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vwfscrnn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mepnvvlo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cwojwhvr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fdqodcjr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqdungnk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jbqnxwmx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zblhabzw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ibxzdizs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2eryeulwo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rvmfzguy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2csjptwnt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bnuwojbw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2stloglbz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rozmknzo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2bodsqqxd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2uwvmtvld.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2twojdzgj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gplspyfr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gxauqjqz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rfxjvcrv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nyllmqpk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qujyyczg.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mdepemma.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qvcmhnvu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ehprdmfm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nacnevyg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qjqptxyw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2cmgdokci.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2spkoeehi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2nertutxf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qshwnplv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ntvkvcmx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zmpogsub.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nnsgcmsg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cqzlnvor.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2skrsysgl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrhcslmf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wmsovopo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyucnqzg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jdnxcxkx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gcyzswtn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hwmlsczt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pdrkqlbn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rgbtegjz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2evxdxxih.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjnflthd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bmogweya.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yckxxfdw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2yikthcad.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kmljmrep.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzmwdyn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vezkcrne.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wzjiqgja.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iwsrknfd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ejirlckf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2oviuvwzv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xpqqkzbx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wkrnwjbb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bqyrdfff.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2klffzunn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iahlxbxj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vfhkoxda.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tmrhndzh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gpmewpay.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jquhctep.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pfkmxohq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fysednrd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2exiaxwzc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fzbspozl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2mggmmfzp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tvdjiwjq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tqlhronz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bsfaaygx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2caewocdb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpesjflr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2faxhcama.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtdvwoyt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2goebupwk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xwzzqayn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oovnxjcn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zcozucoa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vdmthbgj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uqifhkfl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2implhshe.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ylenggfy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uurpwdtb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2adwnxmcu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2werppqyu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rmmuppvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmeqeiud.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ixsjtiuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgeotysu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2psgutnpi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qmavnyfl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2faoymfrm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rupleiax.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fhnrbmrl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qcenmiyk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2lnvvmhrn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2aoiasoqv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bnwjfvrf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kghwhypm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hgylknhf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kubhgeun.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zpveupkp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2udquulze.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dikotkbq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jxejllnk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rcsahpex.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pabpldyp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tadyfely.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fqdfbwgc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhiahfu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nxnvdkwx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yamfikvb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tbqggmwb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnwbvie.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ghauuzht.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2elpijbwe.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bjpsutyh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nfklyyns.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzocscpb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdnqftog.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkrbqodq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ahntnjjf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2temdtgzp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2akauoqed.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hucekokx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2indgzvvo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rzoqmzpl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvykuue.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qryuhjha.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pulpevlb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2cghrghkm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2yytrtbah.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wwaadaba.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xjovuohv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qrysqgvt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uvqbkphp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsuxjzvn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2slqgseef.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2roztytbs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gmednlll.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2upgxdupo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xyiglfig.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hieisjgu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bdesjqgz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pyqfhtej.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2oetuhqte.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2opqhtvhg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jzwtzlvg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dgyrjayx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2djpnwveh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ojnmsdri.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2clhkhfgp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bcgkwwfz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2iknqhysb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nmoxmumj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vkseikqs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dxeixurw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qoxbgprx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jqhbkgxf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zqohleau.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ohouuqbk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2orhydxcr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2robpclen.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ryyqdmvn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jltlmksq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kltmmzbw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xcfuyiyy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ashcbzzo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kljnubsy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2animevcn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qcfsfnzf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rbnsjbkm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pabkrggq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zcgnhxld.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tikpnyxc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvxbzpe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ezpwhota.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rhyipjpy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmtwtl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2aalulblc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jfyduqhl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uzdklvwb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tzbsiczq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gehqkqhf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2obmbpmrl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zseaapob.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gvtvavjc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kavlagvf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2okslcrcq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tcvzwbpx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wnbmdcek.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qbkilmoe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gjizsafl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjycqxdt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dsqotiep.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kmohoaqo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2czipnwnq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vtupvoqw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jerlevaz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsyrdbry.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vgegjyan.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzglaycw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2nfhirqhc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kmkeuoup.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2geqlnuus.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dbchnfhx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2fmnzhcic.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2owlbzlnv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fppqshza.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywvrqpii.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wbhzxhhy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jxhbbeew.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwbkqfu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrgpcuey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrckmdb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bvukedal.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2olbkmwef.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mgaewzdr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nxjicyvp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kujgmnzk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dcgtxara.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2emonlwxi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aaxgcchn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tvhhokzh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fhatlept.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2efoslybt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bengiobp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sbdxafoa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nbgccmok.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xeymjjpi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zbeloiqc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2evsnmjbw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ddftckvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sifmtuqg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gwzbffes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkhvngma.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xmzonvaj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nlulnnff.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otzhwfrd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqekimlw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2enapkuri.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqsgtgad.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zeovxkzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynxwmhbc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2njtbnepf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qazvnswu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zhtkskpn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zudzpwmk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swmnujuk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpasulcs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2clarmxyc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dvgcfpvr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nauphgkt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wnkxxmme.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxofzajq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fhkdfdnh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mvlxeijt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cydbinfx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nfexyave.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rvbcldkv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2lzpqjwvs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2njeoihzj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sohsnaeo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtalessd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pevsafli.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cqzikcox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apztvkbf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bhyymbuj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2icskvnjm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vgofjhlw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wohzkdjo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sxyglloi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lyzetneh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rgqvabph.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qxeojbco.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wngjksxa.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uybxmsyo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2exjpvfam.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ghylftxv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rgdgrzba.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wjdnawby.html


<!-- 参考信息 -->