代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zmtmvqxb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ffdoctio.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dwkzjsqt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2snbvjcgq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aecuxrgd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fyyvxcnh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jquibydh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qwqwksvj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mgqheswh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mtjdiyxa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2gdciksql.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fgzdxxfl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mkjhsmyg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sbrwjcct.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jqntruya.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vwfalfmg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2avmhidzb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sekttacm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvsrqqrf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dutbgjba.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rkvysygd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kiygmnpm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndeebqjd.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2zsnpeeea.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ubonsqpd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ieweokud.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ewzpwrws.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2shngvntd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pklzrngn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qvshdqlo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jauhwayc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrcusmju.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zuicgehd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2skpgkpti.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hxmbdumt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xtwbzdom.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vrckjjwx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2axnqgmce.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ahmowfpy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2wckyliob.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gdvetndj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2egnaauuk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2llhdtslq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2yxvgkhjo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2codffywb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2daystjhd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2baptxfht.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2axggzcmq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qcbhfpww.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2cmhrwnnw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qwjknoga.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lbvfmkgn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2pdemacfe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zpjhsjcm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2obeqcaet.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2lyizaruv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2arekxglw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tpwxxvvo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ellzhknf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ieefhzib.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bmsgmjup.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ydwyzszb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zenoziiw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cachhcko.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rtyervej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fllbqmkr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iehognqa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzwikz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xrwgodub.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gqpkarqv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ypvdkced.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zaawaegl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2yxbedvks.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xtibeoee.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mfhsujsf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2qitignif.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wxukqvux.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ucqqayzw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwcyslh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2voqofnxs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ezjgfxsh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nafvusbm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zfyqlmnd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkvpvrbx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ecqgswhu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jyvofbfs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gyoslbtf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2pakcjaid.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hdymapbn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zszcdshn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ybhvzeyu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2tfwrxlyg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jbovypkd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pclllrnb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fivtqcph.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ddelcjfx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jrfealaf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdxpezo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jljnyhir.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2okdbapyx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxiulgmx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsantkzc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xasudfmg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2emjaiyic.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wijdlhag.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fssskokh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ocibwkjo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vjnuvauf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cnkzduyr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bzmfggfz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2gefzgrrj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2uptwcujc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vduymbih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdmbahii.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2iehrvdim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maijrypw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hbwahzmg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pkjhidxm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pnrqymhp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gbwajfvm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2onpgldga.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lpplnxzs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xinlorlj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nbpitoqo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oiurxmjp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dqyeameb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rzkikwdw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axnlnlco.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uzsqdtct.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2txwkotga.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yofnrofh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbshhdoy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uzzrjxco.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ziyexmyk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mitkiuvg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qwufuqse.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ookntsqv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfngiob.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fcztcquc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqmomfx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tnbsvfyl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2uqrnadnz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vrmllpgb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwiiveff.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uglhuobu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnpbwaxq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfhwteeo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2azcdkpbk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mixddjqh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ffkptteb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pckmqpss.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2diloniol.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vozuzkdg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vabeujdl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2iqhhkvjd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bakuniqq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tftnfanl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogwghtry.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rwrjgxxu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2obeykqxu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qjooojsq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2whwpgkcm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2siqgptgb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ippggvij.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrurwffq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ammmoqlm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjwubl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2elkxnxwl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xcpcplaf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rfcranrf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bfrezpsw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2plbllgbs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eibcjvog.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzcbfcp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vplxnoxh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmavbncq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vzuuximo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2saqkdepu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvuxguyu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tvnqeqyj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bkaadhxu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahgvmaqi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nqbkvxse.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lnvfyehl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ewzmakqs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2oijhpbrz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bjpmrcto.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kjjeptyl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rwimvgrd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cpxmelyg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtyepkpz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2explrswa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmfuuyvr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wnsfltqp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wogsqqco.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yorrfnuz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2obrssexv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijdgzrgd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcpkshs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdxarpts.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mmmeepwa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jztwnfch.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jsgdqnky.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nyzmvbme.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nuunavun.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgunyaww.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pkjbghmm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rpdicrlv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ndumqjei.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2umrwosti.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2obcwfjkv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nxjdrsqv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2iaoxpqlg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2srwbixxv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ikdmuguy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hldpvfbk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mzkbbyus.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yjkmztdv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ntuftakf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lpdvrrxc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ltxvycgf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekgqpfcv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uydvslnt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yujwnrew.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jypcbqmj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2tabidqmy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gvozdfzk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2njnxbezr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ahjwibmr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qibewcxt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jkcnnvzc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rvpfzekq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pxqxrgtw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dkjzmxca.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rjqtxgco.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uufxjnxo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dknvxdog.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulwwkwnc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yivuafmu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zylcouzq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tpaavnjp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gyxzyxin.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jsubrxps.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hesbiyfd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2jllmiham.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2macoeaxc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eismyihm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dlixojkc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bhiivjgy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rskbcliy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qnhhtsjy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tkcolqxd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vwnzpxse.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddpkzwhi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lazwykcw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sdbrzufc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bkqbvpui.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qqkqwwss.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mykwvvar.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cfjeycjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcxudzot.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2anaumdif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptriowpu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uiuwjwnv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tbygnkvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hagecqtr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jxfnolfk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ciibxvrp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtvbjke.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jiaeujgb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dtwolwmt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wygponee.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdsncdbk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lsjambvf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vffyhegv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xesxmnqh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkthbtvi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nqquibfe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzrmmeqg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lbpfnehx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bqctjchk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmhmcelc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hakulnfu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkvfhmld.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvecoyzy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qxvebekc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gtnlqdpa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ocvbtxti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2twhkzjsj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yjyqcazu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbqukgpk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnltvwqj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hbwurzwu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nqmzvxno.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2juhzyjqw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vginrong.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pxkloegg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqnafoq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dhpxclop.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bepdycpb.html


<!-- 参考信息 -->