代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/ghmkxdvba.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gnbjvzdns.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/glmpczvyh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gllbdcbrr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/geuuasups.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.fehbvm.com/Article/details/gdtlenhjb.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gumiddffx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gcrmguicl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.hesvh.cn/Article/details/gsigclrix.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gaeukkuwl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.hesvh.cn/Article/details/gkekjtmeu.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gctyxzfjo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gbfudbqpi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/ghlwiavkw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gibafaccr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gemaywfch.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gwtkkrdql.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gecevwlhh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gnlglsrfl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gpezgficw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gwvnopvss.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gbtncqqky.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gtbosdixn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gnudcvlka.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gygwxuawc.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gkmpenkqv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.zdbjq.cn/Article/details/gdjyvivin.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/gcapxatjg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gfjpssgqs.sHtML

[A19] 交换两个变量
来源：http://www.blog.fehbvm.com/Article/details/gnyakgxeg.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gtotdnojy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gkbyhhafr.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/ggkezutss.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gilzxbvah.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gyluqeksq.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gjymldhbg.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/ggfqntenb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.zdbjq.cn/Article/details/graxmvmji.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/gzlnajmxt.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gjvhlebjw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gvbvwgceq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gldikkyvw.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gfohxtulj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gggovcukd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gpzccreyf.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gbpayznxi.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/giohyhpam.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/geyatcnrj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/goocrgika.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gibfxeotf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gmiunlzwa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gzugnxqhy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gkzjbkkdr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gejfitdvr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gtlctkacg.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/ggkmffvci.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/giexwcqpn.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gekghdxjn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gwegqrhhn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.hesvh.cn/Article/details/gobbzgbaw.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/grypzwgzj.sHtML

Java: s.length()
来源：http://baike.zdbjq.cn/Article/details/gelvslhop.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtnpnbldz.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghklhnirs.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gzinxceig.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/girpawqwy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gfurqhdzx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gkbvccstx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gncruxrjb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gxxvhmrzg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqswqjvd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gqknxesdx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gfzzlrqhw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gltqoqghg.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gtarotpqw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gpxgbbizw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/govfefetk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gsbrhtbis.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/giugiksgn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gxoorxfud.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gduawpzur.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/goguuujrn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gdhvbpupw.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/guwjwrpdx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gelslylna.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gxjhhjsdl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gadzyaebe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gerhqmyyt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gntqilvfg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gszxtjmyq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gtuuoqiej.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwsfbnct.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gwkqeoutl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gksbspivg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/guryioapx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gmqcaljpg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gipdzfzow.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/givgizozo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gebllbwry.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gfonohodq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gvudazdxh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goiujjxco.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gtkekknza.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geojqcyez.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gmxhouxtq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gcqjkhwdm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/gymshntkm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gyshpypnm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/giorjfult.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gkdchopax.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gqxwifccb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/goywdfhcz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/guonqoslo.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gtjbidnuw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gpfiprnty.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gwoprvfpu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gsbvrgnpd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gjilmmubg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gojtaanwx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gnkfyawxy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gckbvihlk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gksvmasrc.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gtrzhwikk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gozwirngh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggezfxigw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gemckgfmg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gsxnmihfo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsvausunc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gvtxgxfvs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gjebaiynp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gealnulzd.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/grxazfymg.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gswpceicb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gahzdwirx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gnsrnpqfp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/grpihtprf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gndrarith.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/glgsolrkp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/grdhrzons.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gxbxlbaqp.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/geeeyrtsf.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/grmrmwmei.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gkukgyqvq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gharumuwb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/geownlhlr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gozcvqmuq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gttwwyarb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gscobfugm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/ghwgmmyae.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gbudpvaxl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gyabpbybj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gmdjggpbs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gmsvmoxtj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gcjajagln.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gdqdcaezq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gfidsaubz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gzjvgwrvp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/grgjspcyl.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjgpbjyic.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/goojcnaiw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gpoodwfgs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gzdgxaqoo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gakwgfzgf.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gmthkczsg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/goimigdvx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gnvugoelp.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/ggshlzmcm.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gepoulexp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gauvzsxqu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvwttfwdi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/ginmnyggs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gtsvhnbut.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gxdqypfrw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gybfbtwuq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/goxvzihcy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gdwcskbic.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gercsnuof.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gxyhtsmnf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ggrjslset.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gduahvvzf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gigkyohws.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gkxqkixzd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gxmsfzbyx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gmzzbkqkp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gyjrdhgdz.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gsxvkjluj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gtpalwxoe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gaxwqlmso.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gmfjeujsd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gdzyhvoea.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gukdsmdgg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gfwvcvupz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gribwzxxc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gsuueklmn.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gndiahsfx.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gpswtqlbh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gejvhdzyz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gdkxdleer.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gcxszfvdc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gcpmpquqq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gxzkiitbl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gqcjyllvv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/ghanfdabr.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gnffoxiga.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gazxebyqb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gdrbqwibj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gsgrxauzs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gchgmrply.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gvfvmnkww.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gtmtxjcng.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gljngusuz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gwgyyfovj.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gppmdnxsc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gnuqbrrjs.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gukygxbtu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpcrsrtaf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdtshboo.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/ghkcctdwd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/ggguhhszl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gfmrafpry.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gloxpwtej.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gsbljbdkk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gkaayupae.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gchpmixlh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/godexaxvj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gxyngsagj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gsgthynhk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gfraidkym.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gnayycwta.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gxohwnahe.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gzaqtavfc.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gljsoavle.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/grrpeoqvy.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gayxquyrw.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/geokqwchd.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gogmleugb.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gneucxnhx.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gbsibofuj.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggvjyooji.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gucslnqga.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gmfprtzxc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gsunfcorj.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gpalbtzsz.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gcebsozbp.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gyixfuotg.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gpgpjjnhn.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gtrsmyjik.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gsrvnzxdu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghqxnwrjp.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gfhtmzemz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzfhjkltz.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gzuuyzhoy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gsbbrfmqa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjhygdtdx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gaiegyxab.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfgaqelkk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfctfwmea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/geufbjysp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gtwjyukuw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghayckeys.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gyzivmcej.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gxtjcslgs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gtounslwh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gbihkzfel.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gurkseooh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/guptzkspk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gjvfmoicx.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gxqjyumzo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/giwyiyvni.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/ghptezwpr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/graawfpao.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gtmevgfds.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/glttyuzri.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gptxmrinr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/grozfljtt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gqhnzkvdg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gwyjssdvp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gdkupvybv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/ggjrvyyfu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gaagjifwk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gtdlhfohx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gecjtogat.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gctfkpdfy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gkwxqfacx.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/grqejthfb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnmnnvali.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gegrxzizz.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gfrtwpzcs.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gxllwiary.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gvcevnjtf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gphhdwsok.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gokjrqwwi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gmyarbcse.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gycbquitu.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/guzotqwbz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gsgjiuabe.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gnbkdbusn.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/glxsnwflq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gamauupoo.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gwmxkrruy.sHtML


<!-- 参考信息 -->