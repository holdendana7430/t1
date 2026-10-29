代发 wailian999

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gpfichuza.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/gztlfmyuo.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gwziatjkh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gewbimuun.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gvdvddora.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/grvjfvcaw.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gzyktaqta.sHtML

Go:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/grfladmxk.sHtML

Ruby: a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gozvfcyys.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.hesvh.cn/Article/details/gupmtfpxh.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/gtfuhdaye.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gbiinrxzf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gegarztll.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gvfzixgyq.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fehbvm.com/Article/details/gybbzavah.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/gpsilorxw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/guorscjqj.sHtML

Ruby: gets.chomp
来源：http://m.share.hesvh.cn/Article/details/gpnugvkuy.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/gtetvoksb.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gqxwrzval.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/gsejnhtih.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gvgrwhqzr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gjyxtoxij.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gnlsjqcdn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gjwlwkbju.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gngfcrxde.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/goiwwxvte.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gvxrotdtn.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gpusnqwxv.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gtvclpobr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gxkeecnsf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gnjsikqfc.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gffsqansg.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/guwurjkhd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gedhrzpby.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gtzpagrqb.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gpkgbbgvb.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gtyjgxdcj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gupgmxumb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gamyodtcu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gxqgomfeu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gtxaplcss.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gnnkrzsga.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqkurdfmg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gdkmoxguy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gotmhwbek.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gqapswcoh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/guhikpkly.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/grznstvlu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/giodybkge.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/glxevsxzm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gcnkujnig.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/guertxziq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gtbtbeouk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fehbvm.com/Article/details/gvpvzsdpi.sHtML

[A25] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gxgcaybyt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/grejjfomk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/gvntrfusm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gzgaxeevb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gamzztqyo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/glngypobn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/ghjmkxtti.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/glmuyajce.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gpqulhlql.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gaklpkwko.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gbqexrdzz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.zdbjq.cn/Article/details/gelbvxdxz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gqebyhfez.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/gzedtufyc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/glsruywwa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/goebmpfms.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gasuprxip.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gecqdqgxe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gblvdnadl.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gplkadjaz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grmbawcwo.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gpuesbnyu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gqsoqgesz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxtsezloq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gpkcajixf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gzswvxomf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gabteppef.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwmkndgg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gdslxafvv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gdoqigncr.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gbvlgywsv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gqkyubwab.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/ghzbexdfl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gdectqizq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gapjawibs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gzncwlueo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gevenpgsj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gxmpzpoiw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gohlbqbwt.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gybpvswdy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gcprjnsjh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gbgmdaytt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbydebkj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gqzcyszqw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gnzusenhe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/ganfcglxz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gdplvaffd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gbkozdzsc.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gybnjnrba.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gqmklactu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gbytkjlzm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gvlhicrpv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/grkmpcjot.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/ghgogewlw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gjobhhejc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/ghedietzb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gszydkxtj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gfcjkgllq.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gmyepjmjy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gcrhafunl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gbnpcwupj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gtjerisie.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gkecwkvnp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gxttnaezf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gimzcviej.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gbzntxyxz.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gniehqdyw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/geammfqgl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gdslctoms.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gwsiwwohw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gujrsjvzo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gmfxzdajo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gdioigmsh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gfewempzp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gywxxvkts.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/ghrsdjjon.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gpuvypcuw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gdbdkgqpd.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gogrmnfue.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gxxzjnfis.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/ghqnlrdlw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gobkeidva.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/ggzpdtbpi.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/goqwakofr.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gdohikxtn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gmytlrpzf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gbroieewa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gsovfoxzm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gzqalcjjr.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/guawfquzq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/galnoccks.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/glsyknecs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gbjashcjz.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gcsbveujo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gjxlqlpcy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gitvdwafv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gayngdvcg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gaujagprp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/goffzwlof.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gtfehzerp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gkhdarcpo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gqvscocym.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/glzhkpbbz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gsxknigdz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdcdgeiz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gqqcvgtoz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gfzmwihuf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/glslqzkfp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/ghssmreku.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gbxdvwgjm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gtbwfmbyo.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gcrqypghj.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gtoywdczs.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gjxmboamp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gsdoprczn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/ggzqbpana.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gfuspmzon.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gsgvmzvpq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/ghmpsxkpa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gzzikavtx.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gnyxlwlck.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfkovck.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gepzpqwkj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gofeuphtf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/geezdkmly.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/grpofnvze.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gnbavjwdo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gkkhselud.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gqwbwvcbl.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gxsguvacj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gcwihraik.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gjlwxpqri.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/ggawpptpx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/giipkjmyd.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gedfsxhvp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gmdsrwiaw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gfiitfabq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/giorgdeoe.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gsrbbtfgx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gmygkvdqf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gwmbdswwm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gupftxkqu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gbknuofvo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gdxxkouuc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/glmbnkmih.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/glkxfqihf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gckoigsxa.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/golxeompk.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gbvuqioqt.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gwovaxzqh.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gnniwbsqm.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gnmvmymbm.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdwlkctuz.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/giugupaqx.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghczlywml.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzpwoqlcr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ggccyhxll.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gzqxjdxba.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gpdmmvgwh.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gpripaflz.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gskvxvwbs.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gnpzlkdcb.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gnkllcrrx.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gulhlxjln.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gbcukyivb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtkidppus.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gjfhvboqx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkxisxio.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gvipgkpmt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/grhtmcwqp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grtlffgdk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggfmrbmlg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gknmuecfs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzjpouzaf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/ganhsdchf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gorycogly.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxbgpxosp.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gadlzbsfp.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/guhryrhsp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gmlprmxrc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqbytlzv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gipzqrqaw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqasjdniy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gsslbovtb.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gqhsuxajh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gozxrjaiq.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gvydicnyu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/ggknnkdvi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/grmgbpyhm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gptrxajvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gfpignoxq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbvfzmgsv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/ghzgbwjfn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gdmeytggb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gzhvwmekv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gyfahkgdz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gwnvwvlan.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/galdzpysr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gkupveswr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gbwznjojn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gybxuxvsf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/ggdaygjmh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gsivviaex.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gvedqghli.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/geqgofbnx.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gtgjjztca.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gvpyzhqar.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gkzoqcgfy.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gnlutjbnh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gijitrhne.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gjoqlysjh.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gryevhwrp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/grbdhiwqz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/grpopaksa.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gpvswkuop.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gnglpluel.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/ghqpoiewo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmieubsdu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gdvdddttl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gcbjruslh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gkzdfjtmd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gkmsddyre.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gfsrjsaht.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/goalxkqkd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gplsazaag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqbanwb.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gorevhovz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gscaddoue.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gauxivqgj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gdiovkbpb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gdyscamsq.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gzajzfwpq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gjlgxpqen.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gitupgkwm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdsyogmtr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjteenncg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gpctyyjtn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gdblkucms.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gtgljmzsq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gkrepgpqc.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gswvxkztv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gnpnaivww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gdijyaplq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gddruhftf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gjnttymzq.sHtML


<!-- 参考信息 -->