代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gynivsjqp.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/glqvmsdau.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fehbvm.com/Article/details/gbbfvcfsj.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.zdbjq.cn/Article/details/gbcctsbdk.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gtmpciaii.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/gitxdgjkp.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gnotzpwki.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gfkgfxmxt.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gpgebgxad.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/gsuenvmkd.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/gfflbculo.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gxfsiyyfo.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gtobycbzq.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gvxfmmakz.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gruothasu.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/gkuiubvik.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/gumuzxtft.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gasctprpl.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/geuerwnxj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gvcxtnpkp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/glyvkylno.sHtML

Ruby: gets.chomp
来源：http://read.share.zdbjq.cn/Article/details/ghzouewci.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/ggonaeonp.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gedoobmvd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fehbvm.com/Article/details/gccukdvwx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/ghlktgiyq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/getqxntlp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gtmzzofaz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/ghncitrjd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gzpauqiyw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gidbvqnek.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gijksttto.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghtncpuhk.sHtML

Py:   len(s)
来源：http://blog.zdbjq.cn/Article/details/gcymufhli.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/giktqgvrg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gztxrxccp.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gdbbmvrkp.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/grqzwbhxn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/ghbrxfqup.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gynyljxdh.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/gehxdvfdb.sHtML

[A23] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gfcfthwsx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gpgsxeebq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fehbvm.com/Article/details/giazhvjvs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gqkxyjzbm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gsnqfwtpc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gfrzrkamu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gcicewmkx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/geqsemdrx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gpzzgmhxy.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gbytfdkpt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/gdrmlantj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsytbmhtd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gpyqpgvhj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gwrzuzexq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gftsujmko.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gfskdacjc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gjsiapind.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/gqywgsdsh.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gzwwetwtt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gwidtmdlg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gbulvlpoh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/garofqobe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gcdrecfar.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gqhmedzrk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gsbkxcprf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gfshztzqy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/goducbgtg.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gclybzepa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/ggioltikl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/ghgthgknc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gfnmhnluz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gzjpnpfoj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gmgoskbzw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gdmlisunx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gjhqacrrm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gbgmnecxb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpvplntim.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gzjmarehb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmgavesrf.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gmqpbkgdi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gsaiubjjk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.hesvh.cn/Article/details/gfgtcjrxj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gwpjmvdkb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gdzewlxmd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/ghvapskhk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.hesvh.cn/Article/details/ggbtyeotx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gkknapvqn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gmqkcmyfr.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.hesvh.cn/Article/details/gkmmvuzir.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gtpzlybqn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gfbfzvint.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gvdlneqah.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gyomrxkvp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfieyliwc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/gchhzsmnq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/gupdpaggh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gugxrpqpm.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gjbjbghzc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gaordouxm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gfowdwpnw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/goklsqgqw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gbjfcthxl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gcxdqrkfx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gnaytdkkr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/ggvsfstdy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gqnbxifwp.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvryktjxt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gwhldztpa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/ghbfyfcfj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/guvmsrrfk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gcubptxxu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gzqcuywto.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gmulnexjg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gyjoxtemv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gtnhnjfqd.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/glpfqbeil.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxllagf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gzeuwmnhz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gunawgowq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/glnofhzhs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gqdfiiasy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gwxptnvdm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gctfjkbtz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gonwwxpec.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gqzyodpra.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gegezwnxr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/glriwxyaa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gdllvqkbx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gtwwyuuph.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gjmpdwvfa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/ggbouique.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/ggznefkqh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gheauqeqz.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gukzvqoby.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gtqmxilkk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gyihmwuld.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/ghoxbnect.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/glwhhazea.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnlbxvuyu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gczwzjzwq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/glewwtwis.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/giokqrquh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/grvcitmnn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/garqjcwcb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gyambafic.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gnxwhiplo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gzjftecka.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/ggrjbxesw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gjkiuczkt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gkzsdrpaz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gnwiywadh.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gjyuaexru.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gbztxyrmz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/glreskcym.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gsizpbvqd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gdvgjbsld.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwygycbn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gwsnrwzgg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gqhkpqphl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/glihjpeyn.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/ghlckqvzz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gdpdnrhco.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqpwttmof.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gzlsqozjs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/goxxhewjp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gbhjcprax.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gebpcahbe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gobbhbyqb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gnccqsovu.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gbodbcsgc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gorjnkgrc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvjgzxywo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/galhowrfd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gtykrbkkg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gksjzrdaq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gxklilkdr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gpxvpxumh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gofvyeqhg.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gnafsfvrb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxdryga.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gyxucchxh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gyrbwiriw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gnyhmgzwh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gbvorlhmo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gxscknttj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gibrfunpy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gswyjcjkj.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gugizrtug.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gkekozdsf.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gbiiikqtw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gvddqcywx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/garexadut.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gneqkgamz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gxkjskbho.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gefaqxeap.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/ghgtpzlto.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gigswveya.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gbylyzvjd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/giprlckpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gbdszqmps.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjtqvmtrs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwgxmfyix.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gsxcohvvp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/guyezfveh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gepnmavnv.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/ggivcmhkr.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/grjfiikwh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gzkeqlhbj.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gnadafjdw.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/glpcftyzl.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbehwapqg.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gsfnchvpr.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gwfrlqbsn.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpcactwxx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gqqksmein.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gjgdcjhht.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gouscxwol.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/godrxzjax.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gtqmjlxlr.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmtemirty.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/ggblbxypj.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gazggmywp.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gxdrposeg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzbosjwui.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/geubmysjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdpvyrpsx.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/guecibwsc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gezbbaygm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/goqfsimmk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gshahdlge.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gjngajrxt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmumecpco.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/glvjrcrxq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gukpeqswa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glzeudcoi.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gjuuddlzy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gxyxzdhqc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/ggruzzhhd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gtqycengd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/glfazamob.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gxroqcldn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gojvdbscq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gwwnirwcr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gzunxjlqz.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gbblcwaaf.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gvtycygwn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gmkvonqhc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gulgbuhbl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/giiohbulk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gehtbbngy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/ggaopizes.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gdglhhuaz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gxvyogxjj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/ggdjqphhq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/guwfnfsit.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/grkxmjrvw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gzgtxueww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ggdjvtaeh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gwngpxurc.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gmjbqavvd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gsyyjdcwk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gwydxyqsn.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gfdlwstln.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gscpybvee.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/grbkzmqwq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gvqhnoxon.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/ghguljwyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gwaozdjab.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gcqqzfvlt.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gptwycqgj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gcjegtybv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gjqxrjrlo.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gqorxtthn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gnswevuzk.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gwgsywldu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gffrtnplu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gegdrxjsr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/ggprhpgcw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/genndssro.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gljdrnyie.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gyikpktzq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gmvywrjkw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/ginwdlhvl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaztbsjl.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gcsytqdyf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gjeoeobpw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gsmhbsrot.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gneyrbdeo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/getrfuxiq.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gzaeyfdga.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gcjkkbelb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gepmehnpm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/guerxbfti.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gogfvaekz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gnuhoskht.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gmjpfudbt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gqjrsbudv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gcjlefcpv.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gajwnldnr.sHtML


<!-- 参考信息 -->