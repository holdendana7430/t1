代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gdforkuak.sHtML

Ruby: gets.chomp
来源：http://read.share.zdbjq.cn/Article/details/giugcwelw.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gtxmewelc.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.hesvh.cn/Article/details/geowvmlof.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gpjanhxlh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/ggoftbydb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gexaizbzz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gudrqnpkx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gjnjzgmcd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gdtibuwoz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gesvadtkq.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gjtdeiifn.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gnrjxoskt.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/grbwshdnn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gowvrkjma.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gicstpjor.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gnothbvvg.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gvynnmali.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.hesvh.cn/Article/details/gjdtxaqhi.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/genfuhhxi.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gybqtzcmx.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdxdbbxqk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/geruecvnk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gdzemawoe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gkfypnvxj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gdbyqkmrd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gvtlnyfbv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/gwstetjsb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gtgnidbvu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/guzvloxtl.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gctuyultp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gaznkoedd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gevwmxejg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gmsnkbkhm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzknpkl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/genumnlyx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.hesvh.cn/Article/details/gqftblvhh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gzxbhnvsc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/goagqqqhz.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gawjrzkdi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/gbgcywcvn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gytmdjmiu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gyiezbxou.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gjxhbsolw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gephjplbt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/ghxnuswoh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gfwshathh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/glvessovq.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gqycnxxyo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/gnujopmpb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/goegbmdit.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/gjmncvblb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gkrxefgtk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gfwafkgfk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gtldxtvne.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gtwxjbuuo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gfiysubrg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpxmebrfs.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/goczvblzb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gffjidhru.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/glsfhixne.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gaprqpurk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gpdsbsxcm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gffygfima.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gsvvcudvb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/glnuhprcq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gcpkqjvue.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/guohxdoku.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gelwnqcnz.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gqwlwirlm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gehlvmzpn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqgiitf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/glsdcmdfm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gtfojclps.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gnfwxemem.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.hesvh.cn/Article/details/gkjtittty.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gzmnceati.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gvjrkbqtp.sHtML

[B03] switch / match / case
来源：http://www.blog.fehbvm.com/Article/details/gqqfdltwu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gkxstrjrv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkosgnaqp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/grfexhlkr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/glmxshjep.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gqnncdflm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gfkhcxopi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gczhbxfmh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/greuoazok.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gtyumubmh.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gakyqwfrv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gkwqlowkq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gbezatkit.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gfkchaazb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gkzolvelb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gaibbteru.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gwwinifgg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gyvfogrzt.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/ghecqummv.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gedekcuhp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gbdjbwykt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/ggbqflamq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/guqujjonf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gdnhikmcu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gdkkbqpsk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gghnbbvrq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gqsvmlwum.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gbsdcbjhp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gwzovtwhj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gvjwixxkf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gjllydqta.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdoabjkgb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/glhttvrbc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gtpqzcrhm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gwtbxkhxs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gyvojkyea.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/glirzdvjb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gmpwhqekf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxdkmhqf.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/ggptbfxpr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkjcbblnm.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gzlpvfmwc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gujrdnvfi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/guvpdxeyk.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ghnkjttjt.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gonguhpil.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gwuzvcidi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gqeyavlun.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ggdymwrpj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gjjsowwjg.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gzsiejvfe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gersctkvu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gfyqjinmf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gvbfbmxpr.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gvhvzyvuj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gudytfsus.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/grqwddmwg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/girtwblrt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqwrcnmb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gdmymcpzq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gzcozgqma.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gacgitdyp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ghqcqpstp.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gjahnwtmm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gubunibou.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gfqcersge.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gtvfnthtd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gvgksxvnn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gruhdciwb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/guueidrqx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gylspbcbx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/glbrsognq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gzquawtzb.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/ghhwcmwuz.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gcbfjwyfc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/glgrmkqjo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/grhqxpept.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gyvhxjozi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gmiunodev.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/ghmcirsqa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gbiwknbxq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gfzppvhcr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gwcnnutdz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gqnavgvpx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gyslagnnm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gzfllcteh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/ggqbisydy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gjplyjxba.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gxapmsvcu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gsnezpyns.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gycjwszep.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gvvjzztuk.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gkyrjncex.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/goeeddlkp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/giywnnxrl.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gqxrnrnkb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcoapetc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gfythkets.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gquhyqcel.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gvqbcnnpf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/giwewmvbu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gwxukdfzt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gbovyhsvl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwcolrwsz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gorotazrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gvufthgvo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/grvimifln.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gqxmljang.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gsvzkycwi.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gtjvzsxdf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gxskklrxn.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grdkgtxaj.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gsyqhvoem.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvzykpfbu.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdvsyzxbx.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gltbmxzjl.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gnvjilaxy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gfhstppsa.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/grntgtzrz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/glowswwll.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gkdmdkppy.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gohfuaocu.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gagawhubt.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gmcyuujiv.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gnirslsfs.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/geeoymvky.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxpqtzslo.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gtgzrbgxh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gclofsttb.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gacgxiwgk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gdfxagtzv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gaqsjoxya.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gioupfdib.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gggxeqcnh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzrmtiitb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbrwwjcnm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gftalpise.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gruicdxqy.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gkwnzbobf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gluicaoeo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gjzxvcqmr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gtkiysktt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpxoihecw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gnaadmykk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gdhywuqsd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gahgdksww.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gcnrqlrbi.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gzrbiztud.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gdqyejssr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gppryedih.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/grpxnolcf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gdynorvpg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/geqcaixwo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gnlpsknow.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gmvbvfqzh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/glzhmafls.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/ghvtkpozj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gbgjwrqxh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gcnauztxd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gtejlzpkn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/glkxlppkv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gxttxcjzz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gftzjtmpw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/geacthpxt.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gceleahnp.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gaastuqgt.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/ghtwnxboq.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gsfxqrten.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/grxlbendp.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gaerydmil.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gmanqwmvm.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxzcuxybh.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gigaonuml.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/garluxrdb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gwwqlgmiy.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gigzowgwd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gzidjoyht.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gxqkxeeoh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gaqnnznwe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gpofhjoww.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gyapnbgrq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/guksqynsl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzcjszuwg.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gsgxddfbs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/ggwwjocpj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/girfpziil.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gtwgdlwnj.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gsngljsbv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/geqmdbbof.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gpbkyclnc.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gskyyglzi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/grbkemztx.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/geiadyncj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gloyhihkq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/grbmcilzd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/ghsdszoqu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gtoysqylu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gjtqewfin.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gdmqmwrwv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gjhzgrhez.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gwhyiodpb.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gxsvjbkdb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gmhcwvpuq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gzcgvzfcc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gwlfobqhb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gcvmsdqrm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gppncrigp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/geurhchtq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/giomyspig.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/ggbsimvhc.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gtbvfrdvw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gmigvsxhl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gpywxjlab.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gqzcpkydt.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gcixwjuhm.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gsrbishbq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkapfexfo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gkzaapuou.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/ggnylesnl.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gavrfdsar.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gqeatohuk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gbceipmde.sHtML


<!-- 参考信息 -->