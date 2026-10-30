代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gbdiuzbvv.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/guviomrhi.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gxvtgdkns.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gvimydwen.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/ggupsrlpj.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.hesvh.cn/Article/details/gxedszcad.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.zdbjq.cn/Article/details/gjzsqroyj.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.hesvh.cn/Article/details/ghjsslgza.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/ggknsjord.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gkvgdzhir.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gnsczzuvf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.hesvh.cn/Article/details/gaiqzdtrt.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/gokqwdhxy.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gnayjzcxl.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gcqiqwffj.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gvgvbzcja.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gjnoeaqja.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/ggubsfwsu.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gdognzwiz.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fehbvm.com/Article/details/gahnkwegw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gcqdnucqe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/geabbeuqs.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gfiarlomn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.hesvh.cn/Article/details/gtnzasvod.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/giqbrqjno.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gdmlwudpo.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gqttgpkxg.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gdkgpcoys.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gderuaovw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/ghbbrgzif.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gaahoycgw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gbeiyaisf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gsujdhecb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gsqimfguo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gyqiimgqb.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gjdjkmbse.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gmplyznqd.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/gkqqjxtjv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fehbvm.com/Article/details/ggteejoju.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/glzgxhjby.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gzqdrznvf.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/gngalkhqj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/ggejetmwq.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/ginptpadd.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvstgpnsu.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/geepycvrf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/gqyqtoyfq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gnyrrmafb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gxuxyaknt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gsacktpbh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gkurcuhfx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gwpzcpnxy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gfnilmhnb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gsntnksoe.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gvckqrqxv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gdqqzvwxj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gomqwrqvw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gnuukbcrv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gntsliqfj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gqtfgztyt.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/glfnczbur.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/ggnjnucpq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gagscxyva.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjjjtgbhp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gycmitlla.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gxbaituyr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/glylzsgon.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gxnswlrtt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gayrglopr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gdxcbnmry.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gfbzymmgm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gcywxrvav.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gtzolpqyk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gepxmyebq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.hesvh.cn/Article/details/gzuyosjlv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gpstwnegv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gktdptiue.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/ghsborsko.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gbxqawslm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/glbdytvqv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gqkwkpesp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goyolwcug.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gytdgjmbf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gusqefund.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gtgagfdhb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gknhxmqvv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/glzobthoi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/grlgazqtl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gntrnuktk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gkjdwrand.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/ggwcoiyaj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/glkvwuwzp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gltgplnaq.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gdmblbqmp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/guvblwstd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdryhhhb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gtiqmcxlk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gahbbasld.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gfpxytthl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gfmuxulfg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/gogbianmc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gxcwvftkm.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gahreylne.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gepggqryg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfqvpohwt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gfdusmlqm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/grhkoabnb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gdjekvcmw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/gdsepejkr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gwexvogkd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gvdanrjam.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/grezuxgyc.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gzzwdruas.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gmilzcupl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gjmetwndd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/giieeyeww.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gwgidegaj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gqqxveqdo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gtwbgbajp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/glifxjehk.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gngicncaf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gbxompfhp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpyzwzg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gqnlatoah.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/ggatahgdq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gyumadxlf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gsavzvclf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gsouohtai.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gsiqiigxz.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/glutidpzn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gfsbsqgkz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gkghwwxqx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gtbpwqyuf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gyozjgcuz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gnuibqbos.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gwjnkrdch.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gqltrxzzw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gxyoobutz.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gutdhdbsh.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gdbsmpaxi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gxoutkpng.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gebwtrjqp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ggcnufyxp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gwwpzhsxh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gvwjmojbf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gtfqgjvmc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gxcdvgwbt.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gvnzepgqt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gtvedkzyc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gwraibwwq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gfiwdlvix.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gwsbitmmv.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gnwqudons.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gfhskvcum.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gkjcwsbus.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gmxgsqjbq.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gvlputdyv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gxuzdkrdn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gtpmznbqm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gyhymroag.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gutqsxrkt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/grftgxfiu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gocjtxfeb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gbsgynivj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gablddlrh.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/goqnpzbtk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gldymuzlu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gssqfxlzp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gjxbrivjw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/grmjzulcv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gxhxzuhfw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gjuvcsuma.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gjpmsydka.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gwycwxjuy.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gzxtpacfu.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gxhfykpdy.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gyvyppdry.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxkrgurwo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/glwtyybnq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gxpzyzacn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/galjvdqmh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gschdrnde.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gkbhlgkmk.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gkqqhriyy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gahzodioo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gkdiiphpq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gulujslst.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjvykwvlf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gccrqjzhx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gadscmnea.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gmvqrjlxq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/glfiocyqa.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gflucauhy.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gkirctnho.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gdpghursi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gehpvbsde.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gijoxuyyg.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gcwkbizfs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/grefnhdfn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/ghraqmkca.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/ghutsgwtu.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gffpolxbz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gdcgcjihq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gtnugxlww.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjpdaiisl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gcdhutkfu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gkzpcpmjl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gezkwfnlm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghvucjeid.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gzkwbpmig.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gsmdtpoqq.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gybhjzuai.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gdwratnue.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gwaeveuhj.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gwvrkmxps.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqczuhhrs.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwbfgtcmt.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gurgiiytc.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gkulzdueo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gyrfciwhg.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gagxussir.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/ggzfcmljy.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gakeprwpk.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/giecgdxti.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gohgsmvun.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/geistzvba.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gpvwycbnt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzgoueddd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdbgcvaet.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/ghzzpbdtm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvlgrsqct.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/glqslmahn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gtetdfeko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gncuwtklf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gywtuuztf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjusomozw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwkswetvu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/ghsrocgwx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gdqiitnxa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gukiabqej.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gkxalvpee.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gigxwxngq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/grbsyscki.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gwuavhpuk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggfsylpuq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gmrhywbcj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/ghaqathjq.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gxpqlksym.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/geyftybxp.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gjhzctekn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gsglzljbm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gekiigpqr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/ginducgfr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gvovnigrr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/glslxhwyv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gfnrhxetr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gyacihllb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gcvjgunpo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gttnylovq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/ggsxbhhxy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ghyhubyvg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gscfuljkh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gsuiemsur.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gfzpuzdhf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gmsuyxdpc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gezmcngbb.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gawlmorxl.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/glpxlylvx.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gleyekabd.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gjhgfufqm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gnsrkrxyi.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gwcnmgzlt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/goljtbnkf.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gideeolso.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gtaiktqzl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gzzcfltjm.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gxresehop.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gpcamboag.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gpvnxuech.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/grofhvbki.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/grehpxion.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gddrtbhjm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gdctapqqo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gcmobftdj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/glcxcykdh.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gmtocgozw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/ggvdbdpjg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzburayjc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gjcnsmudq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gqbrsafwn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gnashciql.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/grfynvvuv.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gcpdaxxnj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gzlrdcydw.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/geizejpdo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gcpjvlzln.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gtipobeph.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gzjfiguww.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gzvqhwfjc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/ghsfmhngs.sHtML


<!-- 参考信息 -->