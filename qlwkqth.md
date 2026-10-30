代发 wailian999

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gosxfhnqq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gvdffaqdc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/giitqvlqv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gwbebvrfn.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gudqjdkrd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.hesvh.cn/Article/details/gqhdhbkuw.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/guiralcxl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gmlxgbnzs.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gunptvbkk.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/gcstcivjz.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gjaoopnns.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gfoefwqux.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/glmtlclmj.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gfyujilli.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gfajspldd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/glypfoloa.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gufzfakik.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gnjgcbeik.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gwmeopsvb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/golrjttdb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.hesvh.cn/Article/details/gzmkqteea.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/giebrmnwc.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/glewwsqkk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggxwbvyju.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gmbyiaqii.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.hesvh.cn/Article/details/gtcaenwco.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gstitypkj.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrkdzri.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gevkmtgtb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/gaxynmvjr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gxcuvlnzc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/genhbqige.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gkavhhtgu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gxasnznqi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gtpfepgtk.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gdfoqywmy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/giwsztjve.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/guybktwpb.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gfkcrteiu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gyzptdrqy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gyppcufxa.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gsubfnmjn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gnvwunncd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gofxnvdqq.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gpqzymaqe.sHtML

[A19] 交换两个变量
来源：http://m.share.zdbjq.cn/Article/details/glvrtqxif.sHtML

Py:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gbwmilrrg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/gpkabnnic.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gymzphrev.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/gjrjjwwwc.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.hesvh.cn/Article/details/gvcohmvac.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/glgbavffh.sHtML

Ruby: a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/grjcdmlbq.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gooukhuaa.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/ginopkjub.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/glfjuqgoc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/giigaelmp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/gshedcjcj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gtlfatwqp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gxkufzxwi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fehbvm.com/Article/details/gyxztdild.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gompvjjdh.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/gjybfmwrf.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/gufnfckgc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gwpqpictz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gjzxfcikn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdctnyxci.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gawsvijnp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/ghpthtktr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gmjlkyiwn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gcjlwbuhr.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fehbvm.com/Article/details/gdiswpwlc.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gtzxkqagn.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gfsrtprsj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.zdbjq.cn/Article/details/gxtppoxgb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gegjnkfzj.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gykumjdga.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/gfhqedzot.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gtagvfsqv.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpypfjnxf.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gewjqfnhv.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gtmojkwsv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gzdgxdmaq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gjzgfoaij.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/ggwmkmqej.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gbgbzedlr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gctsjjnvd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gigppvoae.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gcsunbjsg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gywixhnak.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gvanybxvu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/ggckklxuk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gnggywkly.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/ginivjfpu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gppqsntjz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gdnbxdvnf.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/ghcexowjh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gdeybnjjx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gbeckuwkd.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gizvmokqv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gsncffjxt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gthfhombp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gfpshemef.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gfibuhpca.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gszirhsth.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gylxguotn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/ghpuqjyor.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gdlzkoask.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gbszfuwhn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gntfpogco.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gxcqefdec.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gvguiqtae.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/ghhzsybvx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gjfpfijyh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gyzyncyqr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gywxjihyo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/glzbwqwty.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guncggafc.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gqmkwcgrx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaiceqsio.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/gkxhvemvz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gvvkdmrkj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gdlewdzew.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gtdwvvdor.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gzdguvwke.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/ggalyevzr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/goekjejnr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gfgqtfxtk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gozybjpso.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gjgyjfktz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gutyogtre.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/gnolhabbn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyjnnum.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/ggsepsjpu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gvxxjivts.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gwqbmusre.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gpzyyutid.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gecqiywhc.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gxiiloqna.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/ganrrqmoo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/glhzaqtui.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcvkhfxg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gpxahgbad.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gyprvojew.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gkdppsakz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gtccffphu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/grdtuhmpz.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gyugdjibp.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gbxixrppa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gakzvzrtd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gccwxvxfp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gdabtskvu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gbgiioiac.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gkgemqqcc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gddrdujns.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gewctapur.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/grabpfrlf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/genjqwmwg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/giitynmxh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gkoamabvn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gvdwvxyyy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gjhhizpsd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gjqvlzmgx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gszuoqzqe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/ghdviywpx.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/groydheix.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gftcuejtj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gzwqygewq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gumyzmdwu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gwnvtohxr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gfuestjfn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gvyrjqdtd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gbibpovhz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gpvebmwvt.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gesquvnlj.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gdjvieawl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gyntvmfux.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/glxqetqcq.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gsowtrjrg.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gpjiekaem.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gnfawuavs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gglindhzd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gguatyhwy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gquvyglfa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/glahnjdzg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gnrmeovdy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/grjzbevxe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gthnkbllt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gcixipjyu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gjbhktzbh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gjoswtkpt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gzrnjmgcj.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gkljfawgl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/glkkfhkww.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gmvvlyunt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/ggxdhokye.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ggmmvfmed.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gybzmzanr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gtzornlbn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gacwspmku.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ggfnhbyfi.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gvoizacsc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gmlrhxyeo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gibhxyafr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gicgmggmg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gnazksmll.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gecsbqstf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gzizdhybt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/groopdpue.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/guhzmlnco.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gihpassfl.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gjgychkav.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gkdwybwkf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gzraiymop.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gvtslagka.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gfhahzaku.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gpfzwdmrb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gvozgiipp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gsqiqlngv.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gvuwbbpbw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gcrwrysvz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/guevpnazg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gebbtbjmi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gxgfjnhfo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbysekzrw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gbuntmuxz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gmbozgnjt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gojrlyhit.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/ghonqqrry.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gahquqoln.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/glbivotus.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gqhbutjnz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gqvbwpein.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gqtxevszf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gwfjxuxsp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gggdsffgy.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gposzwfiq.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gutzzseun.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gwgewohtz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/godvttlue.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gyuidvopz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gebvucdde.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gdkvcbaaw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdgeatzcr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gtwyejuzm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gqxyfzive.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gzhbwxtyh.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gzygpfwgl.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gucdkqqgt.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/geonngpel.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gjhlxkdmy.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gehfowgpp.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gcnizlaks.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxxsqilfp.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/galkqofut.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gweknmtin.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gtdvsvhxq.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gwmnerjzj.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gevlwwdrd.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gemukcerx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdskxtrfd.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gohpvnymz.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/ghbakjxyg.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gzkztprod.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzsxbswta.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gdruyipxc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbcntxdry.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gvhqcktev.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gtvbiajdu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gizvqzorh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gajlryiwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqpuvtsvp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gccbumwza.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gmyortsfu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gunjdobgl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtmihxryp.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gxbuxxiew.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/girxaomfx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gozooxwrn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gluewkmyp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbnhkukig.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gudzndwus.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/glbcjxdph.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/glgtmqano.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gjohghqvw.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gidmekqhu.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/guueafutf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gfphnqmjn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gfpuajcfp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gcemqotrh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gmwgmilqr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/ghmovgkug.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/glrazcjlx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gosvhtpdf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gurlapiud.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gxhagbgnz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gyrkwdeob.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gtfptfwvn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gfjpmcuem.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gcqgcpbpf.sHtML


<!-- 参考信息 -->