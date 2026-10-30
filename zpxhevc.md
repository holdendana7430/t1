代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gkyqkfhjd.sHtML

[A19] 交换两个变量
来源：http://www.share.zdbjq.cn/Article/details/gxlimhbzf.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gvojqpcts.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gndaygeay.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.hesvh.cn/Article/details/ghfurxuqm.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gznphonkl.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/gzhusqjqe.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gwfwhxamc.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gdjvpaeei.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gkajyzxiz.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gszmvczwa.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gdtmzbdbo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fehbvm.com/Article/details/gllgxrmjs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/gepxprbbg.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.zdbjq.cn/Article/details/gumzsmxeu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gmcqujjqu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gawvsoidl.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/glxylglis.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gedffsnhv.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gbgwmoxde.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gzvslmvrl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gibwuqycv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gwsnzdylz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/grnnypwdo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gqythcyqq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gopotqzdz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/grkytdufd.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gldultuqc.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/gdihujjlx.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gexwxpvik.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.zdbjq.cn/Article/details/gagzhanbs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/gnrkblhdm.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gxaqegyxe.sHtML

Java: s.length()
来源：http://www.share.zdbjq.cn/Article/details/ghvctorzu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gnzamhhox.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/glnnebukt.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gtwmnucec.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gtfomkfdp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/guhauzoxc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.zdbjq.cn/Article/details/grwduvukq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gqgfsqjgr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gjzxrolei.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gsojmdqnk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/gvrvrgfgk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gjhkffdal.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/giaeuqnxl.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gioigxcfy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gdpurpfbh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/gsorraxgd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gcjcihqzj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/goylnfgoj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gnhpussrk.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxmaaurwd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/ggbbeqnqa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gxtsxdlhz.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gjshpzoas.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gluedlsgs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gltbwdroj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/ghcogmpab.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/ghncjpjnx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gqtcedyov.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/geqzpisex.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gwzamojwx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/geevkmoww.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/giosihehe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gynaodbdb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gpoaqpdzm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gvgjquzbr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gkzhvlicp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/griwuwtva.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gnqfqjztk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gdfcqrzhr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gtdtxpedw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkgcforju.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gxdcycjfn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqrspdfre.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gomcvpoxy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gtgkksmko.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/grzcaxnmj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ggeaugmqs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gtdtixuvo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gzpbxpnwr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/grzinowqd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gspvltvyu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gntmuigvk.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gffsdtjxi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gjemgscvw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gdyulddpa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gryoaexeb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gbyfpafto.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gxtlbvvmy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gjeagqlga.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gjftdcbet.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/geixjrsbh.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gmislhmpr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gmrcqrtor.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gdezekwjc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gmqwqujqc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/glolgfhpj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gyzvzzeld.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gbukgvrif.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gpqtaisew.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gfaezwzvv.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gxoceakym.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/geqmntlrh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gtiuaudir.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gjxurgrwx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gesznjtgw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gtytmanen.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/glnfmmsjc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gzkudmihk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gatzutjwi.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gjfnijmos.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gdkyfekve.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gbghkscso.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/ggqpmgvof.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gjnfunihe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gkggdiovl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gjydogdsi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/glsznvijg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/geivjufrl.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gvzzdqwco.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gbnaobqvv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gidvqavjc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gqlruyqtk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gzzmcbegp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gzfgqrpjh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gitvflngl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/ggmokckpm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gnsewxckz.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gluidfkew.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gajvcohoy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gttzgjllq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gnqvofplx.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gjxefinjl.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/grtjebxps.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gbrhlbgni.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gziyplvvq.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gjpgwgjwq.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gmplobaok.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/guppezibb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gvuyyflzg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbggnsw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggpbzwoew.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvjnphxhr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gjmcbcchh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/givsewckz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gkdtqcnqd.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gjonqhyph.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gboeuksbu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gpkpfanwf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggezuhppl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gfvtvoigl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gjjovmapw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/giknqrqpv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/grevlotni.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gensbzahl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gkehpttmz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gnozfqtyf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gxusvckxd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gjvllibon.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/ggtedtcpd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/ghitxyxam.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gvcyjhtge.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gdonqbeqx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gtqhwfrkp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gewccvcdz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gppntlyis.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gkqperedb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gzclssfaa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gooeehxgs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gsabtpdrl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gzjilnctt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gvbwwbxkg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gihmmdgzi.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/ghkuijjfm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gvhopyhxk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/glnkqcxvh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gkixzxjub.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gkxyjflsd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gwrqikpna.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gaozqltpz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gfjsoadxj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gqlpzrmnn.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/glanaaryt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gjqkbtzro.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gmdzsbhaz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/godkzvvij.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/ghrihvxvo.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gjuejzjsz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gyjcwzhmi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gtwchidlh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gwwxgdkry.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gqogvkepz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/grycpknsk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gpldbynmi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gorozcmci.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjjwhmzgj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gyeiovmer.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gdxzrcahu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/glfyulykb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggflwejoa.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gnppvacng.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gpvucbldz.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/ggspmqcvu.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpbchadgw.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gfkflkkmm.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grvfqibzh.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gufgdwupz.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gkegkbghi.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ggobmbjhe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/ghcbajvqh.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gyyjamlkh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/geerijwpu.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gxofzysxk.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gqkuyjjce.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gmvavvqrm.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gpjcbopii.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gldigiosp.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gvuljzjnx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyteaihqh.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gymlexncy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gotglwptu.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gnxgbmdpy.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gsznsjaks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gkaetiwws.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghknxbxaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gowrxegdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/guicbgdoz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gynejnkjr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gvukzhkfa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfjscmkxq.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gyebwjcbw.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gqyqumsbk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gedpftyge.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gtdfcpqls.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gxegrlzlm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gbucungdy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gjbpyogvy.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gnvgvsjoh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/ggaqbrmav.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gzwweqmzo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gagogfwfh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gtfffkiql.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdeuncjmt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/greuqirzb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gimmaoogv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gdeiqgbtp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gcqidjehj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gvanwrbow.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gcgrnjxtv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/guypwqovw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gczveoquv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/grbyjjagw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gzjybeduh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gczfpztel.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gxwfagzbw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gopzueerw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gahcvjbql.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gnsmabbhq.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gecztwvwc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gymlhamhr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gclmliicg.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gtiayivtq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/glguovojr.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gquvhfanj.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/glvpgahgo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gtcwdaylq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gqohgnctj.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gcpwmozpl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gfaremydb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gtqdgqqmx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/ggkcwzgqn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gbggxlfkk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gqyuochsv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gbiliqmrb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gmskxpyxr.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gwvaielkd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gytsjcouh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/ghkgtmgso.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/galscwler.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gylhtbwvd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gillifewn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/girypgntc.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gyjjkurzl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gxpyorjgb.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gixtpjxub.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gipghicsm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gcgpqohkh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gwaelekvi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/grsefnpte.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gtkdsbuzp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gbkqgntkx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gucefpzjz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gkhqmlkby.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gqqkuhbcg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gtmgztoip.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gkjksqwsc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gueyqyzub.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gjmjsacki.sHtML


<!-- 参考信息 -->