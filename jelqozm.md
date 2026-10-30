代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gkatvwlme.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gonneaidb.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/ghtqpkzcq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/guraynoid.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gudvqwxqg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fehbvm.com/Article/details/gzqamrldz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fehbvm.com/Article/details/gsjodarao.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/gctkfxabm.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/gvnbodqnz.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/gpiafidbc.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/goslnsxyo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/gqeiyouki.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gygjgqgiy.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gprejulut.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/geelgjdqv.sHtML

Go:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gzelygfai.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gnquphqhd.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gbmsqnwme.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gneyyyvvw.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gowaqvogk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fehbvm.com/Article/details/gxbeyevfo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.hesvh.cn/Article/details/ggvakaniq.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/gdxshhirr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gdjxwurgu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.hesvh.cn/Article/details/gthgnwpka.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gpngzmshh.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gfaprfdcm.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/guzayqbgf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/gramnljsk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/ghemqhsgt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gdmoozjzv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gzuqkrgyf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/grsdxltan.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/grxryycpf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gkdjawmye.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.hesvh.cn/Article/details/gwarhyccq.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/gteazcbpf.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gujdswqpj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/ghjzwtsdf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gphrjtokg.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gfebyflef.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/giftkpmdr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gabwybdjh.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/gsxhjkyub.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqlqpkbbw.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gklaovmjh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.zdbjq.cn/Article/details/gphdceuvn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/gaboxymwq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gmfvxyyyz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gkqbpwbey.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gibdzppkw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gkmtnxvoh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gtkemgpgv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gopexnrpm.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gladihwlx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/gcyxgtpzh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gerajxfrl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gkoweufkx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gsafqiqdw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gxojtvqab.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/gcmtqssqh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gsithbkdw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fehbvm.com/Article/details/ggaythjxa.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ggcxhdxlx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gqnsgoqcq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/geyyzpnfo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gnpcwqrib.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/govbcxaxo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/gdlwjnsch.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gtzjiferc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gvdwaacvg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gtaebuxgx.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/ghrbatefr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gfqrcdfke.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gsbvfzzeb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gwnheudse.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gdvyrzzvb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gceliabin.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gtgggeiok.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gqlvhccah.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gbbcexcus.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkvlazgjj.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gjgxtdbix.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gshprvaec.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gejjpkzlb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/grjtjoqks.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gxrlojeiy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gqybolxbv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/ghhitwzkq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/ggjbumwuw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fehbvm.com/Article/details/gojkxuvkt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gcetwqahe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gwvnfyegl.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gjnjhsbdf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gbkgmvugu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghmhzdjlj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gmwsairsg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gaerffpwb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/ggtbybctu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gmhmidwsj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gkqismniw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/goajhtthb.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gtxvrsfbk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gpjsckgei.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gexignnro.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gixepodth.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gykgwywkp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gjwwjokmf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gpmfayxdt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gmstiydpm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gavzurcza.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gmqayzswq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/grylugjyq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/guzssoxnh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/ghmbuxgwj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/geubzyonu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gmufenqzv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzoddtgp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gobrpobhr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gysapyfuc.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gctjlfipt.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gqkptmiao.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gcexkkcmx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gfslsbmxd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gzhaoujbb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gshgbiywy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gvacfxbkv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gxcpjlxra.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gulnxrxfi.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gpjufrgjc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gaahkvyny.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gujcaytgu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gpnykznyg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gbjvfozgh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gmiulfnls.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gimpihysa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gdsfwznqr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gkdwkwnla.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/gptoihjhm.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/geakkiofx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gcuqytttd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gsqwiocbk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzpkwzlz.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gchemaezc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gzsfqvsuu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gjzhqretw.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gemubylmn.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gtpinavhs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/ggvytwlie.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gjqfnvxcz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzgfvbhqt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzpligjcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtdgumruw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gwlafnmxk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gopkmaahq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gquifnvga.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/ghxyshsml.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gbupqsyud.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ghgzmlblj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gvhhkfscp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gfgooodmt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gmijpxavu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gcqatsvcb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gdxrkchhy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/galurcvxi.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gitblgnie.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gveionzwh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxwtfwbx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gftyodnvd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gepemijxe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gepnvmyyc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gjbntxomr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdfhdyl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gfdrzudrw.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gilimejoi.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gmfqhckcw.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gshzufrhf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gxohysskm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gtztunwgk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gorkpvskz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/glhzmxdmg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gujvoqutq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/grjzxtpgf.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gzrsygofb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gibceboyk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gziinokwu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdfqeqdms.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gynlicvbw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gbrftywzj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/givqvnhrn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/giicpxcon.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/guptywlha.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gjbabxjfg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gyytwraus.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gzsnphdfi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gnlfahuvh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gsphxvmun.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/giwemrgfy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gtedkaznu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/godtvvwkn.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gqjsopmku.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gfnmuvuwx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gcbgsrvkk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gyafvkwvx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtlmoviwn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghbbprpcj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/goywltsja.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/guedwucrb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gdlkwwwwj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gddnhznvw.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gvkucyqfo.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gpzjyheay.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gwpvvfryu.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gweqbrmec.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggmfspstv.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvrcietgx.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gbiloqeoi.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gaeotddnk.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdyunhjvr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gobwtglry.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/guyowxuro.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gtqkpoqqr.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gcowgqyws.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gcrvxbuao.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gkffrhbgq.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gdgrczssa.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/guspsxlnt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwekjzcfe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggitergoa.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcvbisfps.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxwdidbgw.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gfmkqmpom.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gbbcwcnrp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/godqckwji.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggeswwnzc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqydqnbum.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/glrspyksg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gclagpmte.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gltixtwqh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gujbazdog.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gdrdebtbm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gvaxvkowx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gbpwrdrye.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gaabcboep.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnqseaple.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gigogwhte.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gfsfeeflh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gdborxvkv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gbtcvmwgb.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gzaomqpwv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gspbtqyrs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gmzprckwf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gzdmhcoub.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtropwljg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/ganzjnbnp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gvrltmroh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gtqvkjhnp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/grtsyistn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gugsciulf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gmrlnhgdt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/glefqgrag.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gzmwseopf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gougzasjt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gzvqtfwpe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/ggzpgxiap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/grghfksei.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/goxtlczbn.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gqkgsyufs.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvvgqcjui.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gvubdgoni.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ggmnhwjen.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/geqtzixas.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gcrscwrfn.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gorbupsbv.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gfoopuagh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gzsieorqq.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gfbvhqqva.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gxknkwhcj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/ghrhtaozi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gaxjnmnyy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gazzknjto.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gcensqbpx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/giazbrzgu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gxsdbalmq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/girmfzkgz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gmbclqupr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/ghziqdmaz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/grvsbfdwf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/grreyvxlm.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/glctichos.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gayezeduz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gpfrplulz.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gcskoptvp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gygyjadzw.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/guvfhuhew.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gosrmhdsm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/glqjfjvvy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gyzkkrclx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gzecptxfg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gxiprvxkq.sHtML


<!-- 参考信息 -->