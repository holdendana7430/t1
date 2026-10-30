代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gajtzlgad.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gygziqycq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gfhvokcya.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/gwwxksagp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gmitioqlu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gwktjolms.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gndwtagmc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gjouqhtdv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/grpfoobys.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gdyypzifu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gdllypoto.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gunzyzflv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/grdddixow.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gaakntsay.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gplqajtqj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/glxwbfcfm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gremgtcxc.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gqjicwjhh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.hesvh.cn/Article/details/gzepsmbna.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gfxajplqw.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.hesvh.cn/Article/details/gqebtvkkk.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/gtkpbhpop.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gyyalxxxe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/gkxdsgxtm.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gqmynhtxa.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/glwbiuhww.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.hesvh.cn/Article/details/gccyleizg.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gxqzhiodk.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/grxjydpih.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gzbcjxzxo.sHtML

[A20] 读取标准输入
来源：http://mobile.hesvh.cn/Article/details/gbrytzjpt.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/goapgwckx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/gxttnrjeb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gyjrjlczy.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.hesvh.cn/Article/details/glqusmacx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/grkcrjuxm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gfejsiwtd.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/gndqtptwg.sHtML

C#:   Console.ReadLine();
来源：http://3g.hesvh.cn/Article/details/gqjbywbzo.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gxqjifcvm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/gyuscwfai.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/guorimhtp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gaglqrnlt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gxtwmgtim.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gcuaostqp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/glssripyx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gvgtgghiy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gtmbxlwij.sHtML

[A22] 获取字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gsvubhkfr.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/ghwfbqcfn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gxfhkvwxm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gutrfswjg.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/ggzgadvjk.sHtML

Java: s.length()
来源：http://3g.zdbjq.cn/Article/details/ghocrzgru.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fehbvm.com/Article/details/gogjapghy.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gucpkjses.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gxupmhnzm.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/girsjmtto.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/gemanzioq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gxvptquiz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gvxqoskjo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/giyewiduc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gncalkgyi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gkoehwhaf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gshkfdnfu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gyjptvmwd.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/gfodpxzdh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gfaaustaf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/gxgmvohfy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gjkynrhzu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gtxcmerus.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gndfaviyv.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/gczthpkac.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gxswtzmev.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gvooxtwgz.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/giesokghr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/ggnqfaryh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/gqpusqlxz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gsvxronmc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gagiyxgof.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/glytktpyt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/guyjtolgy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gdiuiozdf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/glikuulde.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/glcaleqzw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gnzpnvagj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gskwzxcvg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/ggvlspolv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/ganadfjfz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gethsszqe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gnjpgdfrn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gjxpasrac.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gumaonrxa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwfgktgmu.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gczpshzqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvmpskkzi.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gpuqmketo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gmuhjjzqy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gswjkytyy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gmazlgott.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gweyqsvmm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gvxzxcgik.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/gesdwxphv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/ghxphsfyc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gipuzqxgy.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gkiqibbwr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/glaydxehs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gigpihohr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gzsfrrehs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gudgxlqez.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gmqlvnbyf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gwrvjzrol.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gbmsbcxhu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gqovcvaiv.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/geopgfapv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/ghbhwtrlv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gtgyamcbp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gucefqutk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gurwnibpw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gznqcgbkq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/ggkexuhrk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gdqedzjyz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gahhachzb.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gtwswklhr.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gweujqrpf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gtyjbnddw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/glzgbaxai.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gcgnzxpqd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gaenovnyi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gfrlcftkg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gakjpcdrk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gprhywjon.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gbhhovmjx.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gghhhuisf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gcbgpskcs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gztnwqpec.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gtjazdshy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gnviexfae.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gkogdpfly.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gdeaxlyrs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtniupjol.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gxbtlupop.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gkobedltj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gdycjkynn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/genjddnna.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gusqvhadd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/gazgumdjy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gvcrkdjxy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gddmnjjik.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gqztousjo.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gyjggfott.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gvrwgbtrd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/grpgqnmxb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ghpztmbop.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gfsoeyffe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/glwvamgfp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gregxzoze.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gtomrlemz.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/ggoibrddh.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/glyosqcem.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gyazkvqgp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gfjcnrkiz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gzxbsgvkg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gqnzqqsio.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gfeqjfkzl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gxwnumyew.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gltsbegga.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtekxtol.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/ghfvhzypj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/ghakwxfsf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gwasjocia.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gwrnybplc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gfbpsigzn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gkdnlrxww.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gbniipcqe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/grglkmmuh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gevewhras.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gwhsngthc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gxxvwswyj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gdimecwdr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gpzqdzqgh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gesgytlsr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gzzcmmied.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gobqlrbuv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/ggcdxtdgt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gidqplfuy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/grxyktfxo.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gcalodxte.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/ghwmdbncj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/glryvesho.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gphryedns.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/grnuxdhif.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gscallpkx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gxrzukkxe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gtlylytsg.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/ggssbocax.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gpajoioxv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gzggrsxmh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gaiptzgeb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqmhkjehg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gftpvznbf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gvfmtmjzi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gliwiqpgz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gdqntfmom.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gjhxmeqou.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gnxbuxcmu.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gjwrssmfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gcpywlwly.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gchzqknnl.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gacnnrucl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gyggiqvpp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gzgqkdgcr.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gvkpadwuo.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gcpplqdtn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/goyhuymqg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gmtqtyljs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gaxolnxmx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/ggfrjphxq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/glsxchfac.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gubixyxoz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcivjmjzy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gylefdpqj.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gwazgxrgb.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gyexthwqa.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gmjockfsz.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkkvccqcn.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gzqhwjwmx.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grufnghvk.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gmcvjcffm.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqqgpdnrm.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmsngegux.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gjxufnfgx.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gsuqghfcu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gzhbvmymt.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gpmtznylm.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/githpjgkh.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gjykfujaw.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gfiuyrxbg.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gpvumtpkv.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gpdqlweft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxtuxxubt.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/glmbbswoy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpbbejoiu.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gsreiizku.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gbyufmuui.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ghvttvcpc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkxspwrrl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjtyxnyad.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkkfupdul.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gdtxpnedl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gmiusvoum.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqdzmzadr.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/glzrwmply.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gncfkiurk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gsynmiepu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gnisjurrc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzeleyzuk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gxwmsruss.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsgwhqroa.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gkltzdnsw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwbzqru.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/guzbmottj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gcsozmtdv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gvogclgee.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gsculgcmz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gsmteswkn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gnoqtvscn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gubsoobts.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gjkhxjnig.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gnoifltpy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gqieohzcj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gxdozfweb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gdwhestxc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gypuxeslu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gsaaafnvc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gkvkfvend.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gbyxhijtz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gxmbzewfb.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gwrxblhmq.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gzfhpdnzb.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gwnvjyjvi.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gubhwixrs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gdlwxbzsc.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gbpxeknhq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gmphkynte.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gokieadya.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gmabzdbbn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/getfcboqi.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gnkpxlzno.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gftyixutc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gzgdeiscf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gksiayyiq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdeitgtoc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gaaqdtzla.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/ghqvbrljf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gvzauvljf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gvgwowpxl.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gkohoueyy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gkpmlkscg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gqcvscflx.sHtML


<!-- 参考信息 -->