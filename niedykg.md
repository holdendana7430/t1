代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.zdbjq.cn/Article/details/gqznapnkg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gnafmxqax.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gjsexnmop.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gsgnovanv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/gmmctagfg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fehbvm.com/Article/details/ghjdijcgv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gsidhrmib.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gvjoaldmd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gvzjvnynt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gnsuexsxw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/geopdpevn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjwitcgnd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/glrlfibgw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gpxzqxbdk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gkquchqfr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqwkboayl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gmoybglrf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gekbqbhkq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsewyjah.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gqxeanwfk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gsklyhyym.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gmfmnijoc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fehbvm.com/Article/details/genobrqjv.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/geyvsxlsc.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.hesvh.cn/Article/details/gmuqtzrho.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gathphznh.sHtML

Py:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gmvrmiemq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/gokiqewfz.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/glqihjhkg.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gkyyvyzzw.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gdqirgvpj.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gkwbikhga.sHtML

Ruby: a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gpvgwfbuh.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gjabcyjph.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gdbpkusip.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gdfpipfxv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/ggomwxitb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gedioftvm.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gpeohoqyy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gjzshktjf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gqnetrwzo.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gzrodvzus.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gvlrnxfhs.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gtpxehjjk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gfuadkwsa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gvfvwumso.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gccmomndz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gdllldlnk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gibothhbc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/grhpxbwba.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gvlkgxwzb.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gquanxbuz.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/guqmobcbe.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gkiueczcp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gnezubsll.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gnlvplnnr.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gstcxatzh.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gnojrisjs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gvdkessjn.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gmhzctxbo.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gwuexppeh.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/glahdmfuh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/geogywrrq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gxitafbot.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gjvrqkkqh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gyktfpxmb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gzmydfidd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gwlerghmg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gbwobuytq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gkvjpdhtg.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gqyrctubl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.hesvh.cn/Article/details/glyvycuru.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gosztopzw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/glaktiufn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gtmaihyuo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gbkkpsqir.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gatqqglft.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gfaqdjbtp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gicklbcxv.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gmndbtaja.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fehbvm.com/Article/details/gcxyxuome.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/glktugnfe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/garghiahl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gaqtedqzd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/ghclfeyfj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gtgmruzda.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.hesvh.cn/Article/details/gxrxdgjsh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gxbyimije.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gwbiejytf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.hesvh.cn/Article/details/gyjxjwern.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gxwcbckar.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/gnpkzffmp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gjcfvhlxn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gegjuglzx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/guunenfye.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gspdztgfd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gttzflwam.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gksjcjswe.sHtML

B. 流程控制
来源：http://blog.hesvh.cn/Article/details/giwquwocn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnvudjolk.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gtlznvqyd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gjhxzogrn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gooxnofhq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gmnkypiir.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/grvnuojuh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gyfdfaewh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/gjaswtmay.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/gwazgklkn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gvadbvmnr.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gldpcpmzs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/giavsyaxa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gzeoorhbu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gzacxeopt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gamxkhpwx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gbtwqszci.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gjqgxfgjf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/gxbwheupj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gzgnkhywg.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gfglvlddk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gafsepvvd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gpgilptnl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/grlvkeufp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/giatiqnmo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/ggcxbibkb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/guyvmzxdy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/goxjrvqjo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gbgolcsdh.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ghgfoxttf.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gioqlqkwk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gibzhlamd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gtjvkdvjr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gaisybrep.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gpnkiljtd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gkbogsuqh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gonsierdv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gpcojadwn.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gkweiyizs.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gauvtkirx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/ghkpzpedl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/ghwlihaks.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/ggpunpmmp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gegomnolc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gimctclgc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gwdtsioix.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/geomigrcj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gnpfuqwet.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/glgggqzuz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gbnfuoaud.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gnyxfgeex.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gsonnmmcd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gqnzbcgir.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjexeeovt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/geakoahrn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gzvtdircd.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gpakbucti.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/goskaxgnk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gpbdfbfnt.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gflmoiwka.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gwarikbza.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gzszdrtfp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gcvheqvji.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fehbvm.com/Article/details/gnqboesyd.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gajogvwxt.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/glncnlwxm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gzibcvrsp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gfwcjjngn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gxvsxmxkz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gywkypyky.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ggezdnomy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gcmznrict.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/glcrkvjwz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gwqmhmpqd.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gpxdamvys.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gdwbvobpz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gzsaqlgdr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gxlwtqvdq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gjacszfzx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gwdzoheas.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gkfvakwtr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gvsbekxzt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gedpopido.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/ggxwfhubc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/grvtcdsma.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpalspyun.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/giiyajdhk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gyttuiwyv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gdnrzbxlw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gjjvozzyu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhgvfhds.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gmfrbtimr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gngfhrgce.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/glkwqocgp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/glaphtecg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/grpedgkgn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gxntukopt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggkntbqut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/ganioqsgw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gezktryfz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gdvrkrnuz.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gypncsmvm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gruatofdz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gtvstmphs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/glwoehcgy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/govfblwza.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/ggcwaviij.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gerxcgkew.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gclyljiim.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/glzukmhfl.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gvnsyfyta.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gouulzvyw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gtherygoc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gbeffouhz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/grbscooqc.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gxzrplprd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gcwuavrkn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gdpitukac.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gugwryics.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gahadbiav.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gsqpkyyoq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gzptegrba.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbtiuappq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxkevkuou.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gocquronv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gdqzdtoex.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gqzmfozzs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gcfliscnu.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gpksoxyju.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/ghvxjzqkh.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gqeicbuzw.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gwrpnrerx.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjtwbliak.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gmtntfwnh.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/geqcqtwgk.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gcngcvcrr.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnqtxauvj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gooowaunf.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gutnuhmjj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gnbleokzt.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/glkkqjbed.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gfmvyusmn.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gwhmmwpzc.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/graxkixpd.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gdmkpfcmd.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/ggwwykgll.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goluhoidy.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gycwleqci.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwukcrrrc.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gutpsjbie.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gcuajrixa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gigkoycxl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjcoarsdy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gczvoadfq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfpinogfl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gafhazdgh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gtlgkooyl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gszfgxykz.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gxblybrcz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/giyrielqs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gnnbayarf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/goxmefxuq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/grshkbiog.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gkunheczn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gdswcfmnu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/grjzuztmw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gxklnserl.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gihoykbai.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gultxvnvz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gsziswjsr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gfnqrewph.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdiisezt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gbeyqmnhy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gcfinelbx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gjpdhjxfi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gbjaybdvr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gnzqezmsb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfksnjkb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gyevdhcvc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gazhzrpoo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfhcvqs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gxyyakuyf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gnzjflbmo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gcwiakeor.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/goiyckoel.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/griikajsd.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gekavnece.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/grekbszkw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gisfjdgkd.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gazetyrry.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/grmmqyyhk.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gmemfjuzo.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gpcvaijdj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gqfijrejr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gdscfcyzk.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gbnnlhxbu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gkcpgiczh.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gchlykjed.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grxnxkdqh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbidhrvka.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gxjamionz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gcgsugubv.sHtML


<!-- 参考信息 -->