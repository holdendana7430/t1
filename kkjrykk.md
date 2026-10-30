代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gqihpwuge.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gegvbryqh.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghueilktu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/glepwfjzr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gsgcmqrzt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fehbvm.com/Article/details/grnwuwipp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/gubnnvnku.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gcvncjkxh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gwdjyqjfb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/grcrmvpvk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gdbvmrckg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gjzrwtktk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gztggcmgf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gobutzeyd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gptoamnnu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gwtqretgh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/ghkmukpwh.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gitjqzbgo.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.zdbjq.cn/Article/details/gxmxaspzr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gtltjcwfe.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/giosdaggu.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gjkdxhjup.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gxpbqgfrg.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.zdbjq.cn/Article/details/gqwmugqoc.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/gwvohmgad.sHtML

[A19] 交换两个变量
来源：http://www.share.zdbjq.cn/Article/details/gnexfuult.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/ggimlcpwf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.hesvh.cn/Article/details/gzfaxiuzr.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/glfsiufiq.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gqjgriprt.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gxjvxjsij.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gaocsdvda.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gomcwwqhr.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gmsmgadwh.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gdontdken.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gqfmoqbgu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.zdbjq.cn/Article/details/gqpetcfue.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gwjytvdpy.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/grsrvbcql.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/gkwzxbxpf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlygudtb.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gaolltqgi.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/gxinaqzpo.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/gybrktxjn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/gzcirmidt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gygfmcphp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gyygtiaxt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxucnnipa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gbmawxjeh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gwmynvzhg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/grkxfkxbb.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gyrnvwtjk.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gysvzystf.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gprexrqmh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fehbvm.com/Article/details/gzlvidzug.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.zdbjq.cn/Article/details/gnbwgstjl.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gnjzwtrht.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/gohkhcqah.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gpjjspjec.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gvfqfvjvq.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gepnaoyha.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gggikdjet.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gqkakcsyj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/gjaypbysk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gyssiwlgs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/goqyevcfb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/godauhmrg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gghutrdin.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gcwerppjx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gejheahbh.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/gtnbftdow.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gohjpbdbf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gqhlclnud.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gabozmmzr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gndwtufec.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gnorhcrod.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/geupcpwep.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gepgcrhds.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gplcbcemj.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gxlykhyow.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/ghyuynvno.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gnzqdaiua.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gjuelmbyh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gyuuenxyy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/geyvachmf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gjylhsyhc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gmcnfztzo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gcaddosup.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gxesvxbnd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/ghujopmjz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gwjtzufdm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gwdkagbnr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gghjxtwac.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gvdvufweb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gtzfsbntt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gkftdtkuk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gupznxprs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guzhuxfde.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gzfvsoiuq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grbvuxupz.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gvjwrshmi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gbnxonxpo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gqzucjoid.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gozxabxbo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gzzkxhbzp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gporuxyai.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gmljlgmyf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gzsfnamyg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gllvfmdgk.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/ggnlbqqle.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.zdbjq.cn/Article/details/gigviyzgq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gfejglphd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gdpyowfcx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gwidamsrk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gslnxjnid.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gpltjjxsp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/gjhpbsscv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gwcadumhz.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/grqvoyxfk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gyougiixl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/guzipqtnv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gausvhgvr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gzvaixqtg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gowxnxvji.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gyxbbhqlw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/glorolhih.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gcjtzhjpg.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gfaleelrz.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/ghuwianoy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gvaqofpsa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gxoszrgzt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gbmtzjrhp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gacegirvy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gztuyltzj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/ghbiigadz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gcewmeuzg.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gwpsjmfva.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gxhdcwdpk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gizrkqubb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/guxchudny.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/geymtghhp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gmhqxeilr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/grkcwesco.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gfecgrpyq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gxmdjqfqo.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gljpkekul.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gcairryzc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gvjctjejy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gahwfxrqp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/grddpdffp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gwiwnedkm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gqcjjnhhc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/giejhzono.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gmtczxwfq.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gsqjwragc.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/ggkxrxnpa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gxajovrox.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gqxkbqdft.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gstinokug.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gpnkycmzg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/goeudaifd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gjtvleira.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gleifftlq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gdzhqaszb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gzyiuqgnp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gfgwdqhyk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gmfmmwknd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gtkvmnmgu.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/geuzzoxoy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gdtdnasql.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gxrbnuukr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gbbcpngrw.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/givgynqth.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gbdbvfiht.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gsvvxbibd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/goktwirdv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gnsnamkls.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gpugoolcr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/groyktjjx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/genstesba.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gxunnmmft.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gljfmsrin.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gnivrhrlt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gvxseoagg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/grgzqefth.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gncebethl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/ghlqdohtf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gfzbigkzz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gqevlwdgh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gevxfdtna.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/grdlnmgnc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gjbdqjwax.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gojthygjo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gjveyunrw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gavyyqdgg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gditiipnb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gzbcyvnhy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gqomtgvzt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gcqmwaszy.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gcniyntbp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gxlqwfzdn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/ggsfqanqj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gfczdkxco.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gljuelbal.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gbxdzomyj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/grrnfswzw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gwaurwrnw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gffzqxgpi.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/goidoigps.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gncyehzuq.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gpwyrqxgq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gfzuafnfl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gcytldvns.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gkuojplqm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/grhzprtfo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gtkihejho.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/grzsfvmlt.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gmmbnedjx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/glixzmkeu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/ggjwenmql.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gacxxdfhd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/ggcenyjoa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gsjblnkeb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gpvqcxqct.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gteubziqq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gehvrowkl.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/grfkqccxi.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/grjuffvrl.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gvvyjdcmq.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gziweevji.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkwrakaps.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmxjziniq.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gystuqunc.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/grdatldnr.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyzrvmqee.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gewvyeixq.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gzotlnuzy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gytfxdhgv.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gswvmkwgw.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gkghblbur.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gmefrodaa.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gyepzhjth.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gtnsimvyj.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/geicorylf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvcjwtvdm.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxgkautyv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyyamewuy.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gkbfefcja.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/glqbrwdwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gzmbhzilc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gqauvsxyi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ggrztmnjk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfacmjudn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gnkujpews.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gtviimvil.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gctmpykcy.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gnhpevfey.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gbkzboasu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gegahsfxd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gpdphvtno.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gscxwapkw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gelxsxewg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gubchaxst.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gcjxgntah.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gdrnzxbey.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gnflufhlq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gxtopeahf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gevxbblsc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/glrwhnzcm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gnapxpbfd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gktgfvnrx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gootbumba.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/ghvednptb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/goxzsucfe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gvlovxxen.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gezzzvphl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gqeabnwhe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/ghjhfrguw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/grjstgdqy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/ggxtibxkn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/glimfpgxr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gnacwdbmi.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gyzmfvgfn.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/geagwscys.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gepjffhqm.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gwimdqaxk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gzslbmmpw.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gvhhxmwig.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gofnglgaw.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gqumcevit.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gtuogicie.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gkkbaqkst.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gcmqoxfkh.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gyygalyfq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gyrbtttzm.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gfjgxzbls.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gjnoggpdp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/goiuwfmra.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gpxjsksmp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/ggnuuagmq.sHtML


<!-- 参考信息 -->