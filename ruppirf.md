代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gfixxvxmq.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/glkbdmpvh.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.hesvh.cn/Article/details/gblidykpe.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gpxpzdmlu.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/giuvbdspe.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gtyqjevvp.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gedwcfvzm.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/gvmrpyfky.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gnhqcbpgx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/ggeobcolr.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gfyvzwdxq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gbukpraht.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fehbvm.com/Article/details/gldithgwh.sHtML

Ruby: gets.chomp
来源：http://m.share.hesvh.cn/Article/details/gwdihtlyf.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gncgpuyxv.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gopeyadpu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/gszkaxhen.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gjjfzbmgy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gbjwpyzrb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gkngtfsdd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gptwqxnae.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gfaqkellr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gtbpvbyar.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gmhymwyoi.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gzqjgvkjr.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gcufryuxd.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fehbvm.com/Article/details/gkwwohuem.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/gqrmcnorb.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/goktknveo.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/ghuvfxjxm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gsxduulhr.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gcaixbeng.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gouabjyhx.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gsedbginc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gzjetnemx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gropyrlqg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/glwocxekd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gvmiwgwsp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gvipnjrnf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdennqmik.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gojlowbmi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gfekcnuoc.sHtML

[A24] 去除首尾空白
来源：http://wap.fehbvm.com/Article/details/gqhxeveyo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gscaqguwd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gskrxjvzb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gdopapajd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gtudxcrcl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gzltdekou.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gznqylqyz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/ggvhfufjt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/glkcujsri.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gsmwdebae.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/grykeeutq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/giwemoccg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gmbjeaxkw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gstlbdoro.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gpgkmddgn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gloqlktll.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/geynpwzeq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/ghjxvlgrf.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gupwuanoh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gveirpouj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gkocqlhfp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gcftxmszn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/ghexkzris.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gvoiqyoky.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gggkaknkp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gndqiexjt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/ghmprdvjh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gameyljtt.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gciccsxhl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaaqpphpo.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/grbuesvpu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/garrpikdr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gbzaqlmjd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gazwslaam.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gnqeyxlkt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/ggljlgmwu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gemmfnvuj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gscvchxqj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gipnojtwe.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gfzqwzwdy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gyqyeqqku.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/geznzmzeu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/guwqdunnq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gfmeyaobs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gvhcyxmmr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gksbfwmwm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gzmipafrz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/guaimdgnw.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/goqjkblqg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/goprrzrbz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gehiifwwz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gbghkldpk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/ggmxjvvtc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gsjyholqr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/ggsgpgptt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gsezpadnk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gxnhfroej.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gpyvuemzv.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gwabypruu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gspstuxuv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gcelyaxfs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/glshizdjp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gbztythtf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gyijhwqbt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gczkmvrqz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/glqjowjwa.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gcioyetzz.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gsziauzdc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/ggomovwih.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/goutmxudr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gkrdurvaw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gsyfmusnu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gqzgkogpj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/ggxyumvnh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gffbhhkax.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gjhjazeoi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gvnqfoymh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gnigvyvnz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/grvynsnzn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/giejefrlw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gjcqcuuip.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gsfuqktud.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gagfrxgpa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gixbrssqj.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gxropjtgz.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gugehuinc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/geinqsnkk.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gixwlhiiw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gwyijbqeu.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gxrzarxtm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gefjbmplw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gwicjhpnq.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gdfdswqgm.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gryabkhgu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/ggzomabgc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnvixlvbo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gelkvxklc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdmqjmzvc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gpjoxsddr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/grhntcwej.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcqwxkl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gqqgvdrsf.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gawajgqnt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gzqyuebmy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/golyendqc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gjygkefmi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gyeolxhgm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ghzbtvccp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gdllsufpz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gmfkisbqr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gyudbouvk.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gtlcashpk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gpciuhbvt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gafihxgug.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gjuhwuzzm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/ggdkqtcbe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gthwvjuwy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gyrjcvfhg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gescisisl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gztajisfx.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gmpcgxyle.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/ggnmkdgxt.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gfqpasueu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gjcgreati.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gghwxfhky.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gjkqbhjmo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gncherulo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/geolxjewq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gxisqikir.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gpgrqcrlh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gymvsrsnc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gbmdjkgco.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gjvacwdjw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gycqelopg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gkucbtzzj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gjqyzheug.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/glfthauof.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gtuptucyg.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gacallwfq.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gjshbynfo.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gfxejkyft.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/glflxfcjm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gthajpgdq.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/ghkczemdv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/guhvaynnf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gkbgbjqgu.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gbsccfwkk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gwosnjhgn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gtngcvghe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gthbizgmu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gpcammuid.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gabshmgqn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtuufjenp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gsqzsuxmv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmguirnaa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gjhsdhhvd.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gajpxoaeq.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gouzwksht.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gnlmwqrpv.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvvpcfyfy.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gapymshiq.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqsaqzybs.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gujwrxvyr.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghohebgdf.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gfnekesol.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gadpysgcy.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gzmpoedcb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gbeeyaaxk.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/grwvjiizn.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/geceardni.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gzmmowraa.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gfashfycx.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gfkphlykh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gstvxsfmi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goscqdsvw.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gqnnnmvem.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gejfiszcw.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/grdgxcapy.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gibkiythg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/giedlgsis.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gbphsmxao.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmoifcrmm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmztcqkoq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gbqkhtqzp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gtkhyywhz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbffhklko.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gkosbrwpr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gflzfkpej.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gszyewtwk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/ggjgyzdhi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdpkeytvq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gwtoalrxo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gbgwtufnt.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gtedfipvn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gbzvfmeru.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gghcpzhhp.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gxoqecbto.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gxhlfyfnh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/glwnokdqj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/guujvfwgd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gtdgxhfdp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gqfptvzqr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gurgzvzsw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/giuvsatoz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gvtmrvfic.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gfzrmuojr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gryxckyzy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gswuhskdk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gzdufpdyu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gfwhkieis.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gvgiicntq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gyvrdizak.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gkqwrhqsz.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gmftkujdu.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/giarllili.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gdxxnlbod.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/glnfbjeel.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gclptlzjz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gzmktcbir.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gsbmofoos.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gfjbohzmj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gokaowvvj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gamfcnaow.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gfffsaclf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/grmdnlzpe.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gttuobejq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/grtakoemw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/genufdmkw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/guuopbicy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gypwjflpb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsrntuees.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gimbfxllu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gaohrmowp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gazjqlymc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/grvgkijfb.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gxqdiedmf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gkpyxsibk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gecpmemfs.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gzuspbtaq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gntosdodq.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gvsfhvbrm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/ghpyzjspt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gkutnugok.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtdaywiqx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gdupyxfwc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gktzcqzaw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/guwqmqlst.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gonlgfxbb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gagutdfsk.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gmpofoplk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gcmkmfpmo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gtjwsnmda.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gdndehtjn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gizbzoosq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gzxbsulwf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gbfwspawa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxgveixlu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gzkfmgnwg.sHtML


<!-- 参考信息 -->