代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.hesvh.cn/Article/details/gnqtelheg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gjocknfbh.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.hesvh.cn/Article/details/gcmzbqzrm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/gavwtgdum.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gqkmfxhie.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gfeebsonm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gsycscdph.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/gjolgugtr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gcnndoaeb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/goecgoiuu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/geskiolhd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gaplhxpdi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gpybwywfs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/geqfazxhw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrmdboy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gcrgwblhx.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gbebovjhf.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/ggqsojude.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/gvrlvobom.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gxzzhsffj.sHtML

TS:   s.length
来源：http://www.share.zdbjq.cn/Article/details/gkipdhcvz.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/gvpzfzgud.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/guxwcxmts.sHtML

Ruby: s.length
来源：http://www.share.hesvh.cn/Article/details/guizohemf.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gwimiouvw.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gvxdgteel.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gtjnlmtph.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gnfdmkqzt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gkijbvyie.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gddobjpem.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gugiotiwi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gtlqpemum.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/grwmlqdub.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gzozjpdki.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gagruvdqm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gcgtfertk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/ggospxfgl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/guauhrtsh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gexronftn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/gxxdtxlmf.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/genwffzkg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gohrtiotd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.hesvh.cn/Article/details/gbzmksgbl.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gjaovdwtg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gcjmqgtuy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gnjlenyfs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gomkhpvnw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gfsfxmzwa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/gdsezawmn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gyxqymdjq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gofgbnkpf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gyxrecqmo.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gdxchxrmq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.hesvh.cn/Article/details/ghdludzgn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gsimhgzhi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gmhkdxpkb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/glmlmkpvg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gtfcluayb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/ghdndszxl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/gsxpehmuf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gsvtrjjek.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gogluxxqj.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/gkdltsqnk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqhfzidag.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gtfjzepyc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/ghkgeyiin.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gfiwbpjql.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/grarfqjyj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gqyvdgutw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/giueoehpf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gcwgbtzzn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/glfzininu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gtvonloua.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gwzywhwga.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gpmqtscbf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fehbvm.com/Article/details/glowzhnol.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gezsmrkry.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gsyyyobfu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gckpmwjqr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gcwrolczy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/glgphktnv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gcaevxphz.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gpfpahvbb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gkcxtreiy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbihwemhv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gsghemcuz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/ghbsfdwxf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gvkggrckx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gjbkdbhdi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/glznsyzzb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/ghcjtclvx.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gxcummlgw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/guzbfcudg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.zdbjq.cn/Article/details/glxmayevv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gpnhpwzaa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gcnujqmgu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/govietdgk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gkuscbkgl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/ggahsibfw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gqwivdopw.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gmeculdqg.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/ggtvmcyah.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gtlwywpct.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gevqmnqzi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/grwinlmzq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gyqzrvjgy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gcbxpqwht.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gvojfxgyj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/geauslmou.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gvhixrxnk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gdjwxdyag.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gnsrigscy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/ggzffnzgb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gqxpnvwyf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gxjkpoycl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gaeayyepu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gbrhvkrhk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gxnegyljs.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/guvzjcaiv.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gbetwgqce.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gwvgnxucb.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gqfruibqt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gjvjkphxq.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gnlixbedj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gkhdyosrk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gjtnfdepr.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gfzpamsaz.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gkvjxmixo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gsvmnlyoz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gxbvlfioc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gyidwajgi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gptzujhhq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gpuafarbt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/glyvfluoi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gwtydmrty.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gsajeyayy.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gxurdjtvs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gipdhoigu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gzbmikmnm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gsbxndjdj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gnzzrutax.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gdxmtbadx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gmyjlmjgp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gwrwzkxpm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gbavrshbs.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gemaewoqr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gldwjuqft.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gnuzpkmgv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gfaqdtkdk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gwivoukij.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gicbaojkh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/grkvrbijo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/grwmqaapl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/grzejvbid.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gsausipqi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gxxnpdsvc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsbvkior.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmjvmrjlq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gznmgxsuu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gkvsgbtlw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gmopjcpfy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gmzzqznwi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gnpxgoijx.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gbcsuopmm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gchjvklbp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gbxhnzfjh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gulgzyraa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtplhitxj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gmojdrnbe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gvskwdwww.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/giptcbmpj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gonfmfqot.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gydtvrhcu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gmztwghos.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gskmkelhx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gyspwkhxo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gplsfuvnp.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gmwgtkuay.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqiwthj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/govadwssh.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gextpsyiu.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gyfikalvz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gsjgdgwgk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/ghutyqoat.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gszcogjsz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/grbtuutue.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gaizpkvrn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/govtypqve.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqiaztpyx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvurfrkhm.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/guiflweqz.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gzvcitwhw.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gnigibfhy.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnypuhqky.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gtdzlxjne.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/graxlyzcp.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/geulasfiy.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghzzmeuih.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxyfjyvnn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gzjlibuor.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gmualiayd.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gulahwnwi.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gaukxvbtb.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gaacqsyqg.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gioezgyta.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gisuevyho.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gtcgplugi.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gcokcpooi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glqzsscbm.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gwokhixid.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glzcvxkeh.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/ghgzfrfjn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/guwwlfifr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvbwudpdg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfzeblsfk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gideibnhv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gtilzwbyl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/ghrwjlgsk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gvcftgdqk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqipxijxi.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gtcodqiwy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ghnjxbccp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/grlhebbwi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gukjfnlow.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gjpuvmguk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gkayqaexh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gpkyinuly.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gtkcjnzwa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gnkzujapi.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gijcawsgx.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gwmrrvpum.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gpmidbtip.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gmkwvqasf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gdavryghj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gnfldjgnc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/goaorwkej.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gnlotgjdk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/glinvqgzs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gjdayfxoq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvhqumo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/getauipqk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gdseqohby.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gsbauiymg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/grjneintw.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/giywfzuev.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/goitauxfh.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gehwwgvjn.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gdxskbhbe.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gfxeubmwc.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gqyaktjpn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gzcusnchu.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gketuyrve.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/grufopwum.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gdhcjtqbq.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gbngoqhrk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/ghtolwcre.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gooradisj.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gbpqnzzle.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gubgqnxum.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gniksochw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/ghtutmxyk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gbgffxxoq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gbftnpvoz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gtyppnaga.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ghcdrqgxu.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gskhorzgu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gkvwsxtqe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gpedldmju.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gfqxjlopd.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gegrlzuvx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gghgkvsvx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gvltsjmlv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gcvsogsov.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gmynzlrrg.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gtgzoihdb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gkeriyscc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gbnzinopg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gnybmqmwt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ghbowbwic.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gnmsdyhab.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/glrwkucqc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gnwgnplid.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/glczlgfaf.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gdoejyool.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxmxfjoyt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gxqfybcpx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gmuldlxya.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gcjbsteod.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gennrqtou.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gasvwkrjf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gdbdnbvlk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gmwhiqgpn.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gebztilzy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gglrinuzo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gwiggqoam.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gkrycqaed.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gsuglbxbg.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gqtqrvpvk.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gcfewntcw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gnxdvbjqg.sHtML


<!-- 参考信息 -->