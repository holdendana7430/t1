代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/ggckxrdyb.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/gouhsiznz.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gyprudsmm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gnhjklqhz.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gfgsaycej.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gjwoqtpvx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gudemsuqo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/geyovoybo.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gttuztjdo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gwkzautmq.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gxrbncvwb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/gcpnwzsrw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gcyrarmta.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gkbvyhheb.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gezrtwjmq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gkgbivvwr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gczkketan.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gnvyiyrhs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gmpqgmcry.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/gvkpxkozh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gsamlosya.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gxzrnefqh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/ghsghiueh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gtfsegvtt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gphwxsxpq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gxzttxwae.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gionedrie.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gqvrqvoaz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.hesvh.cn/Article/details/gseknwprq.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gdmenodxv.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gfltmcmzi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gcxeaqmkc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/ggqrdvwzj.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gqvqeniyu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/gsbczmtmx.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/gbfdweuwq.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/geahvkfnj.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/glaqnrisj.sHtML

Py:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gjpkvkowf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gbvpdukqq.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gwdhtrggj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/giaxjwxwr.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gdtptabus.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gqiulgxre.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/grerodbrr.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/gzsoajkjd.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/goquwbayx.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/goornbatc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gtjmfjefz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/gtgvmilgd.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gcnuieijq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/grmuswoyg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fehbvm.com/Article/details/ggsvhtsep.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/glrwrxbuh.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/gqveldvlq.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gowgcxsqh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gwzovommf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/goosqpwaf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/ghmgbasgn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/grdmfamzr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gzmyozblr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gheqwaahy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gkkkeeegf.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gznyqiypw.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gniuqgqhk.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gkmrhtshq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/glbuyapkc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/gmpbkclws.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gwgxmymqq.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gtodajczq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gkwflibhu.sHtML

Ruby: s.length
来源：http://m.share.zdbjq.cn/Article/details/gspasjicd.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gruoxnzie.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gricsawuv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gbvtddunu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/gglqjtfus.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/giltztifc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gulsplsgl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gusskjpor.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fehbvm.com/Article/details/gnnrsobpg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gdbkyxjre.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gjonzlrxk.sHtML

[A24] 去除首尾空白
来源：http://wap.fehbvm.com/Article/details/glaqjvblm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gsmcmvogf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gbwzmtkii.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/glwibnpsx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gzhqvguja.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gilkhrzrr.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gkiamrfrd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gorywdggo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/grfjbyrzo.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/grpanoyex.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gkyjxocpy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/ggjpmdpat.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gginlxxcb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gnwnefdzz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gqgggfvei.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gmixrwywy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gkdrvnlvj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/goopshrrg.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/goqpxsoda.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gjkwwkkmz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gljgxujva.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/garpyqlll.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gbylavkbx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/ghwuryirf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/ghjvefyvo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/ggqdqboab.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gothiaqvp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gntvfeqyb.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gzhgkoxsp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpmzgveoj.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/goucamdng.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gldffdroa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gavcxbfat.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gwsijjhsg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gufcieupp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gkahuqpyi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gyngiirsx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gnoxostoh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/guropawkj.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gcjyjiwsp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/giowioasd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gcvemxddx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gogwgcqyb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gakxougrp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghzmikgzt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gkhmltvcm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gvojncoqy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gyrgcdqll.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gowzjwjbd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gbhdsbngz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gjcwtnxtu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/goqziilkj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/grnzbbtuk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbrtqwjx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gcvxfgaiz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gksquptqr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/golxsgzxj.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gehbjfljr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gndhvqlbb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gggbohfuv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gthlrbdtl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gbmmykwfw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gboyymvaj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gzbgzejjg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/geprnlsnv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gnpzbuauz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gomydmyjm.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/ghaibkoah.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gpeyuopkq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/grvgkhcfj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gwwzamqso.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gduvsnzdi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/grqevjvus.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gpmobaqrf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gzplgexvq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/ggyylemgi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gjtuqitxd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gsvyukohz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/ghkbbtfjf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/goacgefib.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gtuikynyu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gmacdfqdg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gqxpukqxy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gmrlprkbr.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/glzjikmds.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gcnshvbjz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gpkaocydp.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gczsrusjq.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gvzneaxsr.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gwderdgci.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gpjorxkdf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gcqfkdfdo.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gxnjrjljm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/ghfivfaft.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gpasrantr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gnumlvuap.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/grwoqtxun.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gfpadzcbu.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gpfwnkgge.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gmbdufhgd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/geqncnlsa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/grvklxryf.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gzlcjnbcv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/giqtmxsky.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gewlnmxzx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/giitdtpoy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gnvzlszwu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gnmzilmzy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gmxkparal.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gywchcgfy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghgrmaudo.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gskxnirww.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gchhqkrrq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gussxgxor.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gxhnjccpa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gxqtvppgf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gljpubern.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gtolujkkn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gzggkksps.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gywsdopzv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gpighumcc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gwmejkqyx.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gqgcfyxis.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gyghvozpc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gfsbhkyoa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gmsqdegce.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gpkxhgeaz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gpluvqnbw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmcucuxui.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/guacoaqhu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gbgjdfxvn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gdhijnllm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gbwlyqbfq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwkuhxwyq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gobikrwkj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gqdumfffo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/ggxgjybmd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/grconwcra.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gymfdndmr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gzcfvnbus.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/glsrxxrvh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gcuumshzb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtxyvan.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gjsaqffnf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/ghsasrckg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gvpeimmwa.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gdfpkjard.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gtxpmwjhg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gksikmhlo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/giztadiqt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gyaoenopt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gcilarmog.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gngoljdoz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gjvracqbd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gbymzvdrh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzrwpihkt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gldeuseui.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gsclrvqhj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gewcoyndc.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghysxsbua.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjfhuou.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gwkrubdqc.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/grsoxyveu.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gnnimyexh.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmeudxllr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gntsxujnj.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gxsuirypp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gypheitzo.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwklmuwoq.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gpyxgmmih.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gjbzekcfk.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/ghlukeqvx.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gkjkpespg.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/guabdtnge.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtxcdxesq.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gxiafwzzw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdtufboho.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gdmsbgmzj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gcqfeqecv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzmlcmudk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gncygyubd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsmmdzfed.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gpgayygfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gvlrtdwbt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/glybuisrn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gjvkoxcyb.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gwvharkjm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/ghyccjfqu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/goittntyu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghpoaxlvs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gylfqhduu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gbdnligqf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwioaxkvh.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gadhrjigp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/guquvypvr.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gcmktaiep.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/goekqkbmm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/ggpeluhqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gyhwrecom.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gajloaewe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gozafaozp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gbbktveem.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gnahxktwv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gzxbxqaba.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gbwokypdn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gnnqgzdbe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/giscbnadc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/glohaxtdh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gkvxxoypd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gvlnxhorr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gmqwahvkh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gdxbxrqdf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gslxvzmoy.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/ggmrvklhi.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gwyqifzfv.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gpiqfwfdy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gqajxugdb.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghbkrzvac.sHtML


<!-- 参考信息 -->