代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2stuqhlwd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2teqfolgp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2muwqtdkp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tfdsnwfp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bexztoqd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ynpdtygk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dzhonrsl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubzkeugm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2whymxznw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2clmvvaxc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkfggqrw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gfptpgot.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fudbogkk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2inetmuyw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2whhilgxh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hzujwyri.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yrrhkkya.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2behsojqu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwrbtomp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tyrkvuyz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2aclexaje.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2plsdxkbf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fiojwvou.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lzwurahd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kljowisi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2acrjytzf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2tgpmvowr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2utdnquwh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vhjntwya.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2lrtxzhmb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kjqwiwzh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kckeoqjg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nzopxyde.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cownbsck.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cejeooxl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bwybnnry.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iekmbnhg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fqeduksm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2szyidtee.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hlupmrnw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2tpldujjp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jlrxlsrn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2emnojdto.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vqeugxcj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qjlquukg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xzjfftgx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xjyywzoq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hzidumud.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lzgncmrq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eiipgaxb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bgtvykvp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pvobzyrs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xphaxpij.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhvkgia.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2akmmympr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sniolicr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2abxycubt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zymbvhib.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jwxgjwmp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qvvbhull.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2vormmgyq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zhqnomjd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akinolgz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uhdbjtlg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2kmarnrhh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dblljyys.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2urarmfxv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vuimnikl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lfeonoxi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lcgksbgx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wvmydjuv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rcvvcwgc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lgbgxcsj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gywilrwe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2boalwhct.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2bbvrcidb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2sdcrhjcb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ldksxdxg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2svctmydy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ifjfezyc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jgpaaxop.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jemnrkqm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2skgbisbj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xrzbeygh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vopglkjz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmeicpzz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2btclwvai.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fyzjqlor.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pwswaodh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxtuexus.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ddpmcadp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2makncfwo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2gwtzqkhf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vdirrwvp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxevnp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tomqujau.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2iuhxabyd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2buaazfxb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vbelpgea.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fpoljwsk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhdidxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2diabgqyw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jedamyuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzwnuttd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mnxwfwlw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pfsjftlk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvyrtyp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2obzuooid.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qdmgkqdo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bemdjout.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ylmqoosi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rsqkqfxw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bakhccmz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xojxpaqb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2luosqeff.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qysxlsiz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mpbekusj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vmmmyuiy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fhuqdwfg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2pzanyhwu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ivztbchs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uvosshmm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kmizlpdj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fkmjpcke.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2azphmetd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pbngcqfn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uisairhi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2roxzoebp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qyrkvdvr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yimdlpbf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mgjgoxhu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqqpctuc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gttvmnhk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyarbenn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eeyfssip.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nahlcolm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2eotdnvdw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvklhfrp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qiqdfzpe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2axxnojnc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gguphmyu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2llnobrzc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqsxpmy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oysvzukl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vafeapgb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjlxsfd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rrjffdjd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2iwpnkjvo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lbsrtfxa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2agbuvaai.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2oeggwtpl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxpjbpee.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aivhjckw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qhskvcub.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2sdhknmeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2wallxrpn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hxntxbep.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjmpurxo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ifgmbakk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ovpytisd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2luyqanca.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ogrsidqq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdsehnso.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rjvrivuf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uexjwcgk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2onnswlsx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnaplaif.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2sjwnsfww.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cqmoqbyj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zxcpbijn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xblkowgo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ztsqcnvp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybrnbcod.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2onazvhot.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aoohfvxp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jfgzkepi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2sgwazkux.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2aumnwnlw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gswdguno.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mhueiavs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2avokkpmx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rkxxwuiw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hxchhfmy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2thrhidyr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lykfusgu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lgvdsgvm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzxibbz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hrhchcew.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lepgwkuq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ocdbicsn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcajsniu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2botiyhcv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ibvrxiih.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2adxdskpi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fsnxsskj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pxvezpme.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cplhlzht.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mtxisisb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wieckhkd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ilvtjvmv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ntttgssd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mgnorrwn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xqxujejk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ozlrvxxw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2acazsfpt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jwpdjyhk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cpzsdxng.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uvuoultg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qirmrwxj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwulwjju.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kvpbzvfj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xlehvgof.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qohklefa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ehifwmeu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2osfnuuoo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2asmgiwlv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjumldlc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hblclxct.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2fcgrcufm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aoogcdem.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qqvukzgm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ewtqwscp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2sadhbppi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xzgzmzio.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sznlgvrx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rsrmrugu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2evbzbbof.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zrgzyucm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hfqlsysw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wzoloyfk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tlsacpkw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2eoexfhob.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2busxducg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtekxurx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqktfpih.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fncdrtyr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bcpuomqf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vkwqkjpr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2omiaiamq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kwokstvj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vbbgvnsv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ecgutjzm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2odxjngxp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aitfxvmo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fdrgijrh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gnjqdfet.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ivwazjqk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tmvggxnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orsqzxjg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2sujlqkzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyzeioyz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukkgxxun.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mbmwkdpp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zasneupw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rlhhdlub.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ouowrqqs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwywrotd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2edenzwsq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikbjieij.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vaibbbto.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mxgiuogl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mtxsjrch.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrtztbyw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxepxnqd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxyhjskj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vqlcatct.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2eohcbtyq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2brspgmih.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2anjepxgg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2timwvwzh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwlupjx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2umyeqczh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdknohtg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sqzudkcx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuqrqovh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2aynfhobi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqtuiiub.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2tfukdlnf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2timfuctt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gwbscfgq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uhogtyon.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vubbprqj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2eyxayjmg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dmrbrjqv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmiwwhip.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2myffvxkw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvmyxmbt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kzvxjwzb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nowayyno.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yyaysoef.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xcnfbaiw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qepzacxc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rdsdolhz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qrcifmef.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dqqnfhsd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ackztcji.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ptmmtdkj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jodbpdre.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kfebqmbj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jpxraprj.html


<!-- 参考信息 -->