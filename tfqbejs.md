代发 wailian999

C#:   (int)'A'; (char)65
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoqnwgrs.sHtML

[A19] 交换两个变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkhdarnsh.sHtML

Py:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gsjrvsncb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fanxiaobao.xyz/Article/details/gwrpyvsix.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gejmpgdkw.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/goyituewu.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gwspodhrc.sHtML

Go:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gmnnentgw.sHtML

Ruby: a, b = b, a
来源：http://www.share.fanxiaobao.xyz/Article/details/ggishxhni.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqzocewk.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gekigzpvg.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhvvkeon.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtouqrdxo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fanxiaobao.xyz/Article/details/gvqhzbaix.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gbkgzmkrb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fanxiaobao.xyz/Article/details/gakjlwxid.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeuispxw.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gdrfrmbbx.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfddwmtp.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxxjlkvk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqpyhuvz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozdkcjco.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gozkpfekb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksooqwxf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnzbognx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdmoajdy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gsshsqsyh.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fanxiaobao.xyz/Article/details/gdywbbewv.sHtML

[A22] 获取字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gyicfasos.sHtML

Py:   len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwbyodzi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/ghywrlxgc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxpmrmnk.sHtML

TS:   s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/guilogecf.sHtML

Java: s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gozkotrfb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gurjirboy.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaujomgox.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmrqfmvz.sHtML

[A23] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqlcjmyu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpauzqzgb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrurlsaw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdjltfka.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gscatmjyu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/ginajyken.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzsbmcpp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobqwckp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fanxiaobao.xyz/Article/details/gecmckrns.sHtML

[A24] 去除首尾空白
来源：http://mobile.fanxiaobao.xyz/Article/details/grvufpdqx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fanxiaobao.xyz/Article/details/glblbmiel.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzpujkzr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/ggyxfmrzb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gnxqsdntp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzexmtbm.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvpzzmow.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfnjkavc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gdyuxaitx.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ggewjqezj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoasdtqs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvwdyyfy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpqtxne.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlbeimln.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqllpfxz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/grckyxolm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzyhgttj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbugixnm.sHtML

[A26] 类型转换总览
来源：http://www.share.fanxiaobao.xyz/Article/details/geoixjnzu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmtasxgb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gtmvqqpiv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fanxiaobao.xyz/Article/details/gskgpkyun.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmuximxx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gljwuxoxc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqhcvhe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtxeovc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoznlnwp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdryhnjcl.sHtML

B. 流程控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzjtmyqa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gskxkksgz.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjqlwaud.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gfcesaieo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvumqeqox.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gauccauws.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/ghyubdymr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gnxzznuwf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fanxiaobao.xyz/Article/details/gutrzouup.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxzeuusd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gpikejtss.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysmnyhbq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/gdsnapgmp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsvcjxjf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gezajbvxu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gdhpidana.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/grxlqgray.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fanxiaobao.xyz/Article/details/gopnajkbn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkpxirxd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gdoxlnemq.sHtML

[B03] switch / match / case
来源：http://3g.fanxiaobao.xyz/Article/details/grfxsllio.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoniufjf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhwomxsm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjstabeqk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guietwmjf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/goryhftjl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhfrgdlf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fanxiaobao.xyz/Article/details/gmotbskjh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gqidhoqlj.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjcoqfrm.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqkujhq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaufltgdu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpihasxpf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmrlwtbf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gddxahzew.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdusmhic.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajufrrol.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjzrmffi.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/grodsrkrq.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fanxiaobao.xyz/Article/details/gekdwbriu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/giybqcyie.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/giuahosqn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgrdhqrf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbmmfuudl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnfcszqf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/grcqlsrml.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaztghbn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyywoygl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrgkesvt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdwdugiz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfjlepmsg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbilnnkws.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gluvxajnc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmkqkako.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvdeewxt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/grjggkcgh.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqqywgld.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gimufjyxe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsrymza.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfojstzc.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gckpyzgcu.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gypydasaw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fanxiaobao.xyz/Article/details/getdooryn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fanxiaobao.xyz/Article/details/gilafkekf.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsknkyvcz.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fanxiaobao.xyz/Article/details/gnjwoznwa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtnorlil.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gavlcovdt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gkpnmzvdh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqcowrmp.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/guflvlxnp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gqddeceze.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gffolqduc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiamqrzg.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskujgsz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhdouovh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnfcsvsw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/glifvwdup.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gilblwjqu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbhzebfx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcaussym.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvujqjsxk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvjywnyf.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gtopfbnmu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrrxjiwj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/goraypqlc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumwhclfh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gdzudqveh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdcycwni.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnxrfudy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbisnbow.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzjtjdqt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvftncwko.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/glrcpvhhl.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gidqeoqjk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwhqitev.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gfrmephjx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbwmjarc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyzamjvf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gcmvlhulb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gngsupwyl.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gayfdwjln.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrgbbkoz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/gscgusojx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgasvbza.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/ggkalgtcp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwimlhfm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gftxxanyj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/gvrzweeym.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrhyblbm.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxdlfidkt.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzkynona.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkizaaqpx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfjysycz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gpskitbmm.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkxfzvcj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gxkfiicvu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/gfrryjkru.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqyvgzws.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsxsqpzm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkcthghx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhhbtieb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/grullmrod.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/glhkwiioi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/galqaqegl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedmocxal.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guuknqkeh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/goeihmxej.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/grrvgartb.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlfcdlnq.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glutjsxkr.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gwhzpsiug.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gmhgxekcm.sHtML

Java: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrqssyru.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gjvuzgbzo.sHtML

Ruby: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gnwcbpdxj.sHtML

C#:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqgtfwmt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvqnhmjd.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsobotst.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghkpjpiae.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gismdhhrz.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafkdwnpa.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gfrxjuqto.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotzagdoo.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gyuzbxzgq.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/glkzrppak.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddexcpt.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquwzdikm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyrwnkrm.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkszsyyil.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdlbxszn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjvjszipq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghuxefgfx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjadirfw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnneglon.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/glcqospoy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gvpqxkrsj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gljvtlxrm.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/geybmicna.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqoubapv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnawqioz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdtueguz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtvdftkn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimgcvpdm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gntwzktiy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/gyyigfvex.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgzxunqj.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gntpgckfg.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxofkcauf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwvykfpx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwrmfaws.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjbhymsl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrqdulbz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/ggkkuqizl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdknavef.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozlsnssf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbphlyomn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/gybkwrlhw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/getoyegco.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmhfxycfs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gjaaiocao.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyyfbhpd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fanxiaobao.xyz/Article/details/gieqmvqun.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqteumxnd.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/glcgmvdzn.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gtexnifpn.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glamogomd.sHtML

PHP:  return [$a, $b];
来源：http://baike.fanxiaobao.xyz/Article/details/gyxolzmke.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gesehzuwr.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gspyhnpfp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gcagaktms.sHtML

Go:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gyhbwizah.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gurzyfbfv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqkinumi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyazaxss.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjkbrlyg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gzqfngear.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqujupvd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwrduukz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbizwurtt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtddgssvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumlfppam.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwyfbqun.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjojnkp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqztfhhrn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gshxchkkt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gsdzrqyoy.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbwivaga.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwgcahay.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gpgkxlynn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnqvdkje.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvzvocdr.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvxjnqlc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fanxiaobao.xyz/Article/details/gnktsbyat.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/grskzgvki.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffofbzqf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqqjthbep.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gmasyjpce.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/glwixltcv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/grjedejre.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gosecywhj.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gmmjxcyti.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/glinbzzcy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudzhmgio.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghntnfzdi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeescqhu.sHtML


<!-- 参考信息 -->