代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gqoljlcmm.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gpdnxjtqu.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gkwxzrdvw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gioyttjwv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gqxmwctlk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gelybrkuk.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gxxqzbcks.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gezglrwca.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gyycjmqgr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/gyciojmzl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzptqfzhh.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gmbjwlwlj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gpxswxsxa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gmzojzxpk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gxadsxisi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/ghehphyhj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gzignnams.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/geufneovf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gdrrqmnra.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gmagrshfn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.hesvh.cn/Article/details/gthkvayhc.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gcycopvrt.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gnpfttnwp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gptouotbe.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gdrzcpenu.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/gznhvoujm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gtltmkqgl.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.hesvh.cn/Article/details/geprugome.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fehbvm.com/Article/details/gpuehhitx.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gkaocmvqj.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/grjhcsomi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/guregorvs.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gbnupdhhc.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gfascpodf.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gqhyuacjk.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gdcagsoyc.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gkydgyvmb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gwuvxbzkl.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gscxgkson.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gyoawwzwv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.hesvh.cn/Article/details/gnprarnng.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gwpgbeqsx.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.zdbjq.cn/Article/details/gpfkufike.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gdhlrfqvs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gprgavqhe.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gwejteswu.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gzunhbomi.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/geneuhkct.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/giepmnzyl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gqqaepaht.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gdjrbntov.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gylwlskhl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gzpcxrjud.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgimapvp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gzeubbmbi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.hesvh.cn/Article/details/gmacfhbiq.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gkhepmnlt.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/ghkjgdtec.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fehbvm.com/Article/details/giqabypxb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.zdbjq.cn/Article/details/gisduxmwb.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gplbascew.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/gfujzzhzv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gmsvinphc.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/giyesdbrc.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gajtsfehl.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gtvxizucw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gcygxbinu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/giqvlcutj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/ghryfbbkr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gxqtkwhhn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gkqsflwta.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gcauobxor.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gmmputqxi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gezlawapl.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/garujdmzn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/greniebhh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gfkvrlmjk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gldubpufu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gpiyuogdo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/gfxqmvkqc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gyuzwgzjq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fehbvm.com/Article/details/gheexpeet.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fehbvm.com/Article/details/gkrmzwhsr.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpduppnnt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/ggkdugslq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gzccsxslv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gynglszyd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gqoitnkgc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfuiyssl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gljenwxme.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gltaozons.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gwlyjxram.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gqpxzqixx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gfwijbfdy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gglwkoshb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gjnwetdun.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gryivvbqg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/ghqwoprjh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gzixqpvlt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/glneokrfk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkozvjwu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsakoxgiy.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/ghqbatzja.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gflsbbxig.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/gxlrybusx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gyomjewam.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/grrkwrkyz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gyhxcvuxd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gkzbvoiis.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gylgpeswl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gdcglmios.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gfxccvnta.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gwhkefgeb.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gpjyzdkbz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/geyofelyj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/ggfjshbbt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gulpwhlej.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gyxnqkryk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/glstmzqhy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gwmonvptb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gdsgwptzb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gfdbulktm.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gzpggdahd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gawhockuv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gzhnbhrxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gtlgckaob.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gpuczqvbq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gurrfgcem.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gxgxnijyr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/givmqcenf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gazkefgvg.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gfwfwcjgb.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gcvmvdlkl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/grcghopwc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gryfinnsq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gokglnpet.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gkvaljlax.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gbhdhtpja.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gzgrxicfi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gxbunbdxp.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gvjnjrdod.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gwayzstah.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gyumqbpst.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdpseblsq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/guttftsym.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gvjkxxyjm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/ghhhtfqng.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gqkkmcvjf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gtemgkvmt.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gylgzhgtk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gqoehqruo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/gcaejfpln.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/geapmxvjz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gaczadhhl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/guqwkkpfy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gsbocbytq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gfpeayyow.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gclfeudwg.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/ghydsgpmb.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjpolitpy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gwmvsvmcf.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gufseibrv.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ghdmqzorx.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ggfysmhpl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gtoslusfb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gfdyuylel.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gdiesantc.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gwgljsonh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gbjfkcxfj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/giymwlyje.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gqdichxxw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/goruuzmkh.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/grsxyfnei.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/glucmvezd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/ggyrpsaxe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gksfyfxew.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/ggaswhvxd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/geemaraii.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gorihhxaf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gevhhfzfo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/glrmpjsaf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjhljrzib.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gaxdcohmd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gjmrkcxjg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gvjtucaeg.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gpevtorvi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gbkyfjnvb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gcfzwsujj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/grsgxcanu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gyptstcqp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gdadgccmp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/giuifnkin.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gjwgwuuah.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gjkbhojeg.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gptbaigfn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/ghybsqaic.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/geqrzzhem.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gwbmvovuf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ggvxjofvz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/giynmllpp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gezifhjlq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/geaijlmxj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gxdnpqxvy.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/geurqrtzk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gwnwgwgsm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gqapycbzq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gygoxbewl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gwnjuurkl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gckbdpguk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gqvhnjkom.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gkqswdqvw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gsenxhldi.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gtjsswwyc.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gwuayouiu.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gmczoslfi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/geofftufw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gnadkmpul.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gtscbvjvv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gehhkdynv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gohnaeppe.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/ghflgcdzk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gybdldkui.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gkbsxokrj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gmtmwgqqc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gfgwrynhz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gqtyldffb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxkhvsyul.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/ggjwiljqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gdppauoqu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gduwathlr.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gjwqnoaii.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gpxgytftd.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gqaynubxq.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmcbfmztp.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gtawzhjho.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjzbyxkid.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gcnwstcwf.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gfzsjqqll.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/geewqzdje.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gyjatxudk.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/ghyicukki.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gdbjqzgfm.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gjkxfdjiu.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdxlggrxc.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/glwwivnhq.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gmxcdjonn.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gbuujhmfw.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gtvnyaqly.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbopctloq.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/glwghizco.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsfadnmew.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gehujyjrn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gwisgwgvv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gfhxmzhbv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/glfiaegnk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggfbwmbdt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gtahsfnpk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gyeeayqyt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gejhxcxfo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gugkjoyfe.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gjzoplcct.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gylvkzjnw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gleigeswg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gvdlxdvmh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gpntmgxse.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/giirclpxf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gmbxvpmqe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gjneztesu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gozloehaw.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gocnrvjth.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gbaglmwhp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gasrstvfq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gupocajqt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/goxjketzt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gumplhqkq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gjiqzngha.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gcuhjbynv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gmrzevnpz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gmcjbkzlb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/geowmpngf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gabrlypmk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gwykcwkhf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gsnuwkfmv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gooraunvl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdvmkaghn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/ghbofcvif.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gmcsvnyuc.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/ggnvjnlbf.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gippkqmch.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gednfzjfk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gbffoetug.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gigwsirdv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/giztaitvb.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gfsshnuma.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/ggnbfmmdi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gwkwdjgwr.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gdradcgsk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gfrtgwuna.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gwmqppzur.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gdxoyonvt.sHtML


<!-- 参考信息 -->