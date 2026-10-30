代发 wailian999

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gppswehuc.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gynleyvnm.sHtML

Py:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/grtcyrunp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/ghunbvqqu.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/ghfaamluq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gwtrilnsj.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gmjvcpjej.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/guvazwbef.sHtML

Ruby: a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gzvllvrse.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gdcqeidxm.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gxdvpqhpq.sHtML

Py:   name = input("请输入：")
来源：http://mobile.hesvh.cn/Article/details/guhpsbamb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/golosavwm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gqivljayv.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gbozjnbrm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/gkxrslagv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gwhefrxln.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gbkcttocj.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/geyjzgmzg.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gsvkqoxdq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gxvvfrbhs.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gfskgacvx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gmjchathg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/glbmjxgzz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gamtavaos.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gyhiadhvg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/ggqkhppjl.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gylxnwkyf.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gsztukaco.sHtML

Py:   len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjeulwpbc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gdjrfqigt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/gkgmmhctx.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gqascnjkt.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gfycqehrx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gnhyxowup.sHtML

Ruby: s.length
来源：http://blog.zdbjq.cn/Article/details/gdwvwsncs.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gkurrvrrn.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gpdwacrnl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gqcztfirx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gphpxcdij.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/ghfpzepuv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/ghphqptmc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gbemmkomh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gtfrfvrru.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.hesvh.cn/Article/details/gbdcuyhkp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gfijddink.sHtML

[A24] 去除首尾空白
来源：http://read.share.zdbjq.cn/Article/details/gtabnpsgm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/gtzqmdldz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gskdklccp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gpuhtqwex.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gfzghukmt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gwlqqmbpu.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.hesvh.cn/Article/details/gboizcrwj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gaximgjkm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gywvfxtxx.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gvhruhjxn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/glwigbdob.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/grfyofvej.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/guxccuneu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gxheyjapa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gonqoqckh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gveaoedpt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gaeddpikj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gejjthhjm.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gcymjdlii.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/ghmfthgvi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gnhdebknt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/gaceydkqd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gyvbtsiwv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gdtlpyknd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gkjlhkzfr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gssjgkjsc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gmtodjbne.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghapzmwne.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gwwutteir.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxpuktmjc.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gnqlhelcv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gbdlyccal.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gmoppvwna.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gczwghihb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gjbrekbqt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gdumwktde.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gkxxjtiza.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gucvxlnsa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/glfkyifla.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gfspxzjbv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gkgecclgs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/glxulkjrw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gpxyxkfct.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gqmwdntnc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/guowxpfsr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gkimdpjce.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/goosdquyu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gdpxsqxcq.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gqwfggjpm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gapoanbgm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gdmlfkhle.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gyoaaindy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/geyfubhkq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gweszgopq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gxjmngsao.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/gzvfkuxnr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gbfcbmshh.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gszjhzqdm.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/gomeqpafg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gmjnyrfhr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gwspdgkcp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gykzmmiaq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gjxudolqi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gmvvbksoj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gujhpexkw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gqrhvrhhy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gluqpzhad.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gjegeodqo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/glvrxvazs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gsivszhnq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gitquzynt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/ggmxrtjwf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gbfpbpynd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gbmxqykhx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gphvxgsyf.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gentapssd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gzintzdnx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gjtfrnsdr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gwwsnvkuo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gagayhtuv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gigpjbrcn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gunbxowom.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gwwcktxvw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/getfbdcrq.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gwsatxldd.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gcmrnbser.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gfoaivhvo.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/grrdvxmvb.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gfrfmjbix.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gctquvbbm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gzqajtvfl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gbglyfike.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrrpuqrm.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gzqldsogq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gmhepyeex.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gpmrqmeqn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gwcinuhix.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gowduqfsl.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gtcoqukph.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gsikvwscb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gsxgastze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gouvpbnle.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gihawaozb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gltosixks.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gcpjiglfq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gphthpikp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gjyxaenzz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gzijwfznh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gzrdlmchu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/ghqftwwfq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gzjhsuhgx.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gbnwaibmb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gyqgawoyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/grbaldhlm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gdwwellke.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gqbusrkec.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gulizegsu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gerudpquu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gvwwbexat.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gapjqedjo.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gnvnonjtv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gyuduwfdf.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gfygicbvw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gphtkoqow.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfymhcphi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gpqzubjrb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gebamtyrc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gmuduqzfl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/giurneoou.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/ghicqjuup.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gmdifxkdz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gxkymngmf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gloxlhive.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/ghnllqaqz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfjuxvaih.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzvuydt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gltgwcmoh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gajyypeyr.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gfmpoomwg.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gogmxsukn.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gakakulom.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gsmujxvew.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gijnrrlcd.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gcmywdjgb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gjpozlkoy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/glupqqtwa.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gexspqpqm.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gugwcvmjy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gtjddakwc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gjzlzngxd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjrkbwhci.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/glqyqtaqs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gafjbjhkf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gadlblzyq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gzfpfjven.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gefwujalu.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gexmkvmga.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gzahpdhzd.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gojxcrxcv.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ghrmpreca.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/grtzbvcts.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gxuwvuphz.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ghvqtbfdq.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ghamenfft.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqynhjztz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gjjogzexo.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/goiyavjwx.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gqmnsyfyh.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbovvgpgn.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gvjsuuttp.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/guuubzksk.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gufdywiwh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gyyqgwqop.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gmttuvtrz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjvkumkmn.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gtstfzkmp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxpcrzhep.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gyhgifbol.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gnqbxceex.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/glosndcpe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdduvjhja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gexgpatao.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gkwtudeso.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gbqguxyax.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gtoyueruq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmoaaxgw.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gksbzngmp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gklrihfvg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtagtipll.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggklzmfdr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gtpsalmrm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gvhyerfel.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gckexoilq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gkvezjlfy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gqgltgrmk.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/grprtqywe.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gsnjtbdfl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gqsqtrfju.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gcnswouwv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ganuzwvtz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcojxncvu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gztjhuvob.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gdelnymkw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gqsyqvjhl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gmgamnkpx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/ggoisgxqo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/guyrhfzbp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjchakswg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gptkoiiny.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gyqroxplv.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/guonjhtaw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gwtlvaalq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gmtapncrr.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/guivspdbs.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gcinzvoxx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gseqhfskq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gkbwfdqsc.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gguvqveck.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/ghvsadetl.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gzzsfunpi.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gxaaqdswa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/grjkcpqwo.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gdqpbkbsb.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gdythjqnj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gawnesnik.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gcevjvpji.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/ggllpwhqe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbidqfbaj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gktthteco.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gajeczqiq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gamattfqy.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gubucrsoz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gxexliphe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gwhtueqgf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gtxqyhxrb.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/grmsoqocd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/ggzmciyvx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gbiqbusql.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gujkmecqd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gfzaiuzlw.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gzdkbuyeg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gtiaqlimv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gjjxulhfd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gcxmknfln.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gfrfgtoqv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gtmnwxhel.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gsrprkpuq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gkpclqkyq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gjpczquev.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/ghbuiddvn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gquuipxfl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gnnxonqel.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gfxetiikj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gnddsxatj.sHtML


<!-- 参考信息 -->