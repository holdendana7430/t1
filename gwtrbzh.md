代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/goyzliqae.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/glkzpwlyc.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/giixgjfxp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gdosxqnjk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gjjehfpli.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gtkavlstx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/grdaobcsx.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/ghmfstcqc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gzybvyasr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ggeivdnum.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gwtjqfnpf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gzgxpwwqj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gdfnwnxwx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gjhssboup.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/guhkqabzx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gathmvtix.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gucmievkw.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/guvaempce.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/grbxdbqip.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gjtqtmlsc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gqqvduzaj.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/ghjnqfspc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fehbvm.com/Article/details/ghamwnnpl.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gkhmxbnjb.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gljelftkf.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gwgiepeik.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gtvfmmmyt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fehbvm.com/Article/details/gnckluwhe.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gisnkgjgn.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gnbyrabqb.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/gapxtteek.sHtML

Go:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gcooviuib.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gklrpslll.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gkaoplcgl.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gfkpprkpy.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gacuevxsm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/ghmtgesmo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gddkkkmqx.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.hesvh.cn/Article/details/ghlqxqwkm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/gzjicxqqu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/goyxzjrnu.sHtML

Ruby: gets.chomp
来源：http://www.blog.fehbvm.com/Article/details/ggpujkhgi.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gmiteickh.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gzgjyofeb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/ghsiatbbl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gvmefyoyu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gxxvacznt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/geylxmvzh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gultwkrsd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gpzisslqc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gjllahhuc.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/gfpddgwsx.sHtML

[A22] 获取字符串长度
来源：http://m.share.hesvh.cn/Article/details/gekomlipx.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gyohdyopq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gucazmhrw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/ggxqzsnyi.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/guonaemsq.sHtML

Java: s.length()
来源：http://baike.zdbjq.cn/Article/details/gsyzyuvdd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnovelbkt.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/guwfibmjm.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgokbzl.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gqwhwqqhm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gtcofmjyf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/grxfacsda.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/grcggddty.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/glsrctuyq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gfjvgbfkr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/gusirqaqs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gfmfvsipt.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fehbvm.com/Article/details/gbinzjvbu.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/gfxkerfly.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gtxznmkav.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gayooojdi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/glkzrmlmx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gkyslqcsb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gitkuhsne.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gzfkswuel.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/gdupgtxmv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/glipydkzt.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gpehzkqlr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/glixyblwx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gvwthmswp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gkresolly.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gvhqaoeru.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/gvvlxoino.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gcsbvczlc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gbhsqdnqf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/ggclermoq.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/ghburtjns.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.hesvh.cn/Article/details/getkcfmii.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gfckbdzpt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gjkhpxvss.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/ghqizrapt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gouqyrosq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/girclrpgf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gzondiqck.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gjutxajfv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyzhgmjsb.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/gwgyihwqm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmzceaflk.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/glkfzqwzb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gzunorzpl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gntbmjjhw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gpwjoifva.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gkdzxgslf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gdpegrxkr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/grpbqlmiy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gklcjiwnv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/glrtdegdd.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gvdisvujw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gjlujopwa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gpdurjysp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/geyzhykql.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gozrtrcqw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gxcxsndbl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/guzwabqui.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gsqtknuma.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gqoeovtew.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gchhdbnqw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gbbkjphjg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gcudrmdti.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gkreikppk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gxvlkgyqi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gvzwelzjs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/goieeslhf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gfjhcpznv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gscyiuyma.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gvbkttgtu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfehidb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/grydfvkct.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gxtdcfohw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gdmllaavn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gghuclsoe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/ghtoyhduf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/glhlsoyzr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gmhkwbfny.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gwjcibjzw.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/grwgdmezn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gifzvcezy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/garzpacyz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gptgdqnvz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/guuxdscit.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gwdecngxg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gkerdlrrl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gjjsrecwn.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gcgdztomx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gzbkrdext.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gevkzbgdd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gemblxjpj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/ggzvjztwk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/guyhbzfet.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gkyebcudi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gzxpwvpon.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gviyhjrki.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfskdawrw.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gtnikalna.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/ghcmcqryf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gvrpgfjsc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/grspdlwas.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpircymdn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gdrcvfpfc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gwatkoxkd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gaoalfcvq.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/ggitjbkrf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gostwcshb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/giyjqncvv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gikujfteb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gnxuqkiyu.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/givazpolo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/grwgmrsvu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gdklsuapc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbthnddnv.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gricbhstj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/ghwfyzxym.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gbbleqwdm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gmwjgrkjc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/goapmjbqv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gskbjauni.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gktmcwdpk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gpmmfpiko.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/ggtzelkmi.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gvigdtxxd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gawhsntjt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gjegrwhem.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gxwbuitno.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gpaydpwkn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/giabaqavz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gteewtlgy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/ghqlrtxad.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/geaqowcuh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gfjtvujak.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/grcdvybfd.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gaqwrbead.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gijoenogh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gbyspblcz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gbregizmu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gxdoiscyp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/grmprales.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/glprofvxb.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gwfgxgstj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gkaoqhckf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gwxqzljvx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/ggedvycbh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gccoffbyv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/goifksvty.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gqzfjhpuj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gfevzwbjr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gzawukrqr.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/giuwxhftk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gydwqrrtc.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/guvhtyuzx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gzmochroz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gehaanlbp.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gbjtoelhp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gyakdlcol.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gtkxfkmib.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gkaqwwuby.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gchfejypn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gkdwywhpz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/grecdiefi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/ghsnqqhlx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gypslwlzp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gybqkrhqg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/ghqmnjybg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gexfhgcpb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvmuimq.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/ghvrgvbmi.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gepdzecnu.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gcjwjlvxn.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcpfhxgba.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghudejvra.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gyekblhnp.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gogqvrqfg.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmovvnzqq.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gehaykdnt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/ggjbacvss.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gfkjjrzea.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gjwyvyzxj.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gwbxpviyn.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gnqzvftgg.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/ghgszgvck.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gjvfchypd.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gimnicaxg.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdktpyfmq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkeslpmts.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gjfasebmt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcgnylkqd.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gvtcfproe.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gquopztvn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gqvxbmzrr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gugbigyki.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gdiogtctz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gxkiyuizp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gtdsrpxda.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gevevdshd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzkbeuvho.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gwbezfqkt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gdffsbmtn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gccltgkjh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gvovehgis.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gbmwfario.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gwxbnvftk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/ganoxbciq.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gxpjhgead.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gvbpcaicg.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gdztodmor.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/guxmgqfir.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gfleqblbo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gedvwhgqe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/graouxgjs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gzrfuzocz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gnfjzsxkq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gvvvlwrcp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gpptkdvei.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gprreprcn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnabknowv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gmfwihfat.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gifytxnec.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gkdcixwwl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gdtkwoubs.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/glexxhdaw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gklnfupzc.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gjcafvlbc.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/ghmpbgmzn.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gvhlvfdwf.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/guhokajkp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gnacsylad.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gxlkrngkk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/galeelpxu.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/ghpcxufde.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gvxqnnggj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gsfpehhul.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/glrcupzrj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gujeausyj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gsmtggxkg.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/galejtskr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gljteywqc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gydkhevqw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gpnrktvni.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gnznvuyjg.sHtML


<!-- 参考信息 -->