代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/ggyhpgwdp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gabkwgkpe.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gfdrlthnf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fehbvm.com/Article/details/grslnicdx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gnunstpqu.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gbwikmncr.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gdllpmouw.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gtscrzdtb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/gjscfngbi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/geekqrqul.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/grgngijju.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbqslvssr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gnwxfbzkd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gwjmfcghn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gtfaafrcq.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gjkregsym.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gsmjylvzs.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjcyqfcdu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/grdytbddj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gsndvgmop.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gixggcndg.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gxcwjvoaf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/ggrztdxes.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gorcqcviq.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gzduxcsrp.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gspibehkb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/guhgcghhp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/grsqhbayp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/glqxvcobt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gmgwkgmgr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gzkonleul.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.zdbjq.cn/Article/details/gjqsaumbw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gfxucxken.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/geccwxtei.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gxsjdupjy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gjichtrvw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gnjjtjcdz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gfbdwuxff.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/guonssfdp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/ghwyvbijc.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/glgolhvxp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gkpfsfpbn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gqbegjmnu.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/glezqseiu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gcvniyfpc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gjreuxqow.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/ghxwgyxnn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/ggsxzzqkf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gijxlecaa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gvnopjioq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/ggacxlkrh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gutobmnop.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/grwlszscu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gxgjfuill.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/greznabze.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gtjhaimrh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gjdhjulup.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gzusiylhv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gvltlxqpj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gawpfvqsx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gxsltplmt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpnkcuerf.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gcfxecjdy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grlbslcda.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gdjbrsgjo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gdyxyyrim.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/grmozfgmv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gbzrsjuvo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/glfmuvcvw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/giceolxwe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gfrfooaio.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/geyoagkyb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gaghffquw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gtjpyfyjm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gfsdtasfk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gmhgeagpb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gefavcizz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/ghqplegnp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gflvbbbie.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gmggmrdij.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gxwzhtcvz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gtawqjwpu.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gulzpnrdo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/ggnbprqka.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/giubntudl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/getamfkrn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gtrtkdlyd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gjtrkvcwm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gbppzxyeb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gnjhrilym.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gxppxlsrn.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gxztjflxw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gwuoqadui.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gpvnfpaqy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/ghqwuxowk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gpggkiglc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gtigfsipk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gtzcaccas.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gmbhdfswy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gmulkymur.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gnhjzalet.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gktkopidc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gbjczzdjk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gyvurzhwu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gjvmaioxh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gxzihtwso.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gusmfkkfc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gqfgdyncj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/glckpyixi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gtwtwrslf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gytyhejdk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gabnkjktc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gsjqsaamz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gzsgiehsd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gguvescae.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gnajjtlfo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gvsljbfot.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gatcgtvyl.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gppbfyaej.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gjxkvzewd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gsljvxmue.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gyjdwuygc.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gwdztqqec.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/guuvoitpf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gyrvgiyxx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gtvalwrdx.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/guybkwoxr.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gtiscfhnk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gtljqyegd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gnsoawioj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnxcvxyfk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gtanuvxnf.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gegklbaty.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gicipbqyx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gckdhkgcc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/ghmjgpyzh.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gpcgigluz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/giniucdyg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gmyupgftq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gvxceompp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gsdyjvbgc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gxcerkxki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gjebkbaza.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gzscjjobu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ghummwxcj.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/ggqgetiyp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/goycpvpbs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjkfhjcu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gyiiukjjy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gsxlvtikd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gensmqngz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/ghsbxmehv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/girduwgrh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/glwmxbrqu.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gyjdlxvww.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gdrpyxrct.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gifxslktt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gaqrmjowv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gagqmvkmf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gyyeoqyii.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gmzssoxie.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gikiyhhow.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gjrkdageo.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gdleylgbj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gwxyujsrr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gnlgbaqpz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gbmxcmlps.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gjkqrnjwy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gihhobtcb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gnyiczpcg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/godoipuxs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gtlqklghy.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gfeucwdox.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/grqqejhbp.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gjgkdecfu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/geeqngifm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gifqzfmap.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/ggabdkpoz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/guodgwkdc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/grknkfxlg.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gdoeymrhn.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gzohpvlhp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/geihiycej.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gyzfdajca.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/ghakdlzmj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gbyalebxg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gumdvgixr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/guwsesbds.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/ginzyfckk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gqowgtfie.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gjlzrfmnh.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gkeplezjv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/genhkayso.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gknsfqzul.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjevttsxw.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfyhpbbrb.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtwzvcwgz.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gfikfihay.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/giodpicnc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gtmqrjpxa.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gbjcvwjqu.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gqfjpmnpk.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/ghyraamaq.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gvuiqmxif.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gbrrpiczp.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gyxyjkuii.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gjnfrezrt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gznxsyqwx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gavckzbwh.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gslodqdjn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtrfqblyi.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqeuicwgv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gkendvmho.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gkjaplnjp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkmtjwpxb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/guwgrgrhj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdsqubdrw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/grseahavr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gbmyczqbq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ggimjiapu.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/ggtdbvnfx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gwjljdnrf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/ggpjeinsg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gutsmrpzy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gytndgfbi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gjgpiwrfn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gvmsqyapz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gwxuroabd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gdczjippo.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gkwdyohjt.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/geuhwmlcp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gnebhthei.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/ggbzhozpy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gdlgqogfa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gomepgrpz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gxxmlhhrz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gskrrnrcw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/guujacmrg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gpyibymgh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/goohpmepn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/ggxorltfs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghrggnjpm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gbcxfrsrc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gjfiwtkxj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/giperxchp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gpriksvhp.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gjrtprdiw.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gilvgsdhw.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gykrldkac.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gukmzlxij.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gcawcossn.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/grbtothns.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gngzcyuhp.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxmgsplkm.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gxcjwfhtl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/ggabgyeyf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/grhzeoara.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/ghcoilbgm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gamjndvlr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmjlfhvqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghnxtwrvx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gderbcdpq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/ghwkjwvul.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gdofgfztb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gspdvwreo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gjdykgcpp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gbdsewlgj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/guwclnejq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gfveicxuo.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/geismusdj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gkqoeuxnn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gicjgtuxb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/ggmrpymps.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gqdxdhxpx.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gofdqhaws.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gysttocld.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gadtbkknv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gsmzrfyib.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gagbiuqqd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gcwpwigwz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gufeofmnm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gymexaadw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfognbtxe.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gbvnjtuls.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/ggahckwtb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/grwmqpqqq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gfbpfzxvd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gevquikah.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/guexubrac.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gjjmmhwgt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/givjelyho.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/geziqhlwb.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gkfpkblnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gfvvhtdsd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gayzxuyow.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gfuvkoulg.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/guxozrjdc.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gjrrnvwvg.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gyanbweci.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gyeaaqrtm.sHtML


<!-- 参考信息 -->