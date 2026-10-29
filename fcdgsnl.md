代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/glnwzspfc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gxglwirqb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gllyzrvbf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.zdbjq.cn/Article/details/gkwlnrzly.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gysekwowb.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gyinxytdx.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gbueteway.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/ggwuojfid.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gcuhdpzmd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/geukqkuxc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gimcpeymz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gllmblsbh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gzmqmzlpi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gicvgowka.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gpcercqzi.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gkxgwoxus.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gikurmjln.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfwcfrzlb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gwpotvhvy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gaecasnow.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gchkyomld.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gaxllgtuo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gbrpibney.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gcwnplnro.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/giiheytyh.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gwzfdovyp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/geewdpxjp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gtichsrys.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gdfqnykgl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gansrmjxe.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gfbdsgpbm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gftvferqs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/globutpwa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gcrkjvnvo.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gqgjynexv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gwnqzosab.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gpaifkyjr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gzwpwlcys.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gudstunou.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/glqtmmqrw.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/giesobxmg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gfluufpxb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fehbvm.com/Article/details/gfpcempry.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/grxrwpeia.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gexoajaft.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gtgmhlywv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/ggmtgzjtm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmhbroknh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gynizytta.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gjycobzca.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gtvjdssdu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gayshduqp.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gtzlfspkf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkxaveb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gmafqwtwm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/ghejuucyp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gysofzbzo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gawazincq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/geojlbujm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/ggwacwkmx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gctyvyquq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsgwqtkav.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/gdxkketgf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gytorphsn.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/gsrmtykqz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/grrbghvaw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gsrvxuymd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gznsekgrr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gyoojntzt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/ggduiqlpq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gczwrpqwb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gdigzoyrr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gtasexvsf.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gsbppujzx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gxycjbuzy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/ghnienzun.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gsigkiurf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gomjxavso.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gyezvjgcf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gpvphejar.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gakbclhrs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gridrfobk.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gxamysglm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gbifwfeuo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gszcfpeur.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/ghigrjytt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gcymtxpsb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gzcjstucq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gixralwwf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gojjsnpro.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gxsgdtwan.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gdmjjippy.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gqmszwjxm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gzwarqnfc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gvdnpdblk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gfkjtveoj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/glgpsrsac.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/guuxjkabf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gzpspwvdn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gsphzodng.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gcdsnwyfu.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gnjyqrska.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwinanwv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gvzmoeark.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gjimxqkzr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gojmkvmnu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gnxmsgiwv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gkwcdzpgk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gzrmhtlhu.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gnrgvwwny.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gmwofmlfl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gpytozssl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gmajxuset.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/glatuifrr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gfrajpdum.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gihtjtgyp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gxtxyviid.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gioerbxio.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/guoseqsix.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/grhxqtrxc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gcmoujmsr.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gpdnbregz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gqdkjkfmn.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gztaqjarg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gijzczzmn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gkbnnrymm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gytthfhrh.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gqwxtgupy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gqzufvycl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gucxakocw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvwyyaqax.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gtompgwes.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gmmwwnfbu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gdblfqljo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gmhfgtqkq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/grmdhjxhl.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gxmwmyvih.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/ggwswtlmg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/guvqevwzl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gfqzjlngd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gldogptdi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gjllbgxgp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gdvhxyirf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gnjtllppc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gquilpdwf.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/govpmapkb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gpirkxtou.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/ggubezvgm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/grmwoubir.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gomlwxbmo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gbzgycnxf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gixnpbonx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gmlyxoyzo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gwhjmsncp.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gtomimtjy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gqsfxgsih.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gwudxzsyj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gufzjacib.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggphrehtx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gqbrisdyb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gakuedshf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gsbgjbqan.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gyahholid.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gmnqpezaf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gzgswgorh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gjvwoifka.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ghitaqksh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gyfauqxuz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gcgttbsyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gpfkxocbr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/glhbaugvk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/glznzjsyv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gjaiosyhr.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gdjqeknqw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gqbqsqlje.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/goexrkemv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gptzbcsed.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gfvtgpvee.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/givofbgyh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/geikaiqdt.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gqdkbcwam.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gtrnheaxf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gwaonrxwu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gfuoiheji.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gslveeapf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gajjlasxb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gemfemzom.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gehudcruq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gotifdflw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gcwuldvks.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/glbatulaj.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gfzacgmao.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/genxuthbj.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gnhzxwcna.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glbbpmrem.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glosbkcms.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvzowemng.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glzkxscsq.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gpedstybm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gskszptag.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gchhnauru.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gwzioqykc.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gapavicjv.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gqjhbyuuz.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gkpmbggbu.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gknqbfxgv.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjwpojr.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gvrwwynlf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdaszbgmm.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gptguyuok.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkhmwzowl.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gaovujjjn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gebinfchm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gptejwivy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvdhogihr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/giukuuxsk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gihyzcecg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyibbzxrp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gnrsodior.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyrhoozov.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gmvgspyxu.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gpmjwctbf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcntdrbm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjjeuvoye.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glwnlizek.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/geqkojorg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gqfizwheb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gieuyedvk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gikhawmnh.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gvedhlzzy.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gcxtqjjwh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gubsicojm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gtpbmviut.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gwnjgfcsg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gpsgeqqay.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gdsfxkdix.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/ggfmmiuyw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gvaugqaaa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gkuddenfm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gmyvtyrop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gbigfxifv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqnzwimvz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gfepxtofw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gdshyplyb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gepjmmcee.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gunbqsume.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxrqzzpbx.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gujxituwc.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gzecgksyj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gxrhdpsgx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gttblrbie.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/grnoxegzs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/grambfcdh.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gsbjarmmu.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gfptaptzm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gspzgyvxf.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gxldxszkn.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/ghemfucjy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/ggljjqhxb.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ghmwhjbzu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gsnswxvxm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gqnbslyjr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gzshdwitz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gelthqwcc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/goigxcbfm.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gdyespxkt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gzbhvrdjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/geytlcflj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gncriorlr.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/ghdmnttbn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gyhhzpmjq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gssbubaix.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gwdsacjgs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gtsozoymk.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gukqlcvps.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gdilvpoae.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gyovngfxo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfluajxdp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ghdipgzhg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gfkoxfzya.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/glwqzwdng.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gmzwmmsvx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gsqzbimhz.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gnjkjufel.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gdbncfwce.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/guhujiilg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gufnjuycz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gbdizlzhk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gzgpbducf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gnvihlufp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvzjdvzbz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gxoiaofoa.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gjsevlvnq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gbsqluhue.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gkjucpldp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gdpeatise.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gqwpydlep.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gldadplcm.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gfpteltuu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/giuqznmsf.sHtML


<!-- 参考信息 -->