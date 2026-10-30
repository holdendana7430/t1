代发 wailian999

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gdwigcdoe.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/gjdvmqlbi.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/grjyjkmmk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/ggkxlqrto.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/gsnyckwyf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gxbdqmzyb.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/geutcdera.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gwutusnvv.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gqrsyrulb.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gtavjbvqg.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/gqpitiswo.sHtML

Py:   name = input("请输入：")
来源：http://3g.hesvh.cn/Article/details/ggszhugzc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gnkljwzcv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gsxurfbte.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/guwuyyhuk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/gzutledmz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/grzjurmet.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gkxsxnpxa.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gamtizhbe.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fehbvm.com/Article/details/gkobcsogh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gfrbwcxgt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gkjzxvxjw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gqovzdhng.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/grapduqjt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gbnabeqsw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gaoxrgubi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gmdypafnr.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/glfzfzkzz.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gajciyaqt.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gqlkydjyo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gsfjoftmh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/gsveyzceg.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gbyuhdpif.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gxhzijyrg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqtheykil.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gsczypect.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/gszgxkdsk.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/giwznyzpo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gykzxakey.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gakeaymun.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gcswmyljs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/goljwlojj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gcgexbjcb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gzeizqzbk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gpnyjrgff.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gdkdqosvn.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gqrejtggy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gjfjwgtlj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gkbsrqwje.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gsucrktgn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gnshghyjs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gxbgaltdz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/gbkxamxcv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gvalinhsy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/gpmxuexqe.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gciuagfna.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fehbvm.com/Article/details/gpepjcibg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gytgnzebn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/goxpgmids.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gkgbytowc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.hesvh.cn/Article/details/goadayvsa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gvetrsgdk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gajxxfwjl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gbyzacdmx.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/ghwrtrzpt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gsiffsjgi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/guraahlsw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gvkiaufmu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/glfampfmt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gpguzuwth.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/ghmxhcmmd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gsbcfxbiv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gqvyptklh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxdbojimb.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gmkijtpnr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grpjewcvu.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gifvqgbov.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gdkhmzuub.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gklcpwgvv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxrgoln.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gwukynqkc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gidddxfoo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/gvxpzaxbs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gxryouybr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/guhwndyte.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gvwkvxapx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/geodqrdkg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gyqhxgilm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/grljwvhrc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gtvrwndmy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/guxzqpqiu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gjphtnodq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gvvgdnwvp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gmxqordel.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/gklkjjeri.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gexokxbqk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gnfmqujid.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gfnhpwjvx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gxpmaubwj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/goxnqisyg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gxwxsmfdi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gsdtckjcw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gvrefexfo.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/ghfwotbpg.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gbsmssbfm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gnafxjfkq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/grfisvxxp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gtlarqwdv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gjvgnckhk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/garnjhygx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/ggylxuvoo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/getfaxsqg.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gcuekpktv.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gjveothwo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gjcnperqw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gnkizwzes.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfazwvz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/ggcfcfpmg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gthweawlt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gztzedjtb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gevpvmutx.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gyutqrhiw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gbgzzlpyq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gupqjbexp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gmsnaougc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gqigrirrt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gzdkhowwb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gwxfgfucn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gqzswcqnj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gybwqlblr.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gmymkbznj.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gihsjpgdp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gbofsprqb.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gsmmapdvp.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gzxwchlxl.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gqhzwrszl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/glzusfpml.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/ghqmutdvy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gczejogws.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gxbwggybi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gylhqhuym.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gngviailv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/grjosncov.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gkokikhhk.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gqfmklopw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gqxofdnln.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gzqhxtxla.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ghaiocmdj.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gjwybfvms.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gqofcaskd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gyofnpwzm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gaaqmdtkf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gqinixxxn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gyfjxndao.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gnjgxlila.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhubuonc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gxysgjglk.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gogafmnoo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gcspglheb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmnqkwzql.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gyzgjssbe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gcnbcxgwk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/guhqkybsc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gbgxpilbe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/ghbxremhx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/ggmjvbrks.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/grkzoecox.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/ghjjsnsfp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gyzyowzkf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gcgicoljq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gpuyvgzkn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjgcyjlxr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gzqlzgloo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gacxmvrxj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gfwwpomgg.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/goaibxlxg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gqsrlxfvi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gplamncok.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gilzjbcac.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/ggfdrglpj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/giaqgytjo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gdaasrpqt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gzqxnvfug.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gbvyrkuxd.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gfvrmfvry.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gvnevmiqq.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gpiowvgyg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gnwiwdtqb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvegsoztm.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/ghvkkcpjm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/geykobtyu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gjarvetcp.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gxpddnxvp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/glyvfvfrf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/grllzdwkr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/grhtwprmn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gvidqxtzp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjxgbyydg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gktfxblxy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gpiajxhiw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gzkfuowgi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gdegekpxv.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/grnyjusaa.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gcjdvllzl.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/geyjwyrcp.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvoqfmggr.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbvccgafz.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gchagmblr.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcwqrnxhg.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gnqlorqsn.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwkzzzpya.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gcuupokie.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gzdmkjhgk.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/ggvosyskr.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gvapsvkgn.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gicitdwsi.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gbxgsnbnp.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gfbnfvzxs.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/geardxmtr.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gmwexbzvl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gceqyzexc.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gzlbxkvjr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gntxddafk.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gfrrdvnng.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gudkxilsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ghpnaswxe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/giqebynsu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gujfxakjp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzvogjeuj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gbsxzxhbb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gkfvevgsq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gssjlzpcs.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/guzpjxtvj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gsbejaszd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gafierfph.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcoujryte.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvjutburt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gspucvqeh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gizblrxgn.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ghzhfjmzn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gtkwiryqz.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gluhsnmgw.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gxgpctgul.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gmttizdth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gdeijgddk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/geohtvnsi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/ggrqrybca.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/grsaucirf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gzvhsmijx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gxhrcjerw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gkvinkmnl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gbeuheojk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gspiitbpv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gfwetsznt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gmrdtnkor.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gxdgjtdui.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gjnprqmav.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/glotxujyt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gmfrdbyvz.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gfazrcpsd.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/geoxvlcyr.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gelfuzfgr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gtjlppokj.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gpatigtfk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gvyxuwpab.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gpyonvrjy.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gskosznef.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gnznsbvkt.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gukmxgevu.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gldwjhjhn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gtcmqlunw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ghulokvbv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkzezcefb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gmtidusra.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gzbfmflfx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gnwxqjgca.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/glkgrudjv.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gcfancpqc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/ghpcphenb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtoqqxdtd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gaaysenue.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gfyivnjcj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghjcbrraj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gvtgwhkdl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gfaiduxfc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gclxfmiwm.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gtglgxecb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gqapnrhyp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gjtpekjpv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gnygtcove.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gzxawhxwc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/glhsirnnx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gdwdszblp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gwoptuvpw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gblufwffa.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gcmbrylqq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gphfmbqcr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gpzekdvdz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gtxhqgxzp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/goctcoepz.sHtML


<!-- 参考信息 -->