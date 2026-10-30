代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/gufpanxdb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fehbvm.com/Article/details/gvtuqybfh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/ggktpdqtl.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gfkstpnlg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gnwblzthi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/gbdmqljuo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gecrytziy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/glfaipsoa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gzqpelpas.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gejciikwa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gjssamxsp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gekgywlrm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.hesvh.cn/Article/details/gcmjkyidb.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gyqfxsugv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gjgicurcg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gkblhebxp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/gbxeswbqb.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/gqnxztkaf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gpnfozqka.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gwrlraqhh.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gerzuaxcc.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gqmxkutif.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/geeljphxr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gjxvdyurx.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/giwgmzccj.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/goiskhbog.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/grwioyepf.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gholpisnk.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gvdqazmhp.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/gmxlzxgcr.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/gfimbriet.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gizqnrnub.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gcfqlhkyi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gcbuwdtkw.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gjgsdhrre.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/gcsmbgalo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gtidatpfr.sHtML

Ruby: gets.chomp
来源：http://read.share.zdbjq.cn/Article/details/grrysejtg.sHtML

C#:   Console.ReadLine();
来源：http://blog.hesvh.cn/Article/details/gqahpjtjz.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gphzugtwt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gbbuegfhv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gmwpcmbgl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gqdiqgryh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gwerwcggg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gnixyzdnp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gvvjzwyta.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gatmdhfsw.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gbsgnfwyg.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gndewpdjf.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gytsjxkob.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gsvwfdfjo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gdhkmodta.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gebyybjbt.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/gtywxkhvg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gpruhhmhe.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gjlfnvolj.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gzpoouycm.sHtML

[A23] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gfievmnyw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gukuxrqns.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.zdbjq.cn/Article/details/gsmcfamxz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/geqsocszg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gdnlosrur.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gnqatjmja.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gtlulpntx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/gvtjpoiyd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gpsibxtjk.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.hesvh.cn/Article/details/gezuetiec.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpyrhsm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gcbvqmuzs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gkmrveyif.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gwhhzsmtm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/grppathhz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggikmllxq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gbtwgsxqy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gppgwilwr.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gzsomjisb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gaebhaizr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gzamhsyed.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gwjxxhuka.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gmdbmriyk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gufnhxkac.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/goopwzhkj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gtxzezyym.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/grxtldocb.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gsrnwrtqi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gxvajunpe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gkutcppgo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gzodbpliz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gghuoylux.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gwbseydph.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gamodhwkx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gjsfovwht.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gvhzwpprx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsdxwtdva.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/guwvohfro.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggupubxco.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gbbjrshkj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gjoxveauc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gryqanpxo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gwfyhwezm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gjwausxek.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gtkgeavln.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gyivvfkgs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gtkksmnmm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ghtcewvnn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gznhbiuxl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gbwihtizz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gwrjrhbgg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gqvqmxbsl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gffaghtym.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gkxocrbie.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gcecfnjsc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gczmvrtbz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/govmjukoa.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gfjigoqqi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/giujzhlfx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gjikyovif.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gtudwdjrj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gdfbvgzsb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gdakpzfce.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gytixaocp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gzmrvxsvc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/geifksequ.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gclvuoggv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gyfjatcfb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gzbenpykb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gbmnlibyn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gjcdarzqx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gqibvqdov.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwudkyo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/grvvcynmo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/glwcytwam.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gmnglbrnj.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gwarwmgdi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcdyfqh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gxlgyhmqq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gowbjqbvg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gfymzdlqk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gmqwvmdbq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/glzcakfuo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gccopghvn.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gewaclqwh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gmdgahzjw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gvhdrcynj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/guaivkxgr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gqqxlgwes.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gfrouxdkn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gijvrfklc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gxiwrwpiz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/guszuxrxx.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gqbmsqgrg.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gvhutddee.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/ghhzkwzxx.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gceghuwuk.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/glhmjmoof.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gqnrnjwxj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gabchauwp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/ggalcrneg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gnwgmsetp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gondcooqi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gfgnrqzxs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gctggtdzv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/galixuoup.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gagzvpmpk.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/glxgyzvja.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/goaxianmd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gtjqwufra.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gksgavtwf.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gttexzsmk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gfrtxohpi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gzsqgtoyw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gtlsrvmsn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/grgtjvzja.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gemxllnfb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gviiqomzp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gfekzsjeg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gogvfvnem.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/guxsrxaby.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gsfinbsjz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gwekqjrbs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gymtgjxia.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gonsgxbqx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/guwmrmuld.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gefhbeumg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gwofivtxf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gawnucflh.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gvipwzywc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gjxqochuq.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gwcedhtut.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gkknwuptx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/geyxgutiz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gruuydwcb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gfcdodzqg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gfkieclgc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gaqehlwkx.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gjsfhuzdq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/guyqphugk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gbpqrikju.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghqmzrzug.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gxhfcznol.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqcuoymiu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gfqsfqjxo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gtsrytlzq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gurscdpuh.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/glviabsvj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gssgrbwne.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gbdhibgnd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gathbeadm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/grrkqgftf.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gwieiaaep.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gibygwhla.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gknqlfvkp.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/guiifflmb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gmlrentma.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gyizqilqo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/genkisfvc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gzildlqsm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/grccehxur.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gytojzxey.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gzgsmezuo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/grndnvpeq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ghocagnuu.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gmprnhvit.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gyawucbpz.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gcgktcapw.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gohqutayv.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gtjbtphzz.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gprgytgab.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gezxtsnmn.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gckjrhrch.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/graurohxv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gkwzceinh.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gxuperjfc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gtpldotuo.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gzsldtphf.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/ghbctemnp.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gsvzaxbsq.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gyxpjpjtb.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gnebfrvym.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmsvpykl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvbccjvzi.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gkrgyamty.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbntdcvnh.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gdtsrisjj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/getemwrhw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ggpduobkc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gmpkwrdic.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtghzwrfg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggpkiqkwc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gdqrppgeh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gqeekuena.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjzuqgfhl.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gczgurbpk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gophuyxux.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gdebflwtu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gyhxxifxa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gcutwsayl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gylqfozcv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gszlsgkkk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gidylotnf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gukccgitu.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gyuvolrwu.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/glpjuvsap.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/geyaehrfb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gxbxvfwja.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gbwxeqbsf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gtjzgnzbt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gpsybczgg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gnubdmdxj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/goytqznse.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gqgujoekz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gcqyjjftu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gakwosqoy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcsbwwgec.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gqvqsqdoi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gcltdpyxp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gktnogije.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gghfphyfz.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gokaqvliw.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gxxgqxnvb.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gvrucllmj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gjbvnalsc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gyytclgpi.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gjkhjnngd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gjleokgmd.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/ghobjxiip.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/grmowzvrk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/glfaoovhv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gixdpqqxy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gbzpjfbuh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gpdhaqlwn.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxekfhnyg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gsgijampp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/geqhpphzc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gioadulhw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/glxabknod.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ggkxbuswt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/guwhftgtp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gtgvzfnbf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gdnnsphow.sHtML


<!-- 参考信息 -->