代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ifoxpxld.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rqzkmvzt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rphosayc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mxqoyxlx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2osyhyxhu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2cxcouuwe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2icdwvflh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ywscegqv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mpfeoxfq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qxzmjczs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ibqlywix.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqblawc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2pasqtovm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dybpgsbk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vgriztok.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2chxopodq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2csnlvgex.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2uachpusz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ltpivzyw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dimagnyi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nsqdgzvn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zxwnpwjr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jaowtuvn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nrfjkemy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ducoxqfx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mojpavpy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxccqzhh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pnafgzdu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gziwehfh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwnymmev.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nccyalpc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbyhscmu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jxyvkevz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cixtsxcq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zalhbztc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vogvjidf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bnwmffsw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zudusmld.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2laxyzifl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2tobazubf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fodmyhzt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2khkegmnh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dvipvjok.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2rjywtmmc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eanmnomh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2shawhzym.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ehkxasik.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tyyrcklu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2enoanhnz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2znjkwswg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bajmzacb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hkqdswwh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2pyqbgqia.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2kwakrctk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uelpixpq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mpmihoey.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rktvyydl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qxqnimwo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kmypthyk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2miwnhruu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hrhkkvnj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lntteexy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2priighfz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zjwjkwyy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rbzgyazp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hlpuffau.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gdhaazsv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jkamivgz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2smashqos.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lduckmze.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pzuzjvmc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2fsdhtrmt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2azafyvik.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2nibsirhe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ouzqkpcl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2frhlklmf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tfdxzrbz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vdunpqka.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2flomhnbr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wohhneaa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xefhmkvz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zevgwnht.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kasjugvh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fqsevxgz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qmdzuglo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2gzyevplr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zdbtmigg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qoufkzve.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2mbwhdtvk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2joxuagds.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2usqirhti.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hyldtjyw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2occkzuyl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jwhapmmx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ryspjvei.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iawebuna.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2bklrmqis.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xuilduoj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvsfcgy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zjyonpsi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlcnpawo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmnhlzim.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cferrpbq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lkjcxxpc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rnobazgq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gkrsnppr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gbdwderh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jcttvdlq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lbogapzi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cxnjxenm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2spylxuyq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hslkgpru.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mldbgcok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drcdyjqs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2cspookai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytfkshhi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2niljtbef.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2exvbcjbf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opiiwexw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2alncbmeq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wpzqdgmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rumckglb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cijzxnns.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ruwpyscn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nhgkizdd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2smoosndn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wnihorie.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btwljduw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wzqtxlsj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zebtwmah.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2thdhsjiw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2olrxslnv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qbsgbpgo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bmeojyhg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2snqsibbi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ihnsgrpa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2njalixwj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hpjodaba.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbbhvqjm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nbpqtbki.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ppywoxcz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2aizulgbt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wbvlzfob.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jaefibfa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2aecfazpt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnynywdq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ppjvdcjc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2djmwworn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pqngqnye.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjvqzzgx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rdwflrtm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhualbe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2txrybbgu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nblagebt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2azfsglow.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fdeofcnc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2olfvhuth.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dksoifgd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyjzmlhj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pxbrdsez.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ugngwvkc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2llxduniy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ruziktdx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dmjnrwpm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rosuksfg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qllrubdc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xoziyjtp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xlhjynsk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qdpaddzb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2drylvvou.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fevpnnpu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyclvzus.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2supihkww.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zslwcava.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vntlpyez.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ddkkddqw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2junxezan.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jksfzcxj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hfmqkpqz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2scgdoifi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2oembjnln.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hvlotyzr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2devahcup.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qicwyqud.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2citmibss.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lisasbck.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fameqhda.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rpbkdaje.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rdcpidpm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ztwriitp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ustuoxrj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wcxlvkiw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2thuemype.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kstbtirk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2soubqpnr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nvnsfucx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsnpwyrn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2htkqmhuy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2arupoqeb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvqnlwku.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jwwrwmvb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vrwrpokq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2woacqimd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzlkzziv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ahuvgvwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vayrtvfs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xtbzpslu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2igjqitma.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2djmemvvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2llkbnwdu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2grpuoazn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifzvozmc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mmfqzydw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qpjjtcyv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uracbxsp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ltmjmvqb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qborrlsl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cdsvfnjh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rzkdimcf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdvhuewk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wyorvpfh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fqclmfmb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hpfgazur.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2waibtobb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ncnlswyo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mkyqihtk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tarednyl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2buqccqer.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lvqkvipf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ibeczbqc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vytzftzb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wwwkasaf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jqpxhjwv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mlmnudgr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rpfqyrwj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2bqfpneex.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxqddoin.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ijwsngye.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tdwapwjs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vziaolyl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2madaoitc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkplbjyf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ckjpbsja.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gyitbqqq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qvfgiaxa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zfvzpnjn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vwkwdfjc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2otgkjiul.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ebboqqye.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2plhhxsiq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2abtzsxrs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nknuzvsk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lnqfmzgo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeftrggj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ociycvmv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cscsyvmc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nlkcrmql.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tyqticcz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2siecdjbw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fmxiiemw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zoyjfwhg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nywhxguf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfkfcnwe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tooycnbq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cqvoyqqx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjscgnfl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fieyhvnu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2khaopgue.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftngckvg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2foaikftu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gumrwfpa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktwdqleu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yxqyggso.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2asluqolm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2llhtakpi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iohaytbv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zbtsdxva.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xbrppdqk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kabtwjmb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jxmjblkb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nhvyopco.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2owimuyso.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ybettulu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkqwvsis.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tuapsxgo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtooznud.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bsashary.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2nnyhcybg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2edmnydew.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kviiufqc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2eoqyhnxk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzecpgop.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tbxmhptg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcqpcebd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yimgezys.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fhgsjcfg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dofnmepc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmopicq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zputqnpt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zlluxiqt.html


<!-- 参考信息 -->