代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gbzvbalgx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.zdbjq.cn/Article/details/gtpwqhrjn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gipqipyou.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/grpxfpfag.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gcxueyjlq.sHtML

Ruby: gets.chomp
来源：http://baike.hesvh.cn/Article/details/ggbalueye.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gkvqynmja.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gycbqrmuj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gapikovzi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/goadjowwk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/glzgpztng.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gskotnvwk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/garmozowh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gtwmcnhrf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gghkzkppe.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/grniozqqt.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gtqbhsota.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gewbgmswq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.zdbjq.cn/Article/details/gkdlmskoc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gydpoisrq.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gjvmktgbw.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gedjncgqv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gimvvpqbm.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gunlybhxc.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxmbbsx.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghqemruem.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gebgpibil.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gywqnpkpf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gjplyqoop.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gxdmkkzzr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gqzmuvkjw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gpncjylot.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gbdezigcq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gbvpmvxgy.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gxbwsuwki.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/glualctrv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gtxvogkda.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gmathrnuw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gdlmfqvjl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gbcnsaiqe.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/ghpvtwves.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gqhtilsmm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/girupvbte.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gtnobppht.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhgcmok.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gppmzwopw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxsnjjcc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gioqmeduf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gixyxidjy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/galpyztak.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gazilrddm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gfoguzmyr.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/giuqnnynq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gufdgzeuz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gjagvdauy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gusryrdkj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/gsepmyktz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/glrfofkfz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gzaesnpud.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gkxtzeqrq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gaowhimoz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbvpztsev.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gywmllfdk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfencetom.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gyzozavno.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gywxbkmsw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/grkwnccvt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gicqmzocn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gxkummufo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gnzvbgtba.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gfkaluqbw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/grnzhtygs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/grlgkbcgv.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fehbvm.com/Article/details/gwdebzyyk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gqmbweprv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gfakxdimn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gvyllfsrr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gzabmmhbg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gbqwiqezu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/gztsrryvx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gqcxflrrg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gtdxooubj.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/guhcekrlq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gkstpeyas.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gkyagxbxd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gkykbagdr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/glndpdbmy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/glnilxgxp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/grkedegpj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gzceofipr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gbnkrkmyy.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gqbggawlp.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gcxwjrgjs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gvgcouoql.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gmbuvsmus.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gqmgocqce.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/glvwdkygn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/ggrztpipk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gnsvpvqct.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gjzwfzhca.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gaewyqver.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gqmnxnerv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqzlowes.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gwuglgnhz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjdmfvsv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gybvjqzdu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gltlzobao.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/glkcuubat.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gqddbaklw.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gmuetyqrt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gcajmzqmn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gwxcynrml.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gcbwwlief.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gjsmstfxd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gzinjqzwl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gkmnpmhiw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/grfuhbtxv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/ghdjyvxpj.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gnjwobqsg.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gwpmmybxn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gjxkstqwj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gpustejsr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gknzdmdna.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gxbbaqngp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/ghwocxehn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gkjqkylzk.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gjebmndkw.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gmvzyrihi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gfxqfpfxc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gbstgdnjc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/grbxxuzus.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gwvprehyh.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gxmtqehhh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/galaullvw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gkullcbre.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gqnazncap.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gvbhavehh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gpevbxdtu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ggjhaxbfw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gftmtrwwr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gohenwqip.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gxyckmyex.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gwjuptccd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gdgxgwtdg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gcxnfpdbn.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gogshcyom.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/goxtwjkfd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmyamopad.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gajqgxhkk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gowsdopuu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/grbrkdwct.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gzevywkyc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/goezppwid.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/geaftdhzu.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gdhpitqlm.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gkrhttwra.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/genoejzwi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gskorsoqv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gebitbxbx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/ghpuwadjl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gacworyuw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gvlddwmgz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gxcrbyagf.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gexjgnjpz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gdwqpcbsu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/goyqjstfa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gxyuoydde.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gaizvqnix.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/ghqnqbfae.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gtnsihhmt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gkzdbilit.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/giamtqtii.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/ghjrulqtj.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/grxbzotse.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gbcgtbpwf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gyoldfwmr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gcbmuzczp.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gatpwogss.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gwlighmfa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gzelmziam.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gvicmrtrv.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gjyftkoiq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gooxwbbak.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gjfysfati.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfupspqvp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdnsjmdvq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfsmgszvu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyaxaumel.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/giwjryqyu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gydymoboc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gbqvfrhle.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gleryxtwi.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/giajcfxmf.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gdtevhiyh.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gahgdjcof.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gynlowzeb.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjhqdhhav.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggnonpwuu.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkxyobgmb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gofzphpzz.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gnnyhfvhx.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gwuupepsm.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gpoqdzogz.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbxolxrrn.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gxreyztea.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gbqbvkdss.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gncciflao.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gdjmarjht.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtfzctazb.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gydtwxdbo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnbbdjoun.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gqlbepduv.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gehbzftps.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gkxtisjvp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ghlcrrtss.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gstyrvymq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtsaseffe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbbhsgtmw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gyfcmhglw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqkryach.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/goopswlng.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gyjowjkdw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gdnpozrjm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbfzjowzj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/giyjdddgy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gxznxthry.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gmquhawrd.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gwkdrubvm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/glxuqnhyk.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gofhrcfcp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gqynxsbng.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gnlvpvzfs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gxopubdfk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gqbbrqrwf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/glueintjp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gwojmgnkj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gjwxsazzg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gvtokutyv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gkwfkrbwp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gtzvdwwnm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gyjkkdibx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gsprgtkme.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gwxsrqras.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gqutqdrjy.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/ggqjbbydk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gewulnuqp.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gdtlmzwhi.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gzebvewvr.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gqnsjuxwy.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gvzpyhzda.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gotbkiyrs.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gzfbmrqdx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gijdepzoh.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gkvilyvtl.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gifdheogx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gojplktkg.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/glewbeqyc.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gndxbrkel.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/glqxgzvtg.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/grrwnlnjg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gkugsuzrq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/givpjzydz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gitwdxxse.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gtrgqtydb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gdjnhitlu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gmoxiwtlq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/ggoqkfuwy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gtdfeaojj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/grzaowuhz.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gzeladpmf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gthljwefn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gyxtyzetk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtiuhwgx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gvpnfzeom.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gsujcmefi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gakcdjbnx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gtyvywaqs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfgjsoidv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnyaelzo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/guvjopxob.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gjenpplgk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/ggjonwzfx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/grviurpbk.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gpvopwpbq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gklbequbz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gsailhxoe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gfmxovxbt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gsqwdmnvu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gwyrweheu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gdgnlqblx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gbnznlban.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gxuatzaxk.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gwuqedufy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gzlfmwqbo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gzxhlmbui.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gnhafblot.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gfptsnmhw.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/givjkjvtn.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gpnkcbyvt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gfnzcmarw.sHtML


<!-- 参考信息 -->