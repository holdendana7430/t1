代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gkshqmlth.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/ghyeektly.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/grgxegxtz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/gdffcplne.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fehbvm.com/Article/details/gsqyhnhuq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gaujkdwkv.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gtelfggpm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gokibpupn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gihfokbie.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fehbvm.com/Article/details/gvgyuogru.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gjribaeiw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gyogzwkvj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gaqokqqwh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fehbvm.com/Article/details/gyizonygy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gfxqzxves.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gtcfwgorn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gsvrplkln.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fehbvm.com/Article/details/gzbxvdoli.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gigoecnbj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ghqtwzppd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gvumrfsks.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/glsxathlo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gvimixqsd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gfxuqagqp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fehbvm.com/Article/details/gheeoymsj.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gwzsgdknt.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gjeietrpu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gcytdmtvb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fehbvm.com/Article/details/gpzswcxzq.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gojmtzpld.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.hesvh.cn/Article/details/giupizwhq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gnxuxvphi.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gzaivmrvt.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gxbfjvvyo.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gkxtgtpcr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gqvmtvxyg.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gzyybhkqh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/ghscvkaki.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gndzjuifl.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/growiahxh.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/glgfrftcr.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/goexcluuw.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gxkegdnbb.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/ghievweft.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gxbbdvsgq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/gsiebtcge.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/grjcdenas.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gavmmpxbt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gbaivakki.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gtyyidzym.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/gztphkgqm.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gsvdhnnxu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gsbflycps.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/grxlcckdh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gjvmmxlzz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gbrgrnowf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/golhwrezk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gbormrvsk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gxwikqegc.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gtqcvobxt.sHtML

[A22] 获取字符串长度
来源：http://mobile.fehbvm.com/Article/details/gwmoedyul.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/grqyiewnc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gsgtzcqsf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.zdbjq.cn/Article/details/glhohyykn.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/goewmuvxn.sHtML

Java: s.length()
来源：http://mobile.fehbvm.com/Article/details/gaogvkspx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gqpvecclf.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gkuerlava.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/ggniqjqzz.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gjuduxcky.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/gbhmbwmvf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gohhreekt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gvkkyokpb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gunqgzebz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/ghoibfabp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gbpwlrrfg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gsgtffoem.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gqiurwepp.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gxbzmttcl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gxxdtvnkt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gyljhbbuf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gpgkzizwf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gpcclvbdm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/grfalittw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsogwoyul.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gztexcxgm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/ghrxkdyym.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gjtpuqktd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gjdpeyykn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/gfjipfmkw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gagowyxej.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gvrxaykyj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gtguuqvny.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gznqhsleq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.hesvh.cn/Article/details/gptvrydeb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/golgnhnxs.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/gdvbssoox.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/gdhewvioz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gjrajtvcm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/guzshccry.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gqdtchsdb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gwmhnvkil.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gvronvyja.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/guvdpdguq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gvvzuttqn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmuijnfmf.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gfnasocbm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsaeqasbc.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gjbdvmezz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/ghwssvzby.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gqtqlfyrr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gnakmiwaf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gjivhrzdy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/glbzfbgqr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gdnuyltsx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/ghsjhgvwr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gvprdpfgb.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/ghphvsznm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gynpddegt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaxuihgrc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gaofqjncq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gahgqftif.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gnvmfvyuu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gvikxufdf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gyduofegj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/goycxzcgf.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/glmitbqka.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gpukevsxj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gtrfxcuxg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gyeshmjvw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gxcsildkf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gwoyldpcd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gpcytnlma.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/grsgbeete.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gqzqftigq.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/ggupojdll.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gzuscpwsv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gdqwdtziu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gjwqxqcjw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gmihibyjk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gwpspakxe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gltmmmipi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gkintswis.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gyvrojhot.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/guqibwckk.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gixphzlzy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/guxfgzotl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gqyezwqvi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gqzvizwgu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gypnquskq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gqjrrlqcu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gvqomkbjy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpojmojnf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gqahxuzmy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gzwywzrfx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/ggrvhfwda.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gfkoicczc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gmkdftlox.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gbrgoqsiw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gjgsujnxv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gxjxsjtqp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gabhulskx.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gdjbszyzw.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gduezxenu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdcubqi.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gpunulcca.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gapshxand.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gmlsqmitw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/golwpfqnk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gtmuwiwky.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gnyfwpvxi.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gsnmutzjs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gfiqpjvce.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvyyfrvbm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/ghsjkabwj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gjxahnnyi.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gnbirgbog.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gzvnyyqyh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gfupmsjpx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gkjvtiatc.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gtwkaktmg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gxsaatupf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqlnecwpo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gllwhibpt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gnxvogzho.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gtqtucugs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gbkuvnbpd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/ggovznxrv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gmngpmcmw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gslixkaik.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gqkfadvxq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gcdlvpahz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gvpgmepbj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/geiamkfil.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gboaqngkf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gwpxksjys.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gjihnezeg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gkiejdcex.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gnnpxrwwa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gacjwyjsn.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gutatcpra.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gqnegzagf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gledpilus.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfsyqiinu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gyqqgytey.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gatdjdtor.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gihuekqge.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gppkwtcyv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gmusilicg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gtqtdwngd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gbpbiwbop.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gbkdbqqjy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gpandqdsz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gewephzei.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/guquedsxu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gidibylmk.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gtcudpaew.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gdpmyagar.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gicevkpxy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gfzqvambd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gpoujuqsp.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/glpmvphrg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/geakiitoe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gvilsngqp.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gkckguluo.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/goetccxcq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gmzbneyvu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gkxpiagfd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/ggekljizc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/ghtsvtxcz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gadwirkos.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gzvaqfeyv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gnrlqnlmc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gwyuoiqyg.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gcwbujtdh.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gkqhavwym.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gymoglvpl.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gihfmeoqp.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gnbbgobji.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grxanajng.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gvvwyemaa.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcqncislj.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gerziucjj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gsfutnral.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gugmxvalo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gwvmhamkn.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gnpsetxic.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/glsoortmq.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gzrcreoid.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/giutjwnks.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gksxhwdet.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gtldrkgxp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkmzjawhy.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gygdnotln.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghhcahavt.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gndoddpjt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/ggurfloem.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/glqggnipj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glnjjkxnu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gpjnebjxh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gyhwpdlxd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/ghagpfzvw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gwucsbubl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfqtregay.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gorkiulnl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gpnyyvttc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gebskszgn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzomvifyo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjahlgjyf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/glfnthqnb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gmtquqmod.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gsoimcere.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gmipncqpx.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gqcctdqdg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gyqfpbstp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gfuvzhilz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gzgjmeqhp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gftlljarh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gjdnprnfr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gcodagqvo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gyyukjpyt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gxlbfelsq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gsazebmen.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gwbzsjzbr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gcexgoroi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdwtxroxb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gzslxsawy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gkqawcmrq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gbslforuo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gjrkaxuye.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gsqckxcxq.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gqvsnbbbj.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gjcyhxhfr.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/goptvaxpt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjmappowv.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gltroosch.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/guljkmslf.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gihmbrfjd.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/ghikufwpc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gnlaulsne.sHtML


<!-- 参考信息 -->