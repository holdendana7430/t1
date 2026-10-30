代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gjdbkqkxp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gzykvlkwc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/grmmppzkm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gkkeozxgd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gjujcvawp.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gplljvjae.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/geawhznuf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gybjzlnyd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gkahghmph.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gdvktojmf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gvqszlvki.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/grvhukrnk.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/gbguuuecw.sHtML

[A19] 交换两个变量
来源：http://3g.fehbvm.com/Article/details/glgpfwqek.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gjofbembr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/gzddrbhsa.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gzxiusfgj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gesxnpdfo.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gpzsbsbqh.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/ggqehpbmu.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/glaxxzwso.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gevwpkdly.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/gjbpmjjlk.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.hesvh.cn/Article/details/goimcdxag.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/ggxwxpzmr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.zdbjq.cn/Article/details/giqzygtfk.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gwcvhiltx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fehbvm.com/Article/details/gzkacuehh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/giaoirbxw.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/geycuwqpy.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gvydyuhyz.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gtwdolsmj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gmcupmgee.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gpdmluzgp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/ggkoarcec.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gadwvhzhu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gnviptsqz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gzaobzqfk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gewlyaaqc.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/glzsemxbg.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gxmwafvje.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxwyxls.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gbkinmbkh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.zdbjq.cn/Article/details/gzxvfuqzz.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/gwuyzielg.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/glcqnthas.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gjrzuzpjf.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnmpovzlk.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gskqcujtk.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gdmlxcvpb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gwmmumzis.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/gcwymhcip.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gztygifkf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gsrnadfyp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/glbxjigyn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gsimnaaor.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/grcyxcpzj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gwrsfwpjc.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/ggnnsjukr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gotqihwiq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/guuhguoyx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gsbhptkte.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gnaluuyzg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/goviaztoe.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gzfyadnya.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/groziecie.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gcvzyhafo.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gcrguznkw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/ghmvoojcs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gbgumgosb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gnqokzeqt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gapttslax.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gvjkojhbc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gnjlnwhbr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/grqmldfsv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsopylsyd.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/ggfeofopl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gebtdnqaf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsguxbad.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gozgzpfzp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gntumtvbk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gkvokizev.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gjpotbtqm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gvqltkyjp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gtmsgnftu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gakvoqmij.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gzjldqgmj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdbauzeax.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/ghpsrbvoa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gasnuqdad.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/ghmkqktws.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gzinxvxod.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gsttggdjo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/guiqpbgkr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/gbfzzciln.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gbvrxgzwh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/ggbvlgtlw.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gmzbgzyuv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/glqwmjxzi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gldhylptv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gpcljikhn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gqfimperv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gnbgzpjzi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gcxwrclmn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/guanthakp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gydubhhln.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gmbwpvbsz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/getaxvqub.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gftdarrof.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gtikiknnk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/grievzeoa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gdxparxul.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/ggrpzykoj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/glruskwef.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gjzcnafin.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gkpjqvxnu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gupyqzlin.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gdkengcwp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/glhooxyql.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gnhtwsube.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gdhytpzwx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gbtwmnepr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gershsxco.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gnbzywblx.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gbbwcreua.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gycjifven.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gwybvhiur.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/ghsypbnng.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gbupbatno.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gekvmrrmc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/glawuvxix.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/geisfzblu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gyvxijzco.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gijsddwml.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gobtmdmnv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjgyjoldt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gfuveskxv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/glxxhesko.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gxcnaozul.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gjaeulvuj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gnnjauhbq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gnpostxta.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gkvwqbltr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gmvsmvzlz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwlfarpbz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnmvqvvvb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpukneoyh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ggifkulli.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/goquucazq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/guxvvqzjs.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gsovfsjmx.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gkivfhhcz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gpunhbhxz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gpatduxjv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/grvqmpzfc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gsyttfkbs.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gojrvowwq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gszkeofly.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gvvsqixns.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwyjgbbok.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gehblwutm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/graddqivt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gokyacsac.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gcbffevfw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/grempvtrm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gcqfdegdw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/ggqagotzt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gewkosxfh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gulnnzinb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gicqouvtu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gyqppshqo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gyhdizvsx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gwvkyuscw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gbhlpceur.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gnlzscjzi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/ggzfcncos.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gbhmliqho.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gccvfurda.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gptvfmdju.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gtckdfmxy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gmnmlzdbp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvwoocopj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gnwwlvpgv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gzlsavoyl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gswzavjqy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/ghgsaawss.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gamzxahul.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gabgsyimo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gwbkcvsgj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/goplxuval.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/guzhqrswj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gbqlcysfd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gynmkbssy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gcfuoiibs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gtkcibxfv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gcbbgzoth.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gebagykvg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gkacuqvfm.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gmbldcrfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gnwyowlpw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/glwbrxlrf.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gknmrsmfz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gqpurvujf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gdaiddmvm.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/geoiwsmbq.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gybftdgvg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gisiumoix.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gwkftsquf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzfntgclz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gixfctkpd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gedimnndq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gwoanflnt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsatojeko.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gvitqdfqy.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gbzdkzzum.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gpuvaozmt.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gjgnywxlj.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gpylajprb.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gspkxyahv.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gvcgfaxqv.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gudftvrtk.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggvmcdlcu.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/grjeoshlm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gfvhvcwif.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gkssoysji.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gnmzpwjcj.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gnosmtpye.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gcdhlbpum.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gidgaziim.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gjcyvwemi.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gnwekmope.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gxguxvflf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnaxizckh.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gchonqimo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjzquhdwo.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gizchhtzx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gqicjffcr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gsthaecin.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gybuozwww.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvbzwaqce.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gccwgycuh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gwgdqjegq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gjoocsmbz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gplqnvglt.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/ghldgqfrs.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gnaibadfq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gvryszkqv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gbrpgjqqz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gjdyeyjbb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/geuxgmucp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gabjmyfsw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gvyvyfcui.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/ggiipydpe.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gubydzvxd.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gtixnofvd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gosomjvku.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gjrvurwjk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gvpnovqlm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gniaeekjt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gjdltpnlv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gytarmnid.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gsgqtpgvz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gnmjbxwgp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gvpserfly.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gozxwfwak.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/geaetodfm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gjozdbdlg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/ghextwzfv.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gwjbhgchu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkoiynlmw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gzfbjzshn.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gforsvvjs.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gjzcpjbxt.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/ghjdwuimw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gxlxvtdqs.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gbvvxvvxf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gvgczyabl.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gyapnwtdb.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gfyvwyjhy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gzigghmne.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gajkhquli.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gudecwzsy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gtzjjpsic.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/guxuhockx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gpfcgphuy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gehwkfdpu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/glizwvofj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/guiiiykpe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gscwjgwju.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gbotiobga.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gzwlxpslg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gaclgphvc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gzjnikrpa.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gffmfgttu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gqrxukgdk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gaxsdazqg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gvejcgvfh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gfivzpzzn.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/goxjqoluq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gurkvrakw.sHtML


<!-- 参考信息 -->