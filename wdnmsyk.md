代发 wailian999

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnxekwbq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvrybxtf.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gktbuveqy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gmtgqarrg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/geziktchs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/gbaxiwmoy.sHtML

TS:   if (!x) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/guvladjqp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gaxlrpphx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqhprxlp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapcofciu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvyirejaq.sHtML

[A17] 位运算
来源：http://baike.fanxiaobao.xyz/Article/details/gmthfmdxe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqxmcljg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gpiakzkzg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjslavjl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvifbiwwo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/ggwgphhin.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzkuascb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gyjknvhfr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/griktfqpk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/graazmefh.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/gohpbtscs.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gnordiaix.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/giueiibra.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtamoeri.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/glsjxegic.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/gsfdjfeho.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtidtwkg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/gfdosnnlb.sHtML

[A19] 交换两个变量
来源：http://baike.fanxiaobao.xyz/Article/details/glkokuklv.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneixmbxj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjqwaqpz.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjziznlin.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsnnbquj.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzpymyjj.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbapzlz.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gmljamodl.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsrolgse.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghggirbeg.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqxxyhth.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozdylvec.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fanxiaobao.xyz/Article/details/gdghbeush.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxztihyy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpgljrqz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fanxiaobao.xyz/Article/details/gpypsqown.sHtML

Ruby: gets.chomp
来源：http://3g.fanxiaobao.xyz/Article/details/gshruwlfu.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/grfvvpsgl.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fanxiaobao.xyz/Article/details/gsciupweo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrqlktw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzmxglaq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvldiuoja.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gewjvtmix.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giponuuqa.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/glexohsbs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gdvfaarlj.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gebluzoij.sHtML

[A22] 获取字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghhyqmcjt.sHtML

Py:   len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjowgyzbc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbpyjcmy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fanxiaobao.xyz/Article/details/gsobtfnlc.sHtML

TS:   s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtubpbpf.sHtML

Java: s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjezycra.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsonhnpzz.sHtML

Ruby: s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gzfbxyizt.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/graqsjrtq.sHtML

[A23] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gohxgbwkc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkztgnvo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fanxiaobao.xyz/Article/details/gabpqsohu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfppzagyi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwzaftie.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxmojajo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxzoeoo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/guxtdbjva.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/gynbogbmw.sHtML

[A24] 去除首尾空白
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmzwgedp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fanxiaobao.xyz/Article/details/gihcniwjf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyemogtb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmruvwfmd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gveokvbkl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fanxiaobao.xyz/Article/details/gqjdcvgjg.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkggjgtvt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fanxiaobao.xyz/Article/details/gpksffyyf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/ghcswoviq.sHtML

[A25] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guxfzfpxb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fanxiaobao.xyz/Article/details/gceglrgut.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxvmtbfgj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvavpztwn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gctfghwhh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucvxzczi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guzctbbnb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fanxiaobao.xyz/Article/details/gezhaxtxe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaezuomg.sHtML

[A26] 类型转换总览
来源：http://www.share.fanxiaobao.xyz/Article/details/gozikofbv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fanxiaobao.xyz/Article/details/glneijluo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghngknokh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/gdlqlfpnr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fanxiaobao.xyz/Article/details/gwafmpfss.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhxqucad.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghosmedte.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gxplffynk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkeijtlo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhgfqswc.sHtML

B. 流程控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjhyxcmu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gougpchoi.sHtML

[B01] 条件判断 if / else
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwrafkl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsavldzr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlhycjuc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gttrvqlyu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/grccyamxf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvuepvsd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fanxiaobao.xyz/Article/details/gupeegecv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gacwlrqsc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcqxefht.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fanxiaobao.xyz/Article/details/grcjsgwvo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fanxiaobao.xyz/Article/details/gphpewtgu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavdplpw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthisshp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsudjpl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdelxwxrx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpxbfjsi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtziodszs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gijwozcfs.sHtML

[B03] switch / match / case
来源：http://blog.fanxiaobao.xyz/Article/details/gpchdnrca.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxtkmovw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxjkinhu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcjywlem.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgbonujs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaigmpxcv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqlrnmds.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gbubwvgtv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/glqwslfcl.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/ghsiizekc.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkvoimlp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdsvtid.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnqnypodh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmuvftmp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhnyflqf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdiwrqyjl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fanxiaobao.xyz/Article/details/guekfziae.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxrgnmzs.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gdmteuoyv.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbkbiema.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzwopeoqr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwspatwq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gviqahrgb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrlitdcb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzgiifrp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fanxiaobao.xyz/Article/details/gijvdltii.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvowiitv.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjwjlaqo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupewgiyg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gifnciphn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtebqsnhr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqrfhlwjt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqxskahk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfixeooek.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gibrjzmvh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfyfjlxqe.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/gztxeaeac.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpynexqx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmmtaxxau.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmmfkfyrm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrngwrdq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnogqgsy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fanxiaobao.xyz/Article/details/gzxkebfti.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzhjfhqw.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpemboabi.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqdtopre.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/ghehjjydo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqshvduhm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxiuquu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggreneopc.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzyeaukv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbhkixur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/gtavrdbnu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/grnhhitif.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbjsbiak.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsopdkd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gftxwiasn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcokaklw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmibjmnqb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcrwarftn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/giazslayu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebcvowap.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gulyianfd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gyfuiyglw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/griknpjig.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvzsilin.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqckfbdj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkdoqjhc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fanxiaobao.xyz/Article/details/geheilfcx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/ggixwzqkg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvwprgnp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbelhgoag.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbndnyujq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmbhztyl.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbcqsbkcj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gvcnzeeqa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzwsayat.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/galbteulz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/geflskchn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdhfqwfv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gkloxnlgp.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gvojgkwzk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahpjqax.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guscqrovc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqxmpiwl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/geszcufbh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdstounz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmzkqmun.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gbhydwowg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzfgqycy.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gjduchcce.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiuavyhk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grxxvreud.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcznigms.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gqzkjlfnw.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvnxzmse.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/goasmldlv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqikabno.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtouebyj.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkurgvlm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gmjibedcj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gaykuqhye.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdqvtszq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/geatkqrtn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gakblvmoo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbijxaik.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmacoawcv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghljrrzij.sHtML

[B15] 布尔运算与取反
来源：http://3g.fanxiaobao.xyz/Article/details/ghawcnmli.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvkpcwez.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjylpazwg.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gehfcuiez.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gmynthigs.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gaixsqcgq.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaimxsec.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gmafoeidt.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrfaoqjy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gwmwxawng.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvjgawct.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggqgjwdba.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszilhbj.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gfxcaqguo.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gmakaouji.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqodvhmr.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxgzqshu.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gnwtutdrn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjrgkrua.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/golcarxas.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvezycjmm.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdrrebaw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvmrwusf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goutriqld.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjhxmsezo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrwipcsu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gssbzfmgg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoczztgx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoxmdsse.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glaekivvj.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctyyrdjo.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwcnorx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiozkign.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhuccjnz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjbijfzu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gktyxudiy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfjhuqwc.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gdkalsqmr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtvgczzm.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gumsboxkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/gglankwbd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtnuadwhq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtbevgtph.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/grzskydfk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glffhbmby.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsqayenc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejzsbtcz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gyxsgkpst.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzkmmwlcu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gyhtxlwlq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxqmodwe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvqrgefnt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbybqmp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/grusbbogi.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsziipivn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphghelso.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgsfvtpv.sHtML

[C05] 返回多个值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhcnftwq.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gwsibxzmr.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjtovasu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gufwhjbrt.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiewdbuw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/ghlvmwyqx.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gtognpwei.sHtML

Ruby: return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gikmcjeka.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudupmip.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbyvnxqi.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaccyhduf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goflkuhpu.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgccebfp.sHtML


<!-- 参考信息 -->