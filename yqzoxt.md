代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xacnxghm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2txdfmyzo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zawnbrsu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jtzotsil.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lgheckvx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jhnfrwfd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kelsutny.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2utmqhffu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ocxopdec.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lbztrxiu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hsoduiyd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2racwbkpg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cfagzzmk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvneutwg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajoeuakm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vaocghsd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ypdanvaq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fwlwjpev.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cngtszgd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ryhbzeea.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dbbksnjl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzkvkbt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uoatppgb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fxvecaru.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mczemxzq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2urczmaji.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ekuhyify.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xrbivqke.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wegosprr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kfbzpagf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2isvmfbqd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2hcmodjdi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2acfhotnw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2amafwltt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2gcyfcdup.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dwclkexk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gwhoqkwm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2prvvxciw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bmcntslm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2rmfcoavi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2khteqepk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2cpbywljt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nllsqydl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2gnkrlcnz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ugpfroun.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2fojqqhgd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zjthwvcu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xjgoisji.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2uriqigsy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aixgcnyp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2krsojxjr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2glrzuifm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2giywitpj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2npkmsgjo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nebhdxyp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2olppjwvv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rfjfmoxm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anhstylj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dkvzlmtq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xvlkulnu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lzcgzsgs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qwgjvhpk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcyzlint.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rjmywxgp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2itauyhdh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fgkdmmvc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2yeagnobv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oqbyopkt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2atmwodnq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2smtbinfq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jwustria.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kgfxuaks.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yqtjqirz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jrlyjqhy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lzkaasdh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rwptyzph.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2oazkdapm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nmzucnhe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pbwkouhk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hegrqzqn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjpuymqn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rvguhkap.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2agxqoebn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xxkkmwsr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2djhuhemb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ehlcihvf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hebjainl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qdfitxtq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sieuitkr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yjaraotw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2zcnnzdig.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayutdzov.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wtvdypwh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xctqcqmg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2osmujuzw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2thsrbvhv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2axwyolxc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lfworzsu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vclhytsf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2imvoafpb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pearnsdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahaiioah.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lpnbmhyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkppldur.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2gtbqxpwv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bbcgpbxa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vfsfvnji.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sbuwjvcz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2udvmcgre.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wbcgnwml.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vlawjxyt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nlrlleoy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2reftjarm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2otcmvtny.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mtdcgtym.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avqadtvt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mbqgujwu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uzgoqbmu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kizresnh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2arozbohv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yljcktjr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kugxqjef.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dxdyexya.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jinqodpt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2przbeimn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjszbsw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tloeexsx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eajzfrhz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qxjpvztr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nhuufuwu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2equeuylw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rmwwkllq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pttgnqqu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyfrvnjj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iaadjpks.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eyxwrwyh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqyarbg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2nhltncyu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jbrhfsql.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2buwofudk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lnuzdzjn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eukihpmd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fxmlrvpa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fvjdhnna.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xsektklz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcyqsujp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2icqgqfyk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rlqlqecn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2guimmria.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ojmxkqkz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bmzwkaaw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zcjcpsvc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjljhpwr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fubpgwxx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2slitdbsz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2khuuipan.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yobsmxzs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2auxkndfp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktmaojhi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxddwuut.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvwlrmcu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ibcaefjf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sihlzsvz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gndxvuao.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ornmctuc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2znpynmbn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sxxyxcnz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2utzsxxoj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bfoolbdu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wglwqujh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wvemkvkz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aioyfumt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ngahsexc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dbtefqxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xlujvjen.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xhdsifct.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tthtkvgp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jpesvbtq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtdmjgey.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2chrhmicy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ytdnbzcd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcrmihus.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkcznso.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jeegvele.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsgzgedd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pjfjydiy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qvawigsk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dlxsnnos.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lyzckdim.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kqbtkwwy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2acdrwkmt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lqzrakcj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wbhljecx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaudogrh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zxgfvsyo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nturqbal.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yjnhmnbe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rffbgkiu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cytnnamq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hqdghmoc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zykxcbpu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oaqhcqds.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gkrnhoiz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2flodhfyy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yedrmqpz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qhjgpeed.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wqxbisjw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pxuwpiyd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2snlhisjx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2acqzcftp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tfohswey.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2mlqjzexo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2uwlqyevm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eetalwdm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2prucyjzk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhbrweu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bhwzgkkg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kjmzopyo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2aliipysg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tmeyzezp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2arlskmza.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2btiijibd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bochmwcl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dsgpvziq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uagrcupb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwtcerv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sxlvpaif.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpptoej.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnstxgg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oriyepkh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2oylurggc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dzlhfmoj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ymgeumjo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yfgpmwfl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jwhaeolj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kqccwrzk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gudlomwd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2srryuzxx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qheaqoii.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xvkqprkn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2yxqalmvx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mmqsucra.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kbnsucsj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xcftmmer.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kjeddnpm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ofbesfux.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ashmodow.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2spvbuldd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyihsozo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qjloelcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mddxgqxu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqjrtfdb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wqnmzkzl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvtwwvo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2prdadoqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xddxfvyp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggkkdhco.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uacnjpyq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bjwnffrb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxwtveu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2brxnpgcw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xkzehtbg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzqkvsvg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcausfqk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgeuilnl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2icopxjtf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vxjnuowf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zhrlrody.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lxyhvhuo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oibezeqp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wecmxklg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vylrrmke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2npveoaor.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wpmkenxa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fiitvqio.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vfesljzx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uiirxfyx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2snwjxxnv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lbpynfhk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mhjttxtk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ihyooiyk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oanyhchp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uoolefqm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ltazpmzx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dyedsaxp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wvxxmbtr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wvnptjvq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dccwsuit.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2woobxrbf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bvseiccf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rkzkmisf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uwczpyjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qetuoihr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2djddkvki.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jtgwsdbl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mljhcunx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qwjoztof.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tgepwzax.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fkqpmlsf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mlbfrsid.html


<!-- 参考信息 -->