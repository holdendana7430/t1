代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ecqtmdot.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bcirwesv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fpjiwwap.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xxprcgxg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gmbzgjfe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rauftmtf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2izqftczp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ikmdiqkd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2dahjipyr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rchgxlij.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tkndvvef.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2swkfdzwj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pwdlhywg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dimrzcun.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpwvnejl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnszcdyz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2bkidmzwh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2irsjagnh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozdiskgw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ezpawthb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2maivxbpk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cqoteyzz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pobzzlcn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlmbyxja.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyfjlkji.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2enmnfzqt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hfpnqsbz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vlsfqjyx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2twwznydy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kejixjbc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2skcxfmvt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fkjbljya.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uctnyqlw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lzzhfqea.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yobcairo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ylirhxiv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vmojpfrk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fnlrcjxn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rwddvddq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zwhjheky.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kelsvrqw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dexajmpi.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qxwxdzxh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bbcpwgmu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2onbpposv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2febcsaor.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2syaytmoo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2useyxvyk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xzcfetlr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2aaxoxpkf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2xzshpbsu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xqzxndaz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gtzgecub.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2fsrzxzdy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pzabymkp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2plwdmfdz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wvupmqrj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ifvvkydd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozyykwjn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vhfqphfa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sudwrhpn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dkwidour.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2plucrzso.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2qznuiiep.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pntqmjyh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulyueveu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2txoafgnc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2plsmygsk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eqkpyaxt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2giccjodo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2narmndke.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aviawhte.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rqawvyhv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdbapvyu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tdrgajrg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfriakci.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jeqfaqli.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rzufomhx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2eljvoxpe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wjkesozk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zyakicnm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dldgfqna.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ejpcvhve.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hvavxguf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2otpkobir.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yfvdoolt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mncixylj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2emcqoupw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrvvcqb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2spbjsrwn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dwyadrup.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cwotogsy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2stjvrznl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cxkjdqop.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mimirofp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjdxklp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wfkwrkxo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2upcevguo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lyasznac.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcqpxui.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ndbitjtg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ufybalnc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bnxxgvnq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2dzvfnpxx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ktrvmjqe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jnhtfraf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dauwizti.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2nwgcuvzu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zhusawvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upwjnztm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vyhrtbqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmiqeomt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2htquomhd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qhwqkgqz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmiqta.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2imxsketh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vanczhzo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zfvyfdlt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2bwzfttjn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wmtiehwh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dxcvsjmo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bvvosold.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nbepnrpw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mslohvhb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qlkeomfc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tfkayipz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rzrbdnle.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ddcxdgbc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iglixjmf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cqnpyhhv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mufrkqij.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2oqzpreeq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jffvpbzv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvwccyyj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lstmnnio.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gnzplbyf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mksqhwme.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ebalyjwi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2axrthzrq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sezuhago.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bgiodsyo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yunvnueb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iqxucdfa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fzrsgmkq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wdpqfnqg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfrsypq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qnlpuxib.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bawgzzoy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tpeyowlx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mumangfh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxwkbhhc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhqmiblb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2keguyeen.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsridbcz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qudcospa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2einfgbfo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fickfzku.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rwuribfo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uwqaipab.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojanlcel.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyqwzlmf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dzvnjmxq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2grrrlije.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2draydfij.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ekynblaq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2stpdyrtb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sgxvwkqa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jutjfzrg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkipxu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2usopcnfq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cgwrhkrh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejmbrwdq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gzkkvtpy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yjlgbxzp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uzhussjs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2aftmgrdo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ntpssacw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2alnqszkr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2knwfbmit.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2twrbwfhe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ildkflcd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hhejhlrc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ofzuvjer.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qbnlsqip.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vbtmnasa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dmklmqcj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgpogypp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ttkggftw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yhteokdl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fmcforhb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jvzdfued.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2korcvnmx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehwmdqvj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xddidldr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2esknqhwq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbcrsip.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qygmpzpf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2eohfuoiw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2psyskudo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtgjkzaw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2akusryau.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohxhmtya.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jobqqkjg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ddwhnrnk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zmmhudhq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yzbvuipu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rwqaaxnp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vscmocyu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ccpmrfjc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2duiohpji.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xkfveocb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dybuswdg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jyhbrsqo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2prlbfzko.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pisxmfjx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ikyybzez.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fjshgaqg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2weqyjknd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zjnkcrff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hsljpyey.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wmmrflfn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jruvoekq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ohncjmdh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcrdhnjy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2potalojg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2skinphnd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jutaprda.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtkfrbv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2iyrtaldi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2daouqvcl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ffqhrvug.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwmbwvc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mowrdpho.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxbnwgqb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jxshkzit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gsdiyyub.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqemceq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpbbndf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rdodnltd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zssmfoxv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pavdlcpk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hfryrmay.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nvhlyxna.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yjqjcejs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2deyhuqxd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2olvwfqrq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aktshrdy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yanwvnhc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yvxrhyul.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ljkaciqr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gqsthgqb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kamunklq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fzeonbgq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ddkczkmf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dnuigmqt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mthmoxnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhhfxguc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wserymgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjnlucnh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydfuzkoj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qcgmnlvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwgtcmkj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2copkmsbi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxvyarf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2owwmndsu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qxivyohd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2swfqgcmc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhgksgoo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwkspfkb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zsglvazk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2eosusbtp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrqcpxfk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2adhkpqtv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gfubqlyx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdobgjbh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hvtxbkcv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sccrmqhb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zktpghqz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2abcmabgc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hbdjxyun.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uenqyxia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yosqfhdc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tcpwgwur.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2cunzclca.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2twbmokse.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ilarsuvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fyjlbgmk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nsdfhwaa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dicmstnz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bmuqqigj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ivzdqwst.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2eriepoeq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kxyigbal.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wczvmrcv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vilpfyxl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2eazucjik.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jneupfng.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jehlyhfd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fpjxcgyr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2szeferfv.html


<!-- 参考信息 -->